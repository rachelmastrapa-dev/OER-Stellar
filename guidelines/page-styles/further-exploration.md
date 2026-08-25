# Style for Further Exploration

## Further Exploration Text Guidelines  - User instructions, not needed by Claude/AI
- Contextualize links in text - explain where the links are going and what the student will find there.
- Follow accessibility guidelines for selecting link text.

# HTML Format

Maintain class attribute tags if present. e.g. `class="lt-phys-64811"`

For a single statement:

<section class="box-note">
<h5 class="box-legend"><span class="lt-icon-default">Further Exploration</span></h5>

<p>Statement with link.</p>

</section>

For multiple statements, format into unnumbered table:

<section class="box-note">
<h5 class="box-legend"><span class="lt-icon-default">Further Exploration</span></h5>

<ul>
    <li>Statement with link 1.</li>
    <li>Statement with link 2.</li>
</ul>
</section>

All links should have this format:

<a href="URL" target="_blank">Link Text</a>

# Example

<section class="box-note">
<h5 class="box-legend"><span class="lt-icon-default">Further Exploration</span></h5>

<ul>
    <li>Watch <a href="https://www.youtube.com/watch?v=dlCRSl3vmHw" target="_blank">What is Spaghettification?</a> with Neil deGrasse Tyson for a brief explanation of how extreme gravity near a black hole can stretch matter into a long, thin shape. This video provides a helpful introduction to the concept before moving into more detailed discussion.</li>
    <li class="lt-phys-64811"><a href="https://youtu.be/kOEDG3j1bjs?si=uiUlf9vxe55JytLh" target="_blank" title="Black Holes 101">Black Holes 101</a> by National Geographic introduces the basic science of black holes, including how they form and why their gravity is so strong.</li>
</ul>
</section>