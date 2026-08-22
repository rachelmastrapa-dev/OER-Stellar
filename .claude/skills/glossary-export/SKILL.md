---
name: glossary-export
description: find glossary in an online textbook and save to a file.
---

# Glossary Export

## Purpose
To find the glossary or key terms for a textbook and make a list of terms and definitions. 

## Prerequisites
- Playwright MCP connected.

## Input
A single URL for an online textbook main page or table of contents.
Name of ouput file.

## Steps

1. **Search for glossary page or pages**
   Navigate to the book TOC URL with Playwright. Read the page's table of contents and collect every sub-page link that is a glossary or key terms page. If you can't find anything, ask for help.

2. **For each page link, copy the terms and definitions**
   - Navigate to the glossary page.
   - Copy the term and definition.

3. **Write to file**
   Create the output file with a header `row term, definition` if it doesn't exist yet. Append one row with a the term and definition.

4. **Alphabetize**
   When all terms have been copied, if the terms are not in alphabetical order, then alphabetize the list. Make sure to keep the appropriate definition with its term.

6. **Report back**
   After the run, let user know you are done, and report how many terms you found.

## Notes
- The skill has been written for any type of online textbook. User is responsible to check licensing and properly attribute text, or get permission for use.