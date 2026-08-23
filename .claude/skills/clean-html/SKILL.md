---
name: clean-html
description: Apply a fixed set of mechanical, no-judgment text edits to every local section HTML file in one chapter folder (strip italics/bold, remove term spans and nbsp, replace figure/table numbers, remove "see" parentheticals, fix minor HTML errors). Overwrites files in place; relies on git for undo.
---

# Clean HTML (Simple / Passive Edits)

Apply a fixed, deterministic set of text-cleanup rules to every section HTML
file in **one local chapter folder**. It is meant to be passive, without user interaction. It does **not** make
judgment calls, reorganize content, touch figures, or handle key terms,
Example/Exercise boxes, headings, Further Exploration, IDEA/grammar
highlighting, or references — those are separate steps.

## Precondition — clean working tree required

Before doing anything else, check `git status` on the target chapter folder.

- If there are **any uncommitted changes** in `chapters/<NN>-<Chapter-Title-Slug>/`,
  **stop immediately** and tell the user to commit first. Do not edit any files.
- Only proceed once the working tree for that folder is clean.

## Input

Ask which chapter to process if not specified, e.g.:

> "Which chapter folder should I edit? (e.g. `chapters/07-Black-Holes/`)"

## Discovery

- List every `<NN.SS>-<Section-Title-Slug>.html` file directly inside the
  given chapter folder.
- Do **not** recurse into the chapter's `images/` subfolder or touch
  `manifest.csv`.
- Do **not** recurse into the chapter's `sources/` subfolder or touch
  `attributions.csv` or `references.csv`.
- If no matching files are found, say so and stop.

## Per-file edit rules

Apply these, in order, to each file's HTML. Read the file, apply all rules
in memory, then write the result back to the same path (overwrite in place).

1. **Remove italics** — strip `<em>` and `<i>` tags, keeping the inner text.
2. **Remove bold** — strip `<strong>` and `<b>` tags, keeping inner text,
   **except** when the tag directly wraps an `<a>` link to a key-terms page
   (href contains `Key_Terms`). Leave those completely untouched — tag,
   attributes, and all. Also do not change for for a figure thumbnail on the main chapter page or for the word Solution in an example or answer in an exercise.
   - Example — change this: `<strong>text</strong>` → `text`
   - Example — do **not** change this:
     `<strong><a href="/Workbench/.../13.07%3A_Key_Terms#nova" target="_blank" title="nova">nova</a></strong>`
   - Example - do **not** change this: `<strong>Thumbnail</strong>` on the main chapter page, usually NN.00-Introduction.html
   - Example: for Exercises and Examples, do **not** change `<strong>Answer</strong>` or `<strong>Solution</strong>`. 
3. **Remove term spans** — replace
   `<span class="no-emphasis" data-type="term" ...>text</span>` with just
   `text` or  `<span data-type="term" ...>text</span>` with just
   `text`.
4. **Remove `&nbsp;`** — replace with a single regular space if a space is
   needed for readability at that point; otherwise remove it entirely with
   no replacement.
5. **Replace specific Figure/Table numbers** — in paragraph text and figure/table markup. (not
   headers), replace any literal
   figure/table number like "Figure 21.5" or "Table 18.1" with
   `Figure \(\PageIndex{1}\)` or `Table \(\PageIndex{1}\)`.
6. **Remove parenthetical "see" references** — remove parenthetical text
   that begins with "see," keeping any Figure reference unwrapped:
   - `(see Figure \(\PageIndex{1}\))` → `Figure \(\PageIndex{1}\)`
   - `(Figure \(\PageIndex{1}\))` → `Figure \(\PageIndex{1}\)`
   - `(see Active Galaxies, Quasars...)` → removed entirely
   - Parentheses wrapping an entire sentence (or more) → remove the parentheses, leave the sentence Example: Change `(sentence)` to `sentence`
   - In-text citations like `(Urton, 1981)` → removed
7. **Correct minor HTML errors** — fix small, obvious structural issues
   (unclosed tags, mismatched quotes). Do not restructure or reorder content.
8. **Remove breaks** - Remove `<br />`. Paragraph text should end with `</p>`

## Hard exclusions — never modify or remove, under any rule above

- Anything inside a `<strong><a href="...Key_Terms...">...</a></strong>`
  key-term link.
- `<img>` `src` attributes or any figure numbering/indices.
- Class attributes from header or paragraph tags. e.g. 
- Anything not explicitly covered by rules 1–8 above (Example/Exercise
  boxes, Further Exploration, learning objectives, IDEA/grammar
  highlighting, paragraph reordering, references formatting).

## Output

After processing each file, overwrite it in place and print a one-line
summary of what changed, e.g.:

```
3.02-Stellar-Winds.html: 4 nbsp removed, 2 <em> stripped, 1 <strong> stripped,
1 figure reference replaced, 1 "see" parenthetical removed
```

After the whole chapter is done, print a chapter-level total across all
files and all rule types.

## Logging

Append an entry to today's session file (`sessions/<date>-sessionNN.md`)
under **AI**, listing: chapter processed, files touched, and total edit
counts per rule.

## After running

Remind the user:
- Review changes with `git diff` on the chapter folder before committing.