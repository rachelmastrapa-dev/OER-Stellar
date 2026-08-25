# Accessible Description Link

The accessible description link is needed to link the figure caption to the accessible description on a separate page. It requires a submitted link.

## Accessible Description Link Format

- The ccessible description link should look similar to this: `/Workbench/TextbookTitle/<NN>:_<Chapter_Title>/<NN0>.<SS>:_Accessible_Descriptions#Figure_FigureNumber_FigureTitle` where
   - `<NN>` is the chapter number and `<NN0>` is the chapter number with the leading 0 stripped off for single digit chapters
       - Example: For Chapter 2 `<NN>`is 02 while `<NN0>`is 2
       - Example: For Chapter 14 `<NN>` and `<NN0>` are both 14
   - `<SS>` is the section number

### ASTR 10 Settings

For the astronomy 10 textbook, the textbook part of the link is:

TextbookTitle: De_Anza_-_ASTR10


## Accesible Decription Link Guidelines 

- Add a `_` between empty spaces in the link
- Omit the figure number if not available.
- The figure number may appear as `\(\PageIndex{1}\)` in other parts of the figure html. Only use a numerical number in the accessible description link. It will either be a number similar to this: 4.8.1, or there will be no number at all.

## Examples

Chapter 14, section 2, first figure
Figure Number: 14.2.1
Figure Title: Binary Black Hole

Accessible description link: `/Workbench/De_Anza_-_ASTR10/14:_Black_Holes/14.06:_Accessible_Descriptions#Figure_14.2.1_Binary_Black_Hole`

Chapter 2, section 4, third figure
Figure number: 2.4.3
Figure Title: Interior of the Sun
Accessible description link: `/Workbench/De_Anza_-_ASTR10/02%3A_Night_Sky_Navigation/2.10%3A_Accessible_Descriptions#Figure_2.4.3_Interior_of_the_Sun`