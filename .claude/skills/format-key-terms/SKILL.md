---
name: format-key-terms
description: Format the key terms for a chapter. This skill is designed to streamline the process of formatting key terms for an Open Educational Resource (OER) astronomy textbook in Libtetext.
---

# Format Key Terms

Apply a set of rules to every section HTML file in **one local chapter folder**. 

## Locating repo files
Before reading any repository-relative paths below, resolve the repo root:
`ROOT=$(git rev-parse --show-toplevel)`

Reference files as `$ROOT/guidelines/editing-standards.md`, 
`$ROOT/guidelines/page-styles/example-box.md`, etc.

## Precondition — clean working tree required

Before doing anything else, check `git status` on the target chapter folder.

- If there are **any uncommitted changes** in `$ROOT/chapters/<NN>-<Chapter-Title-Slug>/`,
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
  `text-attributions.csv`, `figure-attributions.csv` or `references.csv`.
- If no matching files are found, say so and stop.

## Editing Standards
The editings standards for this project are described in `$ROOT/guidelines/editing-standards.md`.  
- The `editing-standards.md` file contains brief descriptions of formatting standards.
- It also contains directions to other files that have more detailed descriptions of specific formatting standards.
- Always look in `editing-standards.md` first when looking for information about editing, formatting, or general guidance for this project, then follow the directions to other files when needed.
- If there is a rule that says to use editing standards, look for guidance in `editing-standards.md`.

## Per-file edit rules

Apply these, in order, to each file's HTML. Read the file, apply all rules
in memory, if a judgement needs to be made, ask the user, otherwise complete tasks, then write the result back to the same path (overwrite in place). 

1. Open the key terms file 
    - Read the information in `$ROOT/chapters/<NN>-<Chapter-Title-Slug>/key-terms.csv`
    - if there is no `key-terms.csv` file alert the user
    - the header of the file should be section,term,definition
    - section refers to which page in the chapter the key term link will appear on e.g. if the section is How Science Works the key term link should be written to `$ROOT/chapters/<NN>-<Chapter-Title-Slug>/<NN.SS>-How-Science-Works.html`

2. Format the Key Terms Page
    - Refer to the Key Terms Page section in `editing-standards.md`
    - Find the section file that has a name similar to `<NN.SS>-Key-Terms.html`.  This is the key terms section page.
    - Format the list of key terms according to editing standards and write them to the key terms section page.

3. For each term in `key-terms.csv`
      1. Open the section page that matches the section for the term in `key-terms.csv`
      2. Find the first occurrance of the term on the section page that is in paragraph text, **not** in figure, table, or header text.
      3. Create the link for that term according to the key terms link section in `editing-standards.md`
      4. Replace the term in the paragraph with the link. 
        - Adjust the number of the term based on context in the sentence. For example, if the term is `black hole`, but the sentence is `Astronomer love all black holes` Then make the term plural. `Astronomers love all <a <key terms link formatting> >black holes</a>`


## Hard exclusions — never modify or remove, under any rule above

- Class attributes from header, list, or paragraph tags. e.g. `<li class="lt-phys-64811">`
- Anything not explicitly covered by rules 1–3 above 

## Output

After processing each file, overwrite it in place and print a one-line
summary of what changed, e.g.:

```
3.02-Stellar-Winds.html:2 learning objectives moved, no equations found,
2 link to learning found and moved, no examples or exercises found.
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