---
name: libretext-export
description: Use when exporting raw editor-source HTML for a chapter's sections from LibreTexts Workbench into this repo. Triggers on requests like "export chapter [name]", "pull the HTML for [chapter]", "sync [chapter] from libretext".
---

# LibreText Chapter Export

## Purpose
Pull the raw editor-source HTML (not rendered page text) for every section in a
LibreTexts Workbench chapter, and save it into this repo under `chapters/`,
mirroring the chapter/section structure. 

## Prerequisites
- Playwright MCP connected and logged into the LibreTexts/Conductor session
  (persistent browser profile — should already be logged in from setup).
- Read-only task. **Never click Save, Publish, Commit, or any write/edit
  control in the LibreText editor.** This tool only reads source HTML; it
  never modifies the live page. If a step seems to require confirming a
  change, stop and ask the user first.

## Input
A single LibreTexts Table of Contents (TOC) URL for one chapter, e.g.:
`https://[library].libretexts.org/Workbench/[Course]/[NN%3A_Chapter_Name]`

## Steps

1. **Discover section links**
   Navigate to the chapter TOC URL with Playwright. Read the page's sidebar/
   nested TOC tree and collect every sub-page link that belongs to this
   chapter (not sibling chapters). Record each link's display title and its
   position in the chapter (e.g. "12.3: Observing Black Holes").

2. **For each section link, extract the source HTML**
   - Navigate to the section page.
   - Open the page editor (the same control used in the earlier recon step).
   - Switch to Source/Code view.
   - Copy the raw HTML exactly as shown — do not clean, reformat, or
     summarize it.
   - Close/exit the editor without saving.

3. **Archive figure images (without touching the HTML)**
   - After capturing a section's raw HTML, scan it for every `<img>` tag
     and record its `src` (and, if present, any `data-*` lazy-load source
     attribute — check a real captured section first to see which one
     LibreText actually uses; don't assume).
   - **Do not rewrite the `src` in the saved HTML file.** The saved section
     HTML must keep pointing at the original LibreTexts image URL exactly
     as exported — the local image copy is a backup, not a replacement.
   - For each distinct image URL in the section, fetch the image bytes
     using the same authenticated Playwright browser session (so it works
     even if the image host requires the login session), and save it to
     `chapters/<NN>-<Chapter-Title-Slug>/images/<NN.SS>-fig<N>-<original-filename>`,
     where `<N>` is the image's order of appearance in that section.
   - If the same image URL appears in more than one section, download it
     once and reuse the local file for the manifest entries below rather
     than fetching it twice.
   - Append one row per image to `chapters/<NN>-<Chapter-Title-Slug>/images/manifest.csv`
     with columns: `local_filename, original_src_url, section, alt_text`.
     Create the manifest file with a header row if it doesn't exist yet.
     This is a plain provenance record, not a replacement for your formal
     attribution log — it just saves you from having to re-find each
     image's source URL later.

4. **Determine the file path**
   - Chapter folder: `chapters/<NN>-<Chapter-Title-Slug>/`
     (NN = two-digit chapter number from the TOC page; slug = title with
     spaces replaced by hyphens, special characters stripped)
   - Section file: `<NN>.<SS>-<Section-Title-Slug>.html`
     (SS = two-digit section number)
   - Example: `chapters/12-Black-Holes/12.03-Observing-Black-Holes.html`
   - If a chapter or section number can't be determined cleanly from the
     page, ask the user rather than guessing.

5. **Write the files**
   Create directories as needed. Write each section's raw HTML to its file.
   Do not overwrite an existing file silently — if the file already exists,
   report the conflict and ask whether to overwrite. If all of the chapter content exists, ask if the chapter should be skipped.

6. **Delete redundant files**
  If playright has left a lot of files, such as copies of the images, or copies of the html, in `.playwright-mcp/`, then delete all of the duplicate files in the playwright folder. Do **not** delete any html or image files in the chapters directory or subdirectory.

7. **Report back**
   After the run, list every file written (path only), any sections that
   failed to extract and why, and any chapter/section numbering the tool
   had to guess at.

## Notes
- If the editor's Source-view control can't be found on a given page (site
  layout can vary slightly), stop on that page, ask the user for the click
  path once, and this skill file should be updated with what worked.
- This tool copies all HTML from the page, including figures.