# Editing Standards for ASTR 10 Stellar Textbook

## Locating files
All paths in this document start in the directory where this file is located.  
- The root directory of the git repository is found with `ROOT=$(git rev-parse --show-toplevel)`
- Example: 
   - If the location of this file is `$ROOT/guidelines/editing-standards.md` and there is a reference to a file called `learning-objectives.md` in `page-styles` then the path of the file is `$ROOT/guidelines/page-styles/learning-objectives.md`
   -If there is just a reference to a file, such as `idea-framework.pdf`, then its path is `$ROOT/guidelines/idea-framework.pdf`

## Guidelines

This is a list of general guidelines to use for all tools in this directory and any subdirectories. These guidelines are designed to help generate text appropriate for an Open Educational Resource (OER) astronomy textbook for a college general education course. Students for this course are not required to have any science or math pre-requisites, and may not have any prior knowledge of astronomy. These guidelines are meant to make the textbook accessible to the broadest range of students.

### General Guidelines

- Do not use placeholders for missing information. Instead, ask immediately. If user has stated a contingency for no information, then default to the contingency.
- Consider the Inclusivity, Diversity, Equity, and Anti-Racism when generating text using the ASCCC OERI Guide, `idea.framework.pdf`
- Follow the accessibility guidelines in `accessibility-guidelines.md`. These are the general ADA WCAG guidelines for the Libretext OER books, adapted for astronomy.
- Do not use italics unless required by APA format.
- Use bold only for key terms or in Exercise or Example boxes.
- Minimize use of quotation marks and parantheses in paragraph text.

## Terminology
- Refer to `page-styles/terminology.md`
- When generating text, use terminology that is appropriate to this textbook.
- This textbook is for an introductory course for astronomy with no math prerequisite. 
- Assume the student is not familiar with astronomy terminology.

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

### Learning Objectives
- Refer to `page-styles/learning-objectives.md`
- Learning objectives list concepts that students should know by the end of the chapter.
- They are listed in a box on the chapter page.

### Further Exploration
- Refer to `page-styles/further-exploration.md`
- A note box near the end of a section page with links for students to find more information.
- Not present on every page, only when needed.

### Example Box
- Refer to `page-styles/example-box.md`
- Format for an example box

### Exercise Box
- Refer to `page-styles/exercise-box.md`
- Format for an exercise box

## Figure Elements

### Figure Attribution
- Refer to `page-styles/figure-attribution.md`
- Figures require an attribution to give the creator credit.

### Figure HTML
- Refer to `page-styles/figure-html.md`
- Standard libretext html format for figures.

### Figure Caption Text
- Refer to `page-styles/figure-caption-text.md`
- The text in the figure caption between the title and attribution.
- Includes the main learning objective of the figure

### Alternative Text
- Refer to `page-styles/alternative-text.md`
- An alternatie text description is a brief description of the figure that is embedded in the figure.

### Figure HTML
- Refer to `page-styles/figure-html.md`
- The figure html is formatted for a Libretext textbook to display a figure.
- The figure html includes the alternative text, figure caption, figure attribution, and a link to the accessible description. 