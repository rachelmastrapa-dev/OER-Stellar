# Editing Instructions for ASTR10
## Starting Day
1. Create new issue in git
    1. Editing for the day with date
    2. List goals for the day
2. Move issue to working in project, assign self, create branch
3. Create new session file for today in VSCodium
4. Starting Claude Code
    1. Open a terminal command prompt 
    2. Navigate to repo cd Crap\OERAI\git_repos\OER-Stellar
    3. Type claude
    4. Exit when not using
5. **Commit often! Keep careful session notes!**

## Ending Day
1. List questions/goals for tomorrow in session file
2. Save and close all files, commit, merge branches.

## Whole Chapter - Manual in Libretext
- Change last section to Accessible Descriptions
- Remove chapter summaries
- Edit main chapter page
  - Have page start with an H2 Introduction before learning objectives and short summary paragraph.
  - check size of thumbnail image and format attribution  
- Change chapter titles - shorten, clarify
- **Delete Extra material** - on the chapter/section level
- **Delete extra figures**
- Commit changes in Conductor

## Libretext export - - Claude/AI Passive
If starting new project, use libretext to harvest book to repo using export-book and libretext-export, or do chapter by chapter


### Clean HTML - Claude/AI Passive
- Read .claude/clean-html/SKILL.md
- Summary, removing italics, bold, spans, figure ## set to default, etc.



### Edit HTML - Claude/AI user interactions

**User: Commit and close all files**
Ask for help!
1. Move all learning objectives to main chapter page.
2. Change equations from MathML to Latex.
3. Move all link to learning items to Further Exploration. 
4. Put example and exercises in boxes and move to the correct section.
<!-- include review of terminology?, remove parens about put comments for rephrasing of same concept  Future: remove text from other boxes?, remove quote marks that are not for dialog-->



## Chapter Review - Manual   

**User: Commit and close all files**
- main chapter page
  - format thumbnail - copy from another example
  - Have page start with an H2 Introduction before learning objectives and short summary paragraph.
  - reduce to 10 or fewer learning objectives (no learning objectives on sub-pages)
- Content
  -  Delete extra text 
      - footnotes
      - references to other chapters
  - Organize page structure
    - Start with <h2> make sure all headers are nested
  - search and replace
    - '  solar system revolve
    - change titles in exercise and example boxes - delete number in example. copy title to exercise
    
- Figures
  - add titles 
  - check index
  - check against files, manifest
  - log - att info or (Openstax Astronomy)
  - contextualize figures and tables.
- key terms 
   -  find in text and log
- Further Exploration
   - check for full link
   - contextualize further exploration links
- text attribution
  - log
- References 
   - log


## Tasks to do when late and exhausted

Copy (Openstax Astronomy) into every figure caption

### Logging 

- references 
  - sources/references.csv
- text attributions 
  - not in libretext auto-attribution
  - sources/text-attributions.csv
  - section, title,	link, source title,	source link, author, author link, license, license Link
- figure attribution info 
  - sources/figure-attributions.csv
  - section, title, license, license link, author, author link, source, image link, figure link
- key terms 
  - key-term.csv
  - section,term,definition

<!-->  - class attributes - connecting to location default attribute?  page attribute? < -->

## Format Figures - Claude AI - more astro figs to skills in ASTR10

**User: Commit and close all files**

- Increment Figure indices??
- Accesible Descriptions
- alt-text
- Figure attribution
- Figure HTML



## Format Sources - Claude/AI Passive

**User: Commit and close all files**

References, manual attributions - per section page?, need style files for each


## Format Key Terms - Claude AI Passive

**User: Commit and close all files**

- Key terms
  - Check against key terms list from Openstax and create list for chapter
  - Format terms and definitions and add to key terms page
  - Find first occurance of term in chapter paragraph text, not figure, table, or heading 
     - format text to bold and link
     - handle whether in plural or singular in paragraph text.

## Final Review - Claude/AI - interactive? - skip for now

**User: Commit and close all files**

make suggestions - search for outer material??. accesibility
1. Make minor grammar and spelling errors.
2. Ask about more complicated errors
<!--12. **Highlight IDEA Framework issues in red** — Flag content in paragraph text that does not meet IDEA (Inclusion, Diversity, Equity, and Access) standards using `<span class="mt-bgcolor-c0392b">text</span>`. For non-text material (figures, headers), describe recommended changes in a list.
<-->

## Final Check- Manual
- Manually paste each page and check for functionality.
  - check size of thumbnail image  for main chapter page   
- Commit changes in Conductor 
- Update progress log.
- Notify Jyothsna that it is done. 
- When you make corrections, update progress again. 

## Reviews
- check Caitling and Jyothsnas - link here?
- wait for accessibility review?

## Jyothsna
- Main chapter page 
  - start with H2 Introduction and brief summary
- Remove all section summaries
- Change name of last page to Accessible Descriptions

