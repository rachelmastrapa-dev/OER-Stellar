---
name: edit-html
description: Apply a fixed set of text edits to every local section HTML file in one chapter folder (move learning objectives to main chapter page, format equations in Latex, move link to learning text to a single Further Exploration box, ). Overwrites files in place; relies on git for undo.
---

# Edit HTML (Complex edits with options for user interaction)

Apply a set of rules to every section HTML file in **one local chapter folder**. Ask the user for input based on the triggers in the rules. It does **not** reorganize content, or handle key terms, headings, IDEA/grammar highlighting, or references  — those are separate steps.

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
  `manifest.csv`, `attributions.csv`.
- Do **not** recurse into the chapter's `sources/` subfolder or touch
  `attributions.csv` or `references.csv`.
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

1. **Learning Objectives**
   - Read the Learning Objectives section in `editing-standards.md`.
   - If there is not one already, create a learning objectives box on the main chapter page
     - The main chapter page should have a name similar to `<NN>.00-Introduction.html` 
     - Read the Chapter Page section in `editing-standards.md` for placement of the learning objectives box on the page.
   - Search for learning objectives boxes on each section page, based on boxes similar to the format for learning objecive boxes given in `editing-standards.md`.
     - For found learning objectives boxes.
       - Move the learning objectives from section pages into the box on the main chapter page. 
        - Move them unedited, they will be edited manually by user. 
        - Keep any class attributes in the HTML. Example: In `<li class="lt-phys-64811">Describe how the concept of a singularity disagrees with our current understanding of the behavior of matter</li>` keep `class="lt-phys-64811"` when transfering to main chapter page.
        - Delete the empty learning objectives boxes on the section pages.
     - Is found text is similar to learning objectives boxes, but does not match formatting, e.g. has a different list structure, then ask user and follow instructions. 
     - If there are no learning objectives boxes, go to next step.

2. **Format equations in LaTeX**:
   - Convert equations in MathML to Latex.
   - Do **not** use `$$...$$` wrappers, instead use:
     - For inline equations → wrap with `\(...\)`
     - For block or display equations → wrap with `\[...\nonumber\]`
   - Plain variables that are not inside an equation (e.g. `H<sub>0</sub>`,
     `v is the velocity...`, `P<sup>2</sup>`) stay as normal HTML text, no italics.
   - Very simple equations in paragraph text can be in HTML e.g. `P<sup>2</sup>=a<sup>3</sup>`
   - Numbers that are in paragraph text should be plain text or simple HTML, e.g. `1.0` and `1.5 x 10<sup>8</sup>`
   - **Never** touch equations inside figure or table markup — leave those
     exactly as-is.

3. **Further Exploration**
  - Refer to the Further Exploration section in `editing-standards.md`.
  - If you find any note boxes with Link to Learning in their header and is similar to this: 
  `<div class="box-note"> <h5 class="box-legend"><span class="lt-icon-default">Link to Learning</span></h5><p>Text with an external link</p></div>` then do the following.  If there are no box notes similar to this, go to the next rule.
     - Read the Section Page section in `editing-standards.md` for placement of the further exploration box on the page. 
     - Create a note box called Further Exploration with format an placement according to editing standards.
     - Move all of the statements in link to learning boxes to the Further Exploration box
     - The URL in the text redirects to another URL. 
       - Use WebFetch on the given URL to find the redirected URL. 
       - If the link can't be found, alert the user. 
          - Ask for a link to use, or if you should continue without changing the link. 
          - Do what the user says and continue. 
       - If WebFetch returns a working URL, replace the link in the HTML with the WebFetch returned URL. Example: replace `https://openstax.org/l/30ndegtystidfor` with `https://www.youtube.com/watch?v=h1iJXOUMJpg`
4. **Examples and Exercises**
   - Refer to the Example Box section, the Exercise Box section, and the Section Page section in `editing-standards.md`.
   - Search for any headers that include Example or Exercise or any Exercise or Example Boxes. If you don't find anything, then you are done with this rule. If you find anything, do the following: 
     - Create a header for the Examples and Exercises section in the position and format according to editing standards for a section page.
     - For found text that starts with a header that starts with "Example," and has some text in the section that looks like an example problem, then ask the user if it should be put in an Example box.
        - If user says yes:
          - Create an Example box according to editing standards.
          - Move the text from the section into the Example box, using a layout according to editing standards.
          - Move the new Example Box to the Examples and Exercises section.
     - For found text that starts with a header that starts with "Exercise," and has some text in the section that looks like an exercise problem, then ask the user if it should be put in an Exercise box:
        - If user says yes: 
           - Create an Exercise box according to editing standards.
           - Move the text from the section into the Example box, using a layout according to editing standards.
           - Move the new Exercise Box to the Examples and Exercises section.
     - For found text that are intact Exercise or Example boxes similar to those in editing standards, move them to the Examples and Exercises section.

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