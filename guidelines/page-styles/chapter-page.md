# Style for Chapter Page

## Page Settings - here for completeness, not needed by Claude/AI
- Guide Listing Display: Single (Topic Hierarchy)
- Article Type: Chapter

## Introduction [Heading 2] – this is the home page
- Chapter Summary  - make sure you can see it in the page settings - here for completeness, not needed by Claude/AI
- Brief Introduction [Normal-aka Default]

## Learning Objectives
- Use Boxes -> for Learning Objectives
- At least 2, <11
- Start with verb from Bloom's Knowledge level, or similar - Define, Identify, Describe, Recognize, Tell, Explain, Recite, Memorize, Illustrate, Quote, State, Match, Select, Examine, Locate, Enumerate, Record, List, Label

## DO NOT DELETE: {{template.ShowOrg()}} - generates table of contents

## Chapter Thumbnail Image
- Chapter Image Thumbnail is in Page Settings 
- put image caption and attribution in text at bottom of page
- No alt text option available
- Use small images for thumbnail, so that you can see the page summary – 512 px works

### Chapter Thumbnail attribution Format

**Thumbnail**: Caption. (License[LicenseLink]; Author[AuthorLink] via Source[ImageLink].)

# HTML Example
<h2>Introduction</h2>

<p>Chapter introduction text.</p>

<section class="box-objectives">
<h5 class="box-legend"><span class="lt-icon-default">Learning Objectives</span></h5>

<ul>
    <li>Objective 1</li>
    <li>Objective 2</li>
    <li>Objective 3</li>
</ul>
</section>

<p>{{template.ShowOrg()}}</p>

<p><strong>Thumbnail</strong>: Figure caption text. (<a href="LicenseLink" target="_blank" title="License">Public Domain</a>; <a href="AuthorLink" target="_blank" title="Author">Author</a> via <a href="ImageLink" target="_blank" title="Source">Source</a>)</p>
