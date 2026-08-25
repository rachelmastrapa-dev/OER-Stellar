# Figure HTML

## Figure HTML Format

Refer to editing standards for detailed descriptions for each of the elements in the HTML.
The html format for the figure html is:

<figure><img alt="alt-text. Details in caption." class="internal default" src="ImageName" /> <figcaption>Figure \(\PageIndex{i}\) : Title. Figure Caption text. (figure attribution) <a href="acc-desc-link" target="_blank" title="Accessible Descriptions">Accessible description of Figure \(\PageIndex{i}\)</a>.</figcaption> </figure>

where 
Image name is the image name from the original figure html = found in `src="original-imagename" Do not change this from the original value. 
i is the figure index - 1 for the first figure on the page, 2 for the second figure, etc.
Title is the title of the figure
Figure caption text is the figure caption text generated for this image.
figure attribution is the figure attribution generated for this image.
acc-desc-link is the accessible description link 

# Figure HTML Guidelines

- When generating the new figure HTML,  update both occurrances of `\(\PageIndex{i}\)` with the value of the figure index. Example: If the figure index is 5, both occurances should be `\(\PageIndex{5}\)`
   - The figure index can also be found at the end of the figure number.  Example: If the figure number is 2.3.1, then both occurances should be `\(\PageIndex{1}\)`
- The title can be found in the figure caption of the submitted figure html.  It should be in between the figure number and figure caption text: `\(\PageIndex{1}\) : Title. Figure Caption text.` Use the submitted title to format the figure html. If there is no obvious title, ask user for it.

## Examples

## Example 1

- alt-text: Neutron Star RX J1856.5-3754 by Hubble Space Telescope
- ImageName: /@api/deki/files/42859/figure-213-isolatedNeutronStar.jpg
- Title: Neutron Star RX J1856.5-3754
- Figure Caption text: This Hubble Space telescope image is the first direct observation of a neutron star, labeled with an arrow, in visible light.
- figure attribution - <a href="https://creativecommons.org/licenses/by/4.0/" target="_blank" title="CC BY 4.0">CC BY 4.0</a>; <a href="https://www.nasa.gov/" target="_blank" title="Fred Walter (State University of New York at Stony Brook) and NASA/ESA">Fred Walter (State University of New York at Stony Brook) and NASA/ESA</a> via <a href="https://esahubble.org/images/opo9732a/" target="_blank" title="ESA Hubble">ESA Hubble</a>
- accesible-description-link: /Workbench/De_Anza_-_ASTR10/13:_Stellar_Finale/13.08:_Accessible_Descriptions#Figure_13.4.1_Neutron_Star_RX_J1856.5.E2.88.923754

The html should be:

<figure><img alt="Neutron Star RX J1856.5-3754 by Hubble Space Telescope. Details in caption." class="internal default" src="/@api/deki/files/42859/figure-213-isolatedNeutronStar.jpg" /><figcaption>Figure \(\PageIndex{1}\) : Neutron Star RX J1856.5-3754. This Hubble Space telescope image is the first direct observation of a neutron star, labeled with an arrow, in visible light. (<a href="https://creativecommons.org/licenses/by/4.0/" target="_blank" title="CC BY 4.0">CC BY 4.0</a>; <a href="https://www.nasa.gov/" target="_blank" title="Fred Walter (State University of New York at Stony Brook) and NASA/ESA">Fred Walter (State University of New York at Stony Brook) and NASA/ESA</a> via <a href="https://esahubble.org/images/opo9732a/" target="_blank" title="ESA Hubble">ESA Hubble</a>) <a href="/Workbench/De_Anza_-_ASTR10/13:_Stellar_Finale/13.08:_Accessible_Descriptions#Figure_13.4.1_Neutron_Star_RX_J1856.5.E2.88.923754" target="_blank" title="13.8: Accessible Descriptions">Alternative description of Figure \(\PageIndex{1}\)</a>.</figcaption></figure>

## Example 2

- alt-text: SN 1006 in X-ray, infrared, and visible light
- ImageName: /@api/deki/files/46059/7c6fd59f47b3a3d89cf431e8ba9d417f6d39356f
- Title: SN 1006
- Figure Caption text: 1000 years later, the remnant of SN 1006 can be detected with X-ray and radio observations
- LicenseLink: https://creativecommons.org/licenses/by/4.0/
- License: CC BY 4.0
- AuthorLink: https://openstax.org/books/astronomy-2e/pages/preface
- Author: Fraknoi, et al.
- FigureLink: https://openstax.org/details/books/astronomy
- Source: Openstax Astronomy 2nd ed.
- accesible-description-link: /Workbench/De_Anza_-_ASTR10/13:_Stellar_Finale/13.08:_Accessible_Descriptions#Figure_13.3.1_SN_1006

The html should be:

<figure><img alt="SN 1006 in X-ray, infrared, and visible light. Details in caption." class="internal default" src="/@api/deki/files/46059/7c6fd59f47b3a3d89cf431e8ba9d417f6d39356f" /> <figcaption>Figure \(\PageIndex{1}\) : SN 1006. 1000 years later, the remnant of SN 1006 can be detected with X-ray and radio observations. (<a href="https://creativecommons.org/licenses/by/4.0/" target="_blank" title="CC BY 4.0">CC BY 4.0</a>; <a href="https://openstax.org/books/astronomy-2e/pages/preface" target="_blank" title="Fraknoi, et al.">Fraknoi, et al.</a> via <a href="https://openstax.org/details/books/astronomy" target="_blank" title="Openstax Astronomy 2nd ed.">Openstax Astronomy 2nd ed.</a>) <a href="/Workbench/De_Anza_-_ASTR10/13:_Stellar_Finale/13.08:_Accessible_Descriptions#Figure_13.3.1_SN_1006" target="_blank" title="13.8: Accessible Descriptions">Alternative description of Figure \(\PageIndex{1}\)</a>.</figcaption> </figure>


