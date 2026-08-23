---
name: edit-html
description: Apply a fixed set of text edits to every local section HTML file in one chapter folder (move learning objectives to main chapter page, format equations in Latex, move link to learning text to a single Further Exploration box, ). Overwrites files in place; relies on git for undo.
---

# Edit HTML (Complex edits with options for user interaction)

Apply a set of rules to every section HTML file in **one local chapter folder**. This mirrors the steps in `astro10-editing-workflow.md` for Claude/AI user intersactions. Ask the user for input based on the triggers in the rules. It does **not** reorganize content, or handle key terms, headings, IDEA/grammar highlighting, or references  — those are separate steps.

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
  `manifest.csv`, `attributions.csv`.
- Do **not** recurse into the chapter's `sources/` subfolder or touch
  `attributions.csv` or `references.csv`.
- If no matching files are found, say so and stop.

## Per-file edit rules

Apply these, in order, to each file's HTML. Read the file, apply all rules
in memory, if a judgement needs to be made, ask the user, otherwise complete tasks, then write the result back to the same path (overwrite in place). 

1. **Learning Objectives**
   - Read `guidelines/page-styles/learning-objectives.md` for formatting guide and HTML examples of learning objectives.
   - If there is not one already, create a learning objectives box on the main chapter page, `<NN>.00-Introduction.html`, according to the layout in `guidelines/page-styles/chapter-page.md`
   - Search for learning objectives boxes on each section page, based on boxes similar to the format in `guidelines/page-styles/learning-objectives.md`.
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
     `v is the velocity...`) stay as normal HTML text, no italics.
   - **Never** touch equations inside figure or table markup — leave those
     exactly as-is.
3. **Further Exploration**
  - If you find any note boxes with Link to Learning in their header and that is similar to this: 
  `<div class="box-note"> <h5 class="box-legend"><span class="lt-icon-default">Link to Learning</span></h5><p>Text with an external link</p></div>` then do the following.  If there are no box notes similar to this, go to the next rule.
     - Create a note box at the end of the page called Further Exploration
       - The box should be located at the end, before or after different headers according to the layout in `guidelines/page-styles/section-page.md`
       - The format of the box is in `guidelines/page-styles/further-exploration.md`
     - Move all of the statements in link to learning boxes to the Further Exploration box
     - The URL in the text redirects to another URL. 
       - Use WebFetch on the given URL to find the redirected URL. 
       - If the link can't be found, alert the user. 
          - Ask for a link to use, or if you should continue without changing the link. 
          - Do what the user says and continue. 
       - If WebFetch returns a working URL, replace the link in the HTML with the WebFetch returned URL. Example: replace `https://openstax.org/l/30ndegtystidfor` with `https://www.youtube.com/watch?v=h1iJXOUMJpg`
4. **Examples and Exercises**
   - Search for any headers that include Example or Exercise or any Exercise or Example Boxes. If you don't find anything, then you are done with this rule. If you find anything, do the following: 
     - Create a header for the Examples and Exercises section in the position on the page and style given in `guidelines/page-styles/section-page.md`
     - For found text that starts with a header that starts with "Example," and has some text in the section that looks like an example problem, then ask the user if it should be put in an Example box.
        - If user says yes:
          - Create an Example box using the format from `guidelines/page-styles/example-box.md`
          - Move the text from the section into the Example box, using the layout in `guidelines/page-styles/example-box.md`.
          - Move the new Example Box to the Examples and Exercises section.
     - For found text that starts with a header that starts with "Exercise," and has some text in the section that looks like an exercise problem, then ask the user if it should be put in an Exercise box:
        - If user says yes: 
           - Create an Exercise box using the format from `guidelines/page-styles/exercise-box.md`
           - Move the text from the section into the Example box, using the layout in `guidelines/page-styles/exercise-box.md`.
           - Move the new Exercises Box to the Examples and Exercises section.
     - For found text that are intact Exercise or Example boxes similar to those in `guidelines/page-styles/example-box.md` or `guidelines/page-styles/exercise-box.md`, move them to the Examples and Exercises section.

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