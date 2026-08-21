---
name: export-book
description: Use when exporting raw editor-source HTML for a an entire book from LibreTexts Workbench into this repo. Triggers on requests like "export book [book]", "pull the HTML for [book]", "sync [book] from libretext".
---

# LibreText Book Export

## Purpose
Pull the raw editor-source HTML (not rendered page text) for every section in every chapter of a 
LibreTexts Workbench book, and save it into this repo under `chapters/`,
mirroring the chapter/section structure. 

## Prerequisites
- Playwright MCP connected and logged into the LibreTexts/Conductor session
  (persistent browser profile — should already be logged in from setup).
- Read-only task. **Never click Save, Publish, Commit, or any write/edit
  control in the LibreText editor.** This tool only reads source HTML; it
  never modifies the live page. If a step seems to require confirming a
  change, stop and ask the user first.
- The libretext-export skill

## Input
A single LibreTexts Table of Contents (TOC) URL for one a textbook, e.g.:
`https://[library].libretexts.org/Workbench/[Course]/[NN%3A_Front_Matter]/[NN%3A_Table_of_Contents]`

## Steps

1. **Discover chapter links**
   Navigate to the book TOC URL with Playwright. Read the page's sidebar/
   nested TOC tree and collect every chapter link that belongs to this
   book. Ignore any part of the table of contents that is not a numbered chapter. Ignore Licensing, Index, Glossary, and Detailed Licensing. 

2. **For each chapter link use the libretext-export skill on that link**
  

5. **Report back**
   After the run, list any errors from export-libretext.

## Notes
- If the editor's Source-view control can't be found on a given page (site
  layout can vary slightly), stop on that page, ask the user for the click
  path once, and this skill file should be updated with what worked.
- This tool copies all HTML from the page, including figures.