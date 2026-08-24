# Accessible Descriptions

## Definition of Accessible Description
Accessible description are for students that are not able to process visual images without other options. An accessible description is significantly longer than alt-text. 

## Format of Accessible Description
- The first line is the figure number and title.
- The second line is a brief description of the figure.
- The format of the rest of the description depends strongly on the type of image. In general, it should be broken up into separate sections using sub-headers. If the description is lengthy, break it into brief statements in a bulleted list, describing some components using nested bullets. Refer to examples below.
- If there is an image credit in the supporting text, include it as the last line of the description
  - Examples of credits in supportin text: (credit: Adam Evans) or (credit: modification of work by Hubble Legacy Archive, NASA, ESA, and Judy Schmidt).
  - Remove text similar to "modification of work by" Examples of edited text for accessible description: Credit: Adam Evans or Credit: Hubble Legacy Archive, NASA, ESA, and Judy Schmidt.

<!-- Follow any general guidelines in astro_figs.html, such as which words are appropriate for the textbook. -->


## Accessible Description Guidelines
Follow these guidelines when generating accesible descriptions.

### Accessible descriptions should answer four questions:

1. What is shown?
2. What relationships or patterns matter?
3. What labels or text must students know?
4. What is the instructional takeaway?

### What to include

- Title of the visual (if present)
- Scope (what area, system, or process is shown)
- Key parts, axes, or regions, or objects
    - For astronomical objects, includes the proper name or the type of astronomical object or objects and a physical description of the object or objects. e.g. The three bright stars in the belt of the constellation Orion.
- Relationships, trends, or sequences
- Labels that are instructionally important
- Conclusions students should draw
- Supporting text:
  - Always use any supporting text, if provided. Generate additional description if obvious components are missing.
  - The relevant supporting text may be in the html in the form of the original figure caption text, figure title, image credit, and original alt text.
  - If there is no supporting text, generate a description based on the image.

### Guidelines for Complex Figures
- If the figure has multiple subfigures:
  - If the individual figures are numbered or use letters to identify them, then refer to them in the caption by figure type and number or letter. Examples: Image (a), Chart 2.
  - If the individual figures have complex labels, refer to them by the figure type and label. Examples: the image labeled Orion nebula, the chart labeled H-R Diagram.
  - If the individual figures are not labeled or numbered any any way, then refer to the subfigures as panels and refer to them by location. 
     - If there is a single row, number them and refer to them from left to right. 
     - If there is a single column, refer to them as top, middle, and bottom. 
     - If there are multiple columns or rows, use a combination such as top right, center left, etc.  Start at the upper left and finish at the bottom right.

<!-- The H-R diagram is a standard chart used in astronomy. Always remember these characteristics. -->

### What to Avoid

- Exhaustive visual detail
- Stylistic descriptions
- Conclusions beyond what is in the figure - describe only what is actually present.

## Address Color and Visual Encoding

Color is almost always important in astronomy figures: If there is no explanation of the meaning of color, ask the content expert.

- Explicitly describe the meaning of color in text
- Always describe color in images
- For false color images, explain how the colors are assigned if available, or include the wavelength of the light. Example: An infrared image of the Crab nebula

When describing the instructional takeaway, use color when it is relevant. Otherwise, describe what the color represents. Examples:

- In this globular cluster, the blue stars are larger and bright than the yellow stars.
- There is more detail of the complex structure in the infrared image of the Crab Nebula compared to the visible image.

## Handle Images That Contain Text

If the image includes text students need to know, include verbatim in the accessible description

Examples:

- Chart titles, axis labels, data ranges
- Diagram labels
- Map legends
