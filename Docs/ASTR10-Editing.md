# Editing Instructions for ASTR10
## Starting Day
1. Create new issue in git
2. Make new branch
3. Open log, AI log, and this file 
## Ending Day
Close all files, commit, merge branches.
## Whole Chapter - Manual
- key terms
  - note possible key terms
  - Copy key terms from Openstax and add to log. for chapter and general  - check general log
- remove chapter summaries
- change last section to Accessible Descriptions
- shorten chapter, section, and subsection headings.
- More links to end - call Further Exploration
- Go over remixed material on each page and make sure it is on correct page. 
- Delete extra materials
- log references
- Commit changes in Conductor
- Learning objectives already moved - need to do this an agentic AI project

## Jyothsna
- Main chapter page 
  - start with H2 Introduction and brief summary
- Remove all section summaries
- Change name of last page to Accessible Descriptions

## Format HTML - Playlab AI
Made new app with instructions in document. 
1. Copy in html of entire page.
2. Copy text output to AI Log 
    1. Click on copy button at bottom.
    2. Copy into plain text.
    3. Ignore html, just copy markdown
    4. Copy markdown into log.
3. Copy html to a scratch file (Appendices) and make sure it works. 
4. Review reccomendation and implement or not
    1. Note what had term html and decide if it is a key term and add to key term list with def
    2. highlighted text
    3. headers
5. rerun if necessary
6. Overwrite chapter page when ready.
 

### App Processing Steps
1. **Remove italics** — Strip all `<em>` or `<i>` tags from the text.
2. **Remove bold** — Remove `<strong>` or `<b>` tags, *except* when they wrap a link to a key terms page.
3. **Remove term spans** — Replace `<span class="no-emphasis" data-type="term" ...>text</span>` with just the plain text.
4. **Remove `&nbsp;`** — Replace non-breaking spaces with a regular space if a space is needed, or remove them entirely if no space is needed.
5. **Replace Figure and Table numbers** — Replace all specific Figure and Table numbers (e.g., Figure 21.5, Table 18.1) with `Figure XXX` or `Table XXX`.
6. **Remove parenthetical "see" references** — Remove parenthetical text that begins with "see" but keep any Figure XXX reference. For example:
   - `(see Figure XXX)` → `Figure XXX`
   - `(Figure XXX)` → `Figure XXX`
   - `(see Active Galaxies, Quasars...)` → removed entirely
   - Parentheses around entire sentences are also removed.
7. **Correct minor HTML errors** — Fix any small structural or syntax errors in the HTML.
8. **Format Example boxes** — If a header starts with "Example," reformat it into a styled example box with the header text as the box legend and the section text inside the box.
9. **Format Exercise boxes** — If a header starts with "Exercise," reformat it into a styled exercise box, with the header as the legend, section text inside, and any answer text moved to the answer section.
10. **Format Further Exploration sections** — Place all text in a "Further Exploration" section inside a styled note box.
11. **Highlight spelling/grammar errors in orange** — Do not correct them; instead wrap them in `<span class="mt-bgcolor-e67e22">text</span>`.
12. **Highlight IDEA Framework issues in red** — Flag content in paragraph text that does not meet IDEA (Inclusion, Diversity, Equity, and Access) standards using `<span class="mt-bgcolor-c0392b">text</span>`. For non-text material (figures, headers), describe recommended changes in a list.
13. **Format equations in KaTeX** — Convert all equations to KaTeX formatting:
    - Inline equations: wrap with `BSOP...BSCP`
    - Block equations: wrap with `BSOB...\nonumberBSCB`
    - Variables not in equations are rendered as plain HTML text with no italics.
14. **Move paragraphs logically** — Rearrange paragraphs to their most logical location within the document. Maintain all class attributes. Do not change paragraph content.
15. **Format references in APA** — Format any references found in the HTML into APA style, organized in a References section. Delete extraneous text in that section

### After Returning the HTML, I Also Provide:
- **Current date**
- **A numbered list of every change made**, including reasoning for any highlighted text
- **A list of recommended changes** for non-text material or other issues
- **Recommended section headers**, including nested topics, starting with an H2 header and introductory paragraph
- **An AI citation in APA format**

## HTML Review - Manual 
- Make sure remixed material is in the correct section.
- Delete extra text or figures.
- log attribution info, including codes                
- Log attribution info for figures and give them titles.
- Figure: Do a global search and replace of XXX with  \(\PageIndex{1}\). 
- Equations: global search for $$ - replace in libretext first to make right and left paren?
  - Inline: \(equation\)
  - Display/Block: \[equation nonumber\]
- log references, key terms, etc.

## Format Figures - Claude AI
The general idea is to copy in the figure, and then the html of the figure and some of the text around it in html.  also add the title of the figure. and attribution data, or https://github.com/rachelmastrapa-dev/astro_figspreformated attribution for openstax, give link to accessible description page. See github package for full details.  
- copy in image, old figure html, 
  - if needed - accessible description link ( start with /Workbench), figure title, default attribution, or attribution information, figure. 
  - Will use attribution from last figure and increment from last figure #
- copy all results to AI log.
- first copy accesible description into accessible descriptions and save!
- copy old caption and alt-text to  and new figure html to chapter text 
- check links
- edit
  - Change indices to correct figure number
  - improve wording of caption, alt-text and accessible description.

## Final Edit - Manual
**The Milky Way Galaxy -all**
- Edit in html to avoid nbsp
- Manually update figure indices 
- Edit    
  - Address all highlighted text. 
  - Edit for consistent tone
  - Simplify language. 
- highlight key terms in green and log
- contextualize links
- manually relink all accessible descriptions
- format any references, attributions, etc.

**Chapter Done?**

## Format Key Terms - Playlab AI
- use chatbot
  - when done, type done, and copy to AI log
  - check openstax for key terms and definitions    
  - In-text key terms are bold
  - create definitions for all terms in spreadsheet
- Use chatbot to format list
- Link term to key term page
  - Search each page for first appearance of term.
  - copy in link from AI or
    - Browse to key terms and find anchor
    - Make sure that link opens new window
- save AI report to AI log

## Edit main chapter page - manual
- Have page start with an H2 Introduction before learning objectives and short summary paragraph.
- reduce to 10 learning objectives (no learning objectives on sub-pages)
- check size of thumbnail image and format attribution  

## Final Check- Manual
- Edit in html to avoid nbsp
- check accessibility in Libretext
- Commit changes in Conductor
- Update progress log.
- Notify Jyothsna that it is done. 
- When you make corrections, update progress again. 