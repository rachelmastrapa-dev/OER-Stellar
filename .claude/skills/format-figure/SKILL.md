---
name: format-figure
description: Format figure html for figures in an OER textbook, including caption text, alt-text, figure attribution, and accessible description.
---

# Format Figure

Apply a set of rules to every section HTML file in **one local chapter folder**. Ask the user for input based on the triggers in the rules.

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
  `attributions.csv`, `figure-attributions.csv` or `references.csv`.
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

1. Locate a figure in the html, e.g it starts with `<figure>` and ends with `</figure>` and do the following:
    1. Use the figure html section in editing standards to locate the alt-text and figure caption in the figure html. If present, copy the original alt-text and figure caption text into a paragraph and place the paragraph before the figure html.
    1. Create figure attribution
       - Refer to the Figure Attribution section in `editing-standards.md`
       - Locate attribution information in `$ROOT/chapters/<NN>-<Chapter-Title-Slug>/sources/figure-attributions.md`
       - In the file, find the row with matching figure title
       - The type of attribution depends on the information found in the row.
          - If the information has the figure title and a the name of a default attribution, return the default attribution found in editing standards.
          - Otherwise, use the given information to format an attribution according to editing standards.
    2. Create figure caption text <!-- read file for attribution info?  how to connect figure html to image in images  -->
       - Refer to
    3. Create the accessible description
       - Refer to
    4. Create the figure html
       - Refer to 


## Hard exclusions — never modify or remove, under any rule above

- Class attributes from header, list, or paragraph tags. e.g. `<li class="lt-phys-64811">`
- Anything not explicitly covered by rules 1–4 above 

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