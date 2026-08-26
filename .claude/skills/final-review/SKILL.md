---
name: final-review
description: Make a final pass through the text for the chapter. This skill is designed to streamline the editing process for an Open Educational Resource (OER) astronomy textbook in Libtetext.
---

# Final Review

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

1. Check each file for spelling, grammar, and html errors.
- if the corrections are small, make the change e.g errors that are up to 3 words long, mispelled words, bad punctuation, mismatched tenses, etc.
- If an error is more complex, more than 3 words long, or will change the meaning of a sentence, or change the functionality of the html, ask the user for guidance.  
<!-- add accessibility and IDEA? -->


## Hard exclusions — never modify or remove, under any rule above

- Class attributes from header, list, or paragraph tags. e.g. `<li class="lt-phys-64811">`
- Anything not explicitly covered by rules 1 above 

## Output

After processing each file, overwrite it in place and print a one-line
summary of what changed, e.g.:

```
3.02-Stellar-Winds.html: 2 spelling errors found and corrected, no egrammar or html errors found.

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