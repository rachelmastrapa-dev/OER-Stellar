# Editing Standards for ASTR 10 Stellar Textbook

## Locating files
All paths in this document start in the directory where this file is located.  
- The root directory of the git repository is found with `ROOT=$(git rev-parse --show-toplevel)`
- Example: 
   - If the location of this file is `$ROOT/guidelines/editing-standards.md` and there is a reference to a file called `learning-objectives.md` in `page-styles` then the path of the file is `$ROOT/guidelines/page-styles/learning-objectives.md`
   -If there is just a reference to a file, such as `idea-framework.pdf`, then its path is `$ROOT/guidelines/idea-framework.pdf`

## Page Styles

### Chapter Page
- Refer to `page-styles/chapter-page.md`
- Format for the main page of the chapter
- Contains an introduction paragrph learning objectives and table of contents

### Section Page
- Refer to `page-styles/section-page.md`
- Pages of content for a chapter in the textbook.
- May contain various page elements.

## Page Elements

## Learning Objectives
- Refer to `page-styles/learning-objectives.md`
- Learning objectives list concepts that students should know by the end of the chapter.
- They are listed in a box on the chapter page.

## Further Exploration
- Refer to `page-styles/further-exploration.md`
- A note box near the end of a section page with links for students to find more information.
- Not present on every page, only when needed.

## Example Box
- Refer to `page-styles/example-box.md`
- Format for an example box

## Exercise Box
- Refer to `page-styles/exercise-box.md`
- Format for an exercise box

## Figure Attribution
- Refer to `page-styles/figure-attribution.md`
- Figures require an attribution to give the creator credit.

## Figure HTML
- Refer to `page-styles/figure-html.md`
- Standard libretext html format for figures.
