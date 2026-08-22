# Style for Chapter Page

## File Name
Chapter page file name is usually in the format of `<NN>.00-Introduction.html` where `<NN>` is the chapter number.

## Page Settings - Libretext instructions, not needed by Claude/AI
- Guide Listing Display: Single (Topic Hierarchy)
- Article Type: Chapter

## Introduction [Heading 2] – this is the home page
- Chapter Summary  - make sure you can see it in the page settings - Libretext instructions, not needed by Claude/AI
- Brief Introduction [Normal-aka Default]

## Learning Objectives
- Use Boxes -> for Learning Objectives
- At least 2, < 11
- Start with verb from Bloom's Knowledge level, or similar - Define, Identify, Describe, Recognize, Tell, Explain, Recite, Memorize, Illustrate, Quote, State, Match, Select, Examine, Locate, Enumerate, Record, List, Label, etc
- Keep objectives brief and specific

## DO NOT DELETE: {{template.ShowOrg()}} - generates table of contents

## Chapter Thumbnail Image 
- Chapter Image Thumbnail is in Page Settings - Libretext instructions, not needed by Claude/AI
- put image caption and attribution in text at bottom of page
- No alt text option available
- Use small images for thumbnail, so that you can see the page summary – 512 px works - Libretext instructions, not needed by Claude/AI

### Chapter Thumbnail attribution Format

**Thumbnail**: Caption. (License[LicenseLink]; Author[AuthorLink] via Source[ImageLink].)

# HTML Format
<h2>Introduction</h2>

<p>Chapter introduction text.</p>

<section class="box-objectives">
<h5 class="box-legend"><span class="lt-icon-default">Learning Objectives</span></h5>

<ul>
    <li>Objective1</li>
    <li>Objective2</li>
    <li>Objective3</li>
</ul>
</section>

<p>{{template.ShowOrg()}}</p>

<p><strong>Thumbnail</strong>: Figure caption text. (<a href="LicenseLink" target="_blank" title="License">Public Domain</a>; <a href="AuthorLink" target="_blank" title="Author">Author</a> via <a href="ImageLink" target="_blank" title="Source">Source</a>)</p>

# Example
<h2>Introduction</h2>

<p>In this chapter, we will discuss the origin and properties of black holes and how they affect spacetime. We will also review how astronomers can observe an object that does not allow light to escape. Finally, we will introduce a new type of observatory that searches for gravitational waves.</p>

<section class="box-objectives">
<h5 class="box-legend"><span class="lt-icon-default">Learning Objectives</span></h5>

<ul>
    <li class="lt-phys-64811">Describe the event horizon surrounding a black hole</li>
    <li class="lt-phys-64811">Explain how a black hole warps spacetime and give examples of how the effect can be observed</li>
    <li class="lt-phys-64811">Describe how the concept of a singularity disagrees with our current understanding of the behavior of matter</li>
    <li class="lt-phys-64812">Describe what to look for when seeking and confirming the presence of a stellar black hole</li>
    <li class="lt-phys-64812">Differentiate between stellar black holes and the black holes in the centers of galaxies</li>
    <li class="lt-phys-64813">Describe what a gravitational wave is, what can produce it, and how fast it propagates</li>
    <li class="lt-phys-64813">Describe the basic mechanisms used to detect gravitational waves</li>
</ul>
</section>

<p>{{template.ShowOrg()}}</p>

<p><strong>Thumbnail</strong>: In this illustration, the black hole named Cygnus X-1, which formed when a large star collapsed, is pulling matter from the blue star beside it. (<a href="https://en.wikipedia.org/wiki/Public_domain" target="_blank" title="Public Domain">Public Domain</a>; <a href="https://www.nasa.gov/" target="_blank" title="NASA">IMAGE: NASA, CXC, Melissa Weiss (CXC)</a> via <a href="https://commons.wikimedia.org/wiki/File:Black_hole_Cygnus_X-1.jpg" target="_blank" title="Wikimedia Commons">Wikimedia Commons</a>)</p>

