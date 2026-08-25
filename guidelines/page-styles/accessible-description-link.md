# Accessible Description Link

The accessible description link is needed to link the figure caption to the accessible description on a separate page. It requires a submitted link.

## Accessible Description Link Format

- The submitted link will look something similar to this: `/Workbench/TextbookTitle/ChapterTitle/`
- Use the submitted link, figure number and figure title to create the accessible description link.
- The final accessible description link should look similar to this: `/Workbench/TextbookTitle/ChapterTitle/SectionNumber:_Accessible_Descriptions#Figure_FigureNumber_FigureTitle`


## Accesible Decription Link Guidelines 

- Add a `_` between empty spaces in the link
- Omit the figure number if not available.
- The figure number may appear as `\(\PageIndex{1}\)` in other parts of the figure html. Only use a numerical number in the accessible description link. It will either be a number similar to this: 4.8.1, or there will be no number at all.

## Example

Submitted link: `/Workbench/De_Anza_-_ASTR10/14:_Black_Holes/14.06:_Accessible_Descriptions`
Figure Number: 14.2.1
Figure Title: Binary Black Hole

Accessible description link: `/Workbench/De_Anza_-_ASTR10/14:_Black_Holes/14.06:_Accessible_Descriptions#Figure_14.2.1_Binary_Black_Hole`