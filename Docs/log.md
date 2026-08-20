# Editing Log for ASTR 10

Note - oldest entry at bottom of page

## Progress
ASTR 10 17 Chapters + Appendices - remove?

Current Chapters Done  9
astronomical instruments, stellar spectra, star formation, aging stars, stellar finale, black holes, the milky way, galaxies

## Tasks
1. Review all completed science and societies and mark as complete in project tracking. - asap - once AI system is working
2. delete figure in dark constellations - can't find license - waiting to hear from caitlin
3. figure out how Jyothsna can help
4. On all main chapter pages make first H2 Introduction
5. Milky Way Galaxy
6. Search and replace Alternative with Accessible for all finished chapters
7. se the agent to format  astronomy toolkit - get the sections remixed properly so that I can summarize and reference them for other chapters.
8. earth - https://eng.libretexts.org/Courses/H...Physical_World
9. go through my presentation slides and include material in textbook to ASTR 4
10. move angulat momentum into solar system formation and seasons to the earth.
11. use the search string site:eng.libretexts.org geology tosses up a bunch of stuff.
12. record descriptions for images
13. figure descriptions - also include detailed credit?
14. use AI to create summaries for each page, and read over, put in main part and in window - do I need page summaries?
15. revisit  main text around figures and captions and use the format image (a), (capitalize in headers)
## Future?
- Create links between chapters
- record descriptions of figures?
- Optional 
    - Scientist Appendices - Make accessible, edit, etc. and link to relevant sections. 
## Procedure
- Whole Chapter
- Format HTML
- HTML Review
- Format Figures
- Final Edit
- Format Key Terms
- Edit Main Chapter Page
- Final Checks
## 8/20/26

### Pinned
- Whole Chapter Introduction to Astronomy
- Do as much of Intro to Astro as humanly possible

Had a meeting with Shagun, Timeline slightly moved up. Need to improve tools to streamline, will be getting less time from Jyothsna.

Switiching to full cloud agent. Here are instructions from Claude

This is a good instinct to sort out before you're deep in it — the structure you set up now will save you a lot of pain later. Here's how I'd think about it.

## The core problem you're solving

I don't have memory across separate conversations (unless you're using a feature like Projects, more on that below), and any single conversation has a finite context window. So "keep the same context for the entire project" really means: **you need an external, versioned source of truth that gets fed back to me at the start of each session** — not a single infinite chat.

## Recommended structure

**1. A living project spec (the anchor doc)**
One markdown file — `PROJECT.md` or similar — that always reflects current reality: goals, constraints, key decisions made (and why), current status, and what's next. This is what you paste in or point me to at the start of any new session. Treat it like a README that's always up to date, not a log.

**2. Session logs (the provenance trail)**
A new dated file per work session — `sessions/2026-08-20-session01.md` — with a consistent template, e.g.:
- Goal for this session
- What Claude produced/proposed
- What you decided, edited, rejected, or wrote yourself
- Open questions carried to next session

This is your Claude-vs-you record. Keep the attribution granular *in the log*, not scattered as comments in code/docs — much easier to audit later.

**3. Decision records for anything consequential**
Lightweight ADR (Architecture/decision record) style — one file per significant decision, numbered, with the options considered and why one was chosen. Prevents re-litigating the same choice three months in, and makes it obvious whose call it was.

**4. Git as the actual backbone**
- Commit after each session, not each message.
- Use commit trailers to mark authorship, e.g. `Assisted-by: Claude` on commits where I generated most of the content, plain commits where you wrote it. This gives you `git log` as a queryable provenance record for free.
- Branch per step/phase if steps are substantial; merge with a short summary of what changed and who drove it.

**5. One file per "domain," not one giant doc**
Split by concern (architecture, data model, open-questions, glossary) rather than one sprawling doc — easier for both of us to load only what's relevant to a given step instead of re-parsing everything each time.

## How to actually run sessions with me

- Start each session by pasting (or uploading) `PROJECT.md` plus the relevant piece of state — not the whole history.
- End each session by asking me to draft the session log entry and any updates to `PROJECT.md` — that's the handoff artifact you commit.
- If you're on claude.ai, **Projects** can hold your `PROJECT.md` and key docs as persistent project knowledge, so you don't have to re-paste them every time — worth setting up if you haven't.
- If part of this involves actual code, **Claude Code** works directly in your git repo, sees `git log`/`git diff`, and can commit with proper attribution itself — genuinely useful for the "who did what" tracking since the commit history becomes the audit trail automatically.

One thing worth pinning down before we go further:

### Finished
## 8/19/26
- Finish Evolution of Galaxies
- Start Next Chapter - Introduction to Astronomy?
Dump astronomy toolkit?  Do simple versions of Intro to Astronomy and Night Sky

### Pinned
- Whole Chapter Introduction to Astronomy

### Finished
- Final Edit The Structure of the Universe
- Format Key Terms Evolution of Galaxies
- Edit Main Chapter Page Evolution of Galaxies
- Final Check Evolution of Galaxies
- Deleted astronomy toolkit - copied in here, but lost image files.
- Cleaned out Introduction to Astronomy and Night Sky and re-transcluded from Openstax
## 8/18/26
- Finish Evolution of Galaxies
Libretext is being slow. reboot?
### Pinned
- Final Edit The Challenge of Dark Matter

### Finished
- Minor fixes to Format Figure- figure indices and auto-confirmation.
- Process Art and Astronomy
- Final Edit Observation of Distant Galaxies
- Final Edit Mergers and Active Galaxies
- Final Edit The Challenge of Dark Matter
## 8/17/26
- Finish Evolution of Galaxies
### Pinned
- Process Art and Astronomy/Final Edit Evolution of galaxies

### Finished
- HTML Review Evolution of Galaxies
- Format Figures Observations of Distant Galaxies
- Copied in astronomy toolkit and edited numbers, focusing on main topics
- Format Figures Mergers and Active Galaxies
- Format Figures The Distribution of Galaxies
- Format Figures The Challenge of Dark Matter
- Format Figures The Strucutre if the Universe
## 8/16/26
- Finish galaxies
- start on evolution of galaxies
- work with agent and astronomy toolkit or break up astro figs into skills
### Pinned
- HTML Review Observations of Distant Galaxies

### Finished
- Final Edit of The Discovery of Galaxies
- Final Edit of Types of Galaxies
- Final Edit of Properties of Galaxies
- Final Edit of The Extragalactic Distance Scale
- Final Edit of The Expanding Universe
- Format Key Terms Galaxies and copy in links
- Galaxies - main page
- Galaxies - final check
- Whole Chapter - Evolution of Galaxies
- Format HTML Observations of Distant Galaxies
- Format HTML Mergers and Active Galaxies
- Format HTML The Distribution of Galaxies
- Format HTML The Challenge of Dark Matter
- Format HTML The Structure of the Universe
## 8/15/26
- Format HTML of Galaxies and next steps
- Buy agent today??
- Astronomy Toolkit Figures??

Skipping Astronomy Archtecture in Galaxes because not done.
### Pinned
- Final Edit of Galaxies

### Finished
- Format HTML + HTML Review Discovery of Galaxies
- Format HTML Types of Galaxies
- Format HTML Properties of Galaxies
- Format HTML Extragalactic distance scale
- Format HTML The Exapnding Universe
- HTML Review Types of Galaxies
- HTML Review Properties of Galaxies
- HTML Review The Extragalactic Distance Scale
- HTML Review The Expanding Universe
- Format Figure Discovery of Galaxies
- Format Figure Types of Galaxies
- astro-figs fix - last attribution, increment figure numbers
- Format Figure Properties of Galaxies
- Format Figure The Extragalactic Distance Scale
- Format Figure The Expanding Universe

## 8/14/26
- Final edit of text for Milky Way, start Galaxies.
- Have started to set up files for Solar System. start with astronomy toolkit  Focusing on this for now.  
- Buy agent soon? 
- Note: use instructions format for Claude instructions.

### Pinned
- Discovery of Galaxies - log figure att

### Finished
- Final Edit of Observing Our Galaxy
- Final Edit of Spiral Structure
- Final Edit of Mass of the Milky Way
- final edit all chapters, key terms
- Main Page, saved in Conductor
- Completed instructions
- Format HTML Discovery of Galaxies
- Copied Astronomy Toolkit

## 8/13/26
Finished format text & manual on all of Milky way galaxy, now Working on graphs in Milky Way Galaxy

## 8/12/26
Finished Black Holes 

Meeting with Jythsna

8/12 meeting with Jyothsna

Tell her that I am done with Black Holes - done 

Next is Milky Way Galaxy, Galaxies, Evolution of Galaxies  #3 Stars and Light

Very behind - sorry = but AI tools working well

Questions

You mentioned some images in chapter (4 4.2.1,4.2.5) were missing.  Are they working? Jyothsna is checking

I've tried running the Libretext accessibility tool. The main error I get is that links should not open in another tab without a warning. I think I remember Shagun telling me to always make them open in a new tab.  I just want to confirm which is correct.  - Shagun  - ignore accessibility do not change  

On the accessible descriptions page, should I remove figure numbers so that they can be remixed more. They will have the figure title so they can be found.  I could also anchor the figures and make a link back to them from the description.   do not change

Shagun - says timeline needs to be updated - finish tracking and -  

follow AD and WCAG  - jyothsna will check - 

Use this document - https://foothilldeanza-my.sharepoint...fxs90?e=UJJbBg




## 8/11/26
Very behind schedule, but working on gravitational waves ib black holes.

Almost done with black holes - key terms and first page.  

8/10/26
Finally got astro figs built - next step, load into claude and ask if it has questions.  Answerrd questions and updated. processing first figures.

Finished Properties of Black Holes, working on observing - very short.

8/9/26
So I am supposed to have 5 more chapters done by Wednesday.  I don't think that is going to happen.  I just had an idea that I should get all 5 to a certain point, but that is not helpful to Joythsna since she has to review them. 

So, focus on Black Holes.  Get it ready for astro-figs and push it through to done!

The next 4 are milky way, galaxies, evolution of galaxies. and Stars and Light

8/8/26
A lot of jumping around today. Working on some of astro-figs, but realized that I needed to compress down my playlab AI and put them all in one - format-html  going to go back and rescan Black Holes and Milky Way Galaxy, but first need to confirm the process in ASTRO 10 editing instruction - make sure everything is in there. 

Streamlined editing process to just one pass through playlab + making key terms, + claude astro-figs. 

Made progress astro-figs, almost ready for testing.  Going to try to push more through format html before bed. 

I did have a moment where libretext shut down, that reminded me to move everything out of here.  

8/7/26
Will continue to work on astro-figs, but I am starting on next chapter and will be running clean text on the background - following ASTRO 10 editing instructions

starting with the milky way galaxy finished this focusing on astro-figs for the rest of the day. 

Morning - implement rearranging text.  combine with the highlighting??? - tell it specifically not to change anything in figures?

8/6/26
Making a new repository called astro_figs to handle figure processing for libretext: creating a repository

Installed git for windows   did all the work in fit-hub scratch - italics means done.

8/5/26
Meeting with Jysothna today.  Report:

Caught up with 5 chapter deadline a little late due to Cal OER meeting. Am implementing things I learned from the meeting and already speeding up the chapter review process.  So far, cleaning html and accessible descriptions. 

Reviewing all of her suggestions  - 

Waiting on guidance for Openstax figures. - keep 

Make changes to notes - first H2 in main chapter page is Introduction.  Last step is notify Jyothsna when a chapter is done. 

Starting with making all the changes from Jyothsna. = made all changes.



8/4/26
Need to relink accessible descriptions in Stellar Finale! - finishing accessible descriptiong, then re-linking, finally completely finished Stellar Finale. 

Next is re-doing editing procedure.  Started building in libretext, but changed to a google doc because of html problems. 

I actually should just build it Playlab and then copy it to the doc.

Cleaned all text in Black Holes. I still have to develop the rest of the editing steps. 

8/3/26
Creating a program in Claude for accessible descriptions. 

Purpose & context

Create accessible descriptions for figures.

Figures are for an Open Educational Resource (OER) textbook about astronomy. 

Accessible descriptions will be linked in the figure caption for students that need a more detailed description of a figure. This may be for students that are visually impaired, but also for students with other learning support needs, or just for students that would like a more detailed description.

Requested by editor of textbook: Rachel

Procedure

Rachel will upload a figure, or a link to a figure, the figure number and the figure title.
(Optional) Rachel will upload any metadata along with the figure such as a draft of the accessible description for use in the final accessible description. The text may be in plan text or html
Claude will return an accessible description in html based on the format described below. 
Rachel may return her edited description for training purposes. 
When Rachel requests a report, generate a list of all accessible descriptions generated since the last report and generate an AI citation in APA format. 
Accessible Descriptions

An accessible description is significantly longer than alt-text.  The content is less about the context of the image and more about the components of the figure.

When generating accessible descriptions, Claude should follow these guidelines:

The first line is the figure number and title.
The second line is a brief description of the figure.
Always indicate the type of figure, including image, chart, illustration, map, etc. 
if it is an image include the telescope or instrument it was acquired by and the wavelength, if available.
If it is a multi-panel figure include each panel and the figure type.
Supporting text:
Always use any supporting text, if provided. Generate additional description if obvious components are missing.
If not, generate a description based on the image.
The format of the rest of the description depends strongly on the type of image. In general, it should be broken up into separate sections using sub-headers. If the description is lengthy, break it into brief statements in a bulleted list, describing some components using nested bullet.  See examples below.
Describe all key labeled components and visual structures in the image. This includes the name of the astronomical object or objects and a physical description of the object or objects.
Account for multi-panel images by addressing each panel distinctly
If the are labeled with a letter or number, refer to them as Image (a), or Chart 1 depending on the numbering system.
Include a reference to the location of the panels relative to each other, such as to the right, or at the bottom.
Only include image credit if submitted by Rachel
HTML Format
<h2>Figure FigureNumber FigureTitle</h2>

<p>Brief Description.</p>

<h3>Subsection</h3>

<ul>
<li>Description.</li>
<li>Description</li>
<li>Description</li>
</ul>

<h3>Subsection</h3>

<ul>
<li>Description</li>
<li>Description</li>
<li>Description</li>
<li>Description Component
<ul>
<li>Description</li>
<li>Description</li>
<li>Description</li>
</li>
</ul>

Example 1


Supporting Text:

Evolutionary Tracks of Stars of Different Masses. In this plot the vertical axis is labeled “Luminosity (LSun)” and goes from 10-2 at the bottom to over 104 at the top. The horizontal axis is labeled “Surface Temperature (K)” and goes from 25,000 on the left to 4,000 on the right. The “Zero-age main sequence” is drawn as a diagonal red line beginning above L = 104 at the upper left of the image down to T ~ 4000 at the lower right. Six evolutionary tracks are drawn. Beginning at the top, a star of “15 solar masses” is plotted. It leaves the main sequence above L ~ 104 and T ~ 25,000. The track moves rightward across the top of the plot. The star maintains a relatively constant luminosity, but its surface temperature decreases with time. At “1.01 × 107” years its temperature is about 20,000 K. At “1.11 × 107” years it has fallen to about 15,000 K. At “1.19 × 107” years T is about 9000 K, and the track ends at “1.2 × 107” years near 4000 K. Next, a star of “5 solar masses” is plotted beginning near L ~ 103, where it leaves the main sequence. The star maintains a relatively constant luminosity, but its surface temperature decreases with time. At “6.55 × 107” years its temperature is about 12,000 K. but its surface temperature decreases with time. At “2.39 × 107” years it has fallen to about 5000 K. Then the luminosity rises slightly to the final plotted point at “7.02 × 107” years near 4000 K. Next, a star of “3 solar masses” leaves the main sequence near L = 102 and 15,000 K. After “2.21 × 108” years its temperature has fallen to near 11,000 K. After “2.46 × 108” years its temperature has dropped to near 6000 K. Then, its luminosity increases by about a factor of ten where its curve ends at “2.51 × 107” years and 5000 K. Next, a star of “1.5 solar masses” leaves the main sequence near L = 30 and 9000 K. After “1.55 × 109” years its temperature has fallen to near 7500 K. After “2.09 × 109” years, its temperature has dropped to near 5000 K. Then, its luminosity increases by about a factor of one hundred where its curve ends at “2.39 × 109” years and 4000 K. Next, a star of “1 solar mass” leaves the main sequence at L = 1 and 5700 K. After “7 × 109” years its temperature is nearly the same, but its luminosity has increased slightly. After “10.4 × 109” years, its temperature has dropped to near 5000 K, and its luminosity has increased about 20 times. Then, its luminosity steadily increases to where its curve ends at “11.4 × 109” years, L ~ 103 and T ~ 4000 K. Finally, a “0.5 solar mass” star is partially plotted. Its curve begins at L ~ 10-1 near T ~ 5000. Its curve is a short arrow pointing upward as its evolutionary timescale is too great for this diagram.

Description:

<h2>Figure 12.1.5 Stellar Mass and Evolution</h2>

<p>AN H-R Diagram with model evolutionary tracks of stars with a range of masses.</p>

<h3>Chart Elements</h3>

<ul>
<li>The vertical axis is labeled Luminosity (L<sub>Sun</sub>) and goes from 10<sup>-2</sup> at the bottom to over 10<sup>4</sup> at the top with increments of 10<sup>2</sup>.</li>
<li>The horizontal axis is labeled Surface Temperature (K) and goes from 25,000 on the left to 4,000 on the right.</li>
<li>The horizontal axis is non-linear. There are two increments of equal size, the first is from 25,000 to 10,000 and the second is from 10,000 to 4000.</li>
<li>The Zero-age main sequence is drawn as a diagonal red line beginning above L = 10<sup>4</sup> at the upper left of the image down to T ~ 4000 at the lower right.</li>
</ul>

<h3>Evolutionary Tracks</h3>

<ul>
<li>Six total</li>
<li>Beginning at the top</li>
<li>All tracks have points marking the age of the star.</li>
<li>15 solar masses
<ul>
<li>It leaves the main sequence above L ~ 3 x 10<sup>4</sup> and T ~ 25,000.</li>
<li>The track moves mostly rightward across the top of the plot.</li>
<li>Overall, the star maintains a relatively constant luminosity, but its surface temperature decreases with time.</li>
<li>At 1.01 × 10<sup>7</sup> years its temperature is about 20,000 K.</li>
<li>As the track leaves the last point, it increases in temperature to just about 23,000 K and then makes a sharp turn to the right to meet the next point </li>
<li>At 1.11 × 10<sup>7</sup> years it has decreased in temperature and moved right on the chart to about 15,000 K.</li>
<li>At 1.19 × 10<sup>7</sup> years T is about 9000 K </li>
<li>The track ends at 1.2 × 10<sup>7</sup> years near 4000 K.</li>
</ul>
</li>
<li>5 solar masses
<ul>
<li>Begins near L ~ 10<sup>3</sup>, where it leaves the main sequence.</li>
<li>Overall, the star maintains a relatively constant luminosity, and its surface temperature decreases with time.</li>
<li>At 6.55 × 10<sup>7</sup> years its temperature is about 15,000 K. The star's luminosity has increased to roughly 3 x 10<sup>3</sup>.</li>
<li>There is a very small increase in temperature after the last time point.</li>
<li>At 6.98 x 10<sup>7</sup> years the surface temperature is about 5000 K.</li>
<li>The track ends at 7.02 x 10<sup>7</sup> years at a temperature of about 4500 K. The luminosity has increased to roughly 4 x 10<sup>3</sup>.</li>
</ul>
</li>
<li>3 solar masses
<ul>
<li>Leaves the main sequence near L ~ 10<sup>2</sup></li>
<li>Overall, the star is relatively constant luminosity until the end of last time point. The surface decreases the most during the first two sections of the track and then decreases a small amount at the end of the track. During the same section, the luminosity increases.</li>
<li>At 2.21 × 10<sup>8</sup> years its temperature is about 12,000 K. The star's luminosity has increased to roughly 2 x 10<sup>2</sup>.</li>
<li>There is a very small increase in temperature after the last time point.</li>
<li>At 2.46 x 10<sup>8</sup> years the surface temperature is about 5500 K. The luminosity has decreased back to 10<sup>2</sup>.</li>
<li>The track ends at 2.51 x 10<sup>8</sup> years at a temperature of about 4500 K. The luminosity has increased to roughly 6 x 10<sup>2</sup>.</li>
</ul>
</li>
<li>1.5 solar masses
<ul>
<li>Leaves the main sequence near L ~ 10.</li>
<li>Overall, the star decreases in temperature with time. At first the luminosity is mostly constant, but it increases by a large amount in the last section of the track.</li>
<li>At 1.55 × 10<sup>9</sup> years its temperature is about 7000 K. The star's luminosity has increased to roughly 30.</li>
<li>There is a very small increase in temperature after the last time point.</li>
<li>At 2.09 × 10<sup>9</sup> years its temperature is about 6000 K. The star's luminosity stays near 30.</li>
<li>At 2.39 × 10<sup>9</sup> years it's temperatures has decreased to about 5000 K. Its luminosity increases to 3 x 10<sup>2</sup>.</li>
</ul>
</li>
<li>1 solar mass
<ul>
<li>&nbsp;Leaves the main sequence at L = 1 and 5700 K.</li>
<li>After 7 × 10<sup>9</sup> years its temperature is nearly the same, but its luminosity has increased slightly.</li>
<li>After 10.4 × 10<sup>9</sup> years, its temperature has dropped to near 5000 K, and its luminosity has increased to 10.</li>
<li>Its luminosity steadily increases to where the curve ends at 11.4 × 10<sup>9</sup> years, L ~ 10<sup>3</sup> and T ~ 4000 K.</li>
</ul>
</li>
<li>0.5 solar mass
<ul>
<li>Begins at L ~ 10-1 near T ~ 5000.</li>
<li>Its curve is a short arrow pointing upward as its evolutionary timescale is too large for this diagram.</li>
</ul>
</li>
</ul>



Supporting Text:Two Images of the Globular Cluster Omega Centauri. Panel (a), on the left, shows a ground-based image of Omega Centauri as a large sphere of thousands of stars that is so dense that the central region appears as an indistinct patch of light. Panel (b), on the right, shows a high-resolution H S T image of the central region, showing dozens of bright red and blue stars amidst a background of thousands of fainter yellow stars.

<h2>Figure 12.2.1 Omega Centauri</h2>

<p>Two Images of the Globular Cluster Omega Centauri.</p>

<h3>Image (a)</h3>

<ul>
<li>On the left</li>
<li>Ground-based image of Omega Centauri as a large sphere of thousands of stars that is so dense that the central region appears as an indistinct patch of light.</li>
<li>Credit: NASA, ESA and the Hubble Heritage Team (STScI/AURA)</li>
</ul>

<h3>Image (b)</h3>

<ul>
<li>On the right</li>
<li>A high-resolution Hubble Space Telescope image of the central region, showing dozens of bright red and blue stars amidst a background of thousands of fainter yellow stars.</li>
<li>Credit: NASA, ESA, and the Hubble SM4 ERO Team</li>
</ul>

8/2/26
Working on final edit of Neutron Stars and Pulsars.

The Libretext accessibility checker says not to open to new tabs without a warning and a quick search confirms.  , but I am pretty sure Shagun told me to always open in a new tab/   Jyothsna has not comented either.

8/1/26
Geeting overwhelmed by implementing AI.  For now, I will focus on just getting the chapter done, then implementing work in libretext, then piecemeal shifting to claude code?

7/31/26
Reviewing editing process and rebuilding chatbot to help more.

Break into multiple phases. Need to make sure that overall page structure is correct, figures in order. info in the correct section.

clean - remove italics, etc. replace all figure and table numbers with default Latex number, highlight excess material for deletion?

figures - move captions to a paragraph with figure number adn highlight, cut large alt text, move to paragraph and labels as accessible description and highlight. replace alt text with temp placeholder, for non openstax figures - put in standard format caption. Label openstax figures before - then put in figure attribution. Create titles before and have it make list of accessible descriptions - put text with it? and link?

edit - re-arrange paragraphs into logical order - but do not change content!!!, highlight idioms, anything hard to translate, etc. identify key terms! - identify key terms!, check for material that is not needed

review the rest of the editing process and see if I can compress and make mostly AI

Current instructions in formatter

Never remove class attributes from header or paragraph tags.
Never remove any tags from key terms. Example do not change anything in something that looks like <strong><a href="/Workbench/De_Anza_-_ASTR10/13%3A_Stellar_Finale/13.07%3A_Key_Terms#nova" target="_blank" title="nova">nova</a></strong>
Remove italics
Remove bold except when they are around a link to the key terms page
Remove term
Remove $nbsp


I am also making a diff function so I can compare text. 

Playlab still has problems with the figure numbers \(  puttin in $$ instead - changing to have it be XX and I will do a finf and replace.  

When it edits things in the alt text it breaks the figures.  I think I will remov

Let me rearrange things a little:



Break into multiple phases. Need to make sure that overall page structure is correct, figures in order. info in the correct section.

clean - remove italics, etc. replace all figure and table numbers with default Latex number, highlight excess material for deletion?

figures - move captions to a paragraph with figure number adn highlight, cut large alt text, move to paragraph and labels as accessible description and highlight. replace alt text with temp placeholder, for non openstax figures - put in standard format caption. Label openstax figures before - then put in figure attribution. Create titles before and have it make list of accessible descriptions - put text with it? and link?

edit - re-arrange paragraphs into logical order - but do not change content!!!, highlight idioms, anything hard to translate, etc. identify key terms! - identify key terms!, check for material that is not needed

review the rest of the editing process and see if I can compress and make mostly AI

Moving the work to Preliminary Clean page.

Pausing this until I am done with stell finale. But trying the section only draft?

For evolution of Massive stars I am running the clean html on it. then going section by section.

I ran into some issues with the chatbot getting too bloated, and retaining memory of things I did not want it to do.  I broke it into three chatbots.  Wasted a lot of time.  :( Although it will be a huge timesaver if I can get it running.  

7/30/26
Back to equations.  One last try using quote marks in the chatbot? 

finished equartion - quote marks do not work - so have to create delimiters 

Moving to prelim clean on black holes, because multi-tasking. Black Holes/Black holes prelim

I have done some stuff with the Black Hole Chapter and I need to come back and revist this when I can focus, so skipping to Milky Way. 

Going to make a chatbot function that will clean the bad stuff out of the html, strong, italics, term, nbsp. replace all figure and table numbers with default Latex number highlight idioms or ablist language?

Forgot - went back and finished key terms in Stellar Finale. 

Done with meeting so starting final text run of Stellar finale - hope to be able to focus

Creating a clean html function, where it removes all of the above - do not put in the figure and table numbers yet, because I have done those.  I will see if it can highlight idioms, ablist or anti-idea language.  Code for highlighting in red: <span class="mt-bgcolor-c0392b">text</span>

Something wrong with key terms.  Fixing.

Finished final edit of The Death of Low-Mass Stars Next - Evolution of Massive Stars = tomorrow afternoon.  For now, back to Milky Way Galaxy. 

7/29/26
finished prelim on binary systems and almost done with radium girls.  

Updating Playlab chatbot to return references when given a link. pasting in examples of specific types. 

added equations to main formatter, Matty, changes key term links so that it is not a list - annoying.

Learned that I can't get Playlab to display the delimiters I want so I will have to stick with $$ and replace them myself. Still working on equations in Stellar Finale.

7/28/26
prelim Binary Star Systems

got some feedback from jyosyntha and made some changes to my editing instructions and some corrections to Stellar Spectra.

7/27/26
Meeting with Jyosthna. 

time is an issue - accessibility of images most time consuming. 
meetings wed at 9am 

finished prelim of Neutron Stars and Pulsars

7/26/26
Trying to do prelim of supernovae at the hospital. 

finished supernovae.  taking care of the the image for accessible description link - check stellar spectra, star formation - done

remove extra alt-text html markup for all openstax images - check astronomical instruments, stellar spectra, star foramtion. - done

 prelim of pulsars and neutron stars

7/24/26
Finished prelim of Evolution of Massive Stars, moving to Supernovae

7/23/26
Finished Prelim of Death of Low Mass Stars, starting Evolution of Massive stars

Also, met with Shagun, have set due dates August 31 and October 31?

7/22/26
Reassessing how much work is complete # of chapters completed (on my end 0 still need accessibility) - # of chapters that need to be done

Completed - Astronomical Instruments, Stellar Spectra, Star Formation. Aging Stars  4 total

Count once astronomy toolkit, introduction to astronomy, night sky navigation - 3

Solar System 12

Stellar 12

Need to be done - 26

Tiime between now and district opening day.  8 weeks

My chapter rate could be about 2 chapters a week, depedning on complexity 

So probably 16 Chapters by September 16 - one of the textbooks at least.  I might be able to go faster but we will see.  

7/22/26
Prelim clean of The Death of Low-Mass Stars

rearranging order of text- moving nova to binary stars.

7/21/26
prelim clean of science and socity = completed + final edit

chapter-wide final edit. 

Finished Aging Stars!!! Next is Stellar Finale

Starting Prelim clean of The Death of Low-Mass Stars

7/20/26
final text -  Star Clusters - done - moving to clusters on the H-R diagram - done - further evolution of stars. - done

whoops, haven't done prelim clean of science and socity - that is next + final text.

7/17/26
Aging stars prelim clean - further evolution of stars

adding notes on searching for key terms in openstax markup

noticed that the openstax alt text is in the figure html markup - comparing to another figure to make sure I can remove it properly. The openstax version has some span garbage - remove that and you are cool.


Figure \(\PageIndex{1}\): Reflection. The law of reflection states that the angle of reflection equals the angle of incidence. Details in text. (CC BY 4.0; Andrew Park via Introduction to Physics (Park))
Finished prelim clean - moving to final text run for all sections starting with From Main Sequence

Finsided final text - From Main Sequence - next is Star Clusters

7/15/26
Aging stars prelim clean - further evolution of stars

7/14/26
Assessing how much work is complete # of chapters completed (on my end 0 still need accessibility) - # of chapters that need to be done

Completed - Astronomical Instruments, Stellar Spectra, Star Formation.  3 total

Count once astronomy toolkit, introduction to astronomy, night sky navigation - 3

Solar System 12

Stellar 12

Need to be done - 27

Let's get that number a bit higher before Monday.

Aging stars prelim clean - further evolution of stars

7/12/26
continuing prelim clean of - clusters on the HR - finished

7/11/26
Continuing to paste stuff into Aging stars- checking attribution codes - finished remix and delted extra page.

Back to clean - check first section

Almsot done with first section but realized that I had lost the attribution codes when copying a bunch of stuff in. - need to go back and fix that!!!  - done

Back to cleaning first page - logged figures, attributions, etc, finished section main sequence to red giant., finished star clusters.

7/10/26
I am going over the accesible descriptions in astronomical instruments. - done

moving to aging stars. Starting preliminary clean. 

Realized that I had copied in some material from another chapter hear and need to figure out where to put it.  (HR and stellar evolution at the end of the chapter.  Slowly pasting material over - remember that some does not have codes, so need to manually attribute



7/9/26
The plan is to finish up star formation and start on Aging Stars.  Need to pick up the pace.

Completed all final text runs - need to do main page thumbnail and key terms

finished thembnail

putting key terms into main OER formatter, formatted further exploration links for all pages

redo learning outcomes!!!!! -done  make formatter able to batch format - maybe did?

next is final check

going back and putting in simple descriptions for complex figures in Stellar Spectra.  Will come back to them if Ican 

check tasks in todoist - copy here???

7/8/26
Continuiing with figures in stellar origins

The accessible descriptions take a long time - maybe put in a minimum and then come back to them?

Completed up to HR

7/7/26
Updating figures in stellar origins

7/5/26
Continuing final text on stellar origins.

Compled editing text of stellar origins.

7/3/26
Had a little time off due to surgery #3.  Will finish working on science and society and then will just edit the planet formation instead of redoing - for now.

s&s - logging links & other info. finished logging

Starting on evidence of planets - changed name to Evidence of Exoplanets.

Finished prelim clean on Star Formation starting Final Text on Stellar Origins



7/1/26
Having a nightmarish time accessing libretext from hospital wifi.  will try my best. changed name pf H-R and star form.

made the excel spreadsheet for aging stars and added the content for remix that was on this page.  Need to figure out where the go there - left a note.  Updated names in spreadsheet.  Moving link on page.  

I got some responses on my ticket that there had been some library problems.  It seems like it is solved and so far working better.  Yay!

Completed preliminary clean for HR & Star Formation. skipped planet formation, almost done with naming stars - need to enter references and links into spreadsheet.

6/30/26
starting pre text clean on HR and the...

OK - so HR and the evolution is not about stellar evolution past formation, but it is remixed with that material,  The page I am editing belongs in Aging stars and the names of this chapter need to chage  - main chapate to Star Formation.  1st subsection Stellar Origins 2nd H-R diagram and star formation, this page needs to be re-copied in and then kept mostly as-is.

6/29/26
Final format - brown dwarfs. 

Finished Stellar Spectra. 

Starting on Star Formation - preliminary clean. on star formation page.

Finished figures in star formation up to Winds & Jets section - taking a break.

Completed preliminary text clean for star formation section. Next is The H-R and the Study....

6/27/26
At doppler shift in stellar characteristics.

Finished all of the descriptions. Continuing to formatting everything. USing bots in playlab https://www.playlab.ai/login?redirectTo=%2Flogged-in

Finished file format up stellar classifications - next brown dwarfs

6/26/26
Picking up at stellar classification - try to note where I am done, so I can pick back up. 

learned from yesterday - break descriptions into lists, copy text from pages in editing.  (Accessible description .....)

finished final text run of stellar classification, starting brown dwarfs

Brown dwarfs was short, starting final text run for stellar characteristics. 

Libretext is being shitty and keeps loggine me out!!!! and then won't log me back in. Plus, I am already logged in to conductor, so it is just being a dick. Then I try again and it works.  So annoying. 

Part of the way through stellar characteristics.  Taking a break.

6/25/26
All the sections will take time, just get stellar spectra done and move on.

Got to stellar classification.

6/24/26
Got blood drawn today, so focused more on other work.  Taking a look at the "easy"chapters star formation, aging stars, stellar finale, 

6/23/26
Completed Astronomical Instruments, except for one image of light in atmosphere - created a powerpoint, so I can do a bunch of images at once.  Should probably also redo spectrometer. 

Moving on to Stellar Spectra - reviewing chapter editing procedure



6/22/26
Confirming that astronomical instruments is ready to go.

Checking my editing guides, and style files, making sure they are up to date. 







5/22/26

Taking another look at MET 10 to make sure that I have a clear idea of the requirements for the accessible descriptions.

I am moving the style file into Solar System Templates and converting to Libretext. I think I need to redo all of the templates in Solar System Templates – but not now!!!



5/19/26

Back to working on astronomical instruments – working on image descriptions

5/8/26

There aren’t a lot of examples and exercises in the books so didn’t have a lot to fix

Working on captions and alt text



5/7/26

Shagun made some suggestions for changing things.

First thing is to put all the examples back in boxes – starting in astronomical instruments

I have access to MET 10L to see examples of captions and alt-text

Alt-text – what is in the image

Caption – learning objective

Alternative description of the image = detailed description of the image







3/29/26

Finished logging key terms, creating list, anchors and links

Edited the Key terms chatbot to also create the anchors and terms in bold with link.

Finished key terms

It seems like I forgot about the existence of stellar characteristics, so I need to do everything on that section.  Finishing references first.

Editing stellar characteristics.  Went through and fixed figure labels and attributions – did most of the alt -text, but check and check captions.

3/16/26

Continuuing logging data in excel.  Working on key terms



3/9/26

I need to edit Stellar Classification before I can log its infor, because I may get rid of some of the images and text.

3/6/26

Previously made progress through some to types of spectra

Pasted over the work into spectral lines

Starting at the beginning of the chapter and logging all info in the spreadsheet

3/3/26

Working on the excitation levelsof the atom.  Some equations needed

3/1/26

After some technical issues, switched to chrome.  Fingers crossed



2/26/26

Actually, I should focus on the parts that overlap with the toolkit.  Back to re-arranging Light a bit more. And Spectroscopy

So I emptied everything in spectroscopy into the light sections – basically, everything that is not directly astronomy-related – so I left behind a spectrum of the Sun.

Completed parts of the spectroscopy page and am working on spectral lines.  I am working on Light and am in the middle of organizing types of spectra – with a lot of the info copied into scratch

2/25/26

Fixed figure attribution numbering and captions in astronomical instruments ethics of building telescopes.  Oops

Rearranging Stellar Spectra

·         Spectroscopy

o   Reflection/refraction

o   The Visible Spectrum

o   Collected first spectrum of Sun – saw weird lines – what is happening?

o   What happens when light an matter interact – review matter

·         The Atom

o   Nuclear atom

§  Particles

§  Ionization

o   Elements

§  Isotopes

§  The Periodic Table

§  Cosmic Abundances

o   How do light and matter interact on an atomic level?

·         Spectral Lines

o   Atomic Transitions

§  The Bohr Model of Hydrogen

§  Hydrogen’s Energy Levels

§  Ionization and Spectral Lines

§  Identifying Elements

o   Types of Spectra

§  Continuous

§  Emission

§  Absorption

·         Stellar Classification

o   Organizing Spectral Data

o   Temperature and Spectra

o   Spectral Classes

·         Brown Dwarfs

First Organizing the text that I don’t have to change very much

Stellar Classification



2/24/26

Finishing up Astronomical Instruments to send to review

            Formatted links, removed links from main text

            Removed in text citations

            Replaced Mauna Kea with Maunakea

Updating Project Tracking

Made some changes in OER Textbook Formatter - updated attributions

Checked in with Shagun – submitted astronomical instruments-

Moving back to Stellar Spectra

The Atom – writing in astronomy toolkit, then editing down.

Working on final pass through text, alt-text, figure captions

Figure numbers and key terms will be copied over incomplete and filled in Stellar Spectra

Completed the atom up to final text run

Spectral Lines – starting in Astronomy Toolkit – Light

Need to do a lot more organizing of the next three sections – stellar spectra and brown dwarfs seems to be redundant with stellar classification. Move classification first and then have a small section on brown dwarfs – or combine??

2/19/26

Reviewing ethics of building telescopes

2/17/26

Finished figure attributions

Going to chapter summary

Finished and sent to Caitlin

2/15/26

Finished the last pass through on preliminary clean ans starting final text run. Did a lot of removing of italics and idioms already, and changing equations to latex. 

Starting on all definitions – finished all key terms

Checking links – adding links at the end – creating chatbot

Almost done with figure attributions – definitely ready to send to caitlin



2/12/26

Moved all documents to word and storage in FHDA Onedrive and on desktop.  Incomplete but ongoing.

Finished Radio astronomy





2/10/26

Gotten to editing text on Capturing Light



2/9/26

Working on Modern Telescopes



2/8/26

Marking all key terms, links, etc

Finished telescopes



2/5/26

Previously completed logging figures, tables, references

Starting preliminary clean, finished through checking for weird html



Working on Spacecraft

2/2/26

Continuing in astronomical instruments.  

Following this procedure

Created spreadsheet 

Completed Attributions

2/1/26

Starting on Astronomical Instruments

1/30/25

Updating project tracking with new schedule

Working on first page of black hole chapter 

Copying AI stuff into AI log - using AI to format, references, key terms list, math equations



1/29/26

Met with Caitlin - notes are in OER notes in De Anza Drive 

Moved Cosmology to Appendix

Set Toolkit to Chapter 0

Note that I changed chapter numbering making Astronomy Toolkit Chapter 0 

Shagun wants us only to fill out review forms - don't comment in text. 

Accessibility - smaller titles and remove special characters - just change main title to Science and Society, or the title of the Section? 

OER scheduling 

Review Caitlins update - confirm I will do reference formats, move cosmology to appendix? 

Focus on ASTR 10 

Astronomy toolkit – just get basic science organized to link to sections 

12. 13, 14 star form, aging, finale 

Celestial census 



I want to do the easiest chapters first, Black Hole, Galaxies - timing of science and societies? - want to have whole chapter done? - schedule chapters for quarter 

honors classes - have form to fill out - need Mehrdad? 




1/27/26

Reviewed Shagun’s accessibility notes. 

Starting ASTR 10 Black holes chapter for final editing and submission to accessibility.

Will share just one page to double check.  

Creating a final edit and accessibility review process

Final Text Run

Edit text for consistent tone, remove idioms, support IDEA
Remove all italics
Change equations to Latex
Create all term definitions
Check all links
Final Formatting Run

Confirm auto-attributions
Check image alt-text
Check image caption and attribution
Check figure numbers and references.  
Check video attribution and embedding?
Chapter page

Create summary for chapter
Shorten learning objectives list
Check thumbnail caption and attribution


1/4/26

Going over Project Tracking, reviewing Science in Society

1/1/26

Astronomy Toolkit run

Rearrange order of text
Make sure headers are nested properly
Delete any obviously extra text
Still in Numbers in Astronomy



12/30/25

Starting the next run, skipping first three chapters, any other things copied from ASTR4 Solar System, Sun, exoplanets - I was getting ready to do this, but I think I really need to make the toolkit chapter at the very least, because I need to be able to copy in information/summarize, and refer to information in the summary.  

So, going back to astronomy toolkit:

Starting in Astronomy Toolkit - Numbers

Need to move temperature, mass, volume, and density to Numbers - after I log all the info from Physics, too.

Still working on Numbers in astronomy - the web site keeps crashin

Getting a little too much in the weeds with editing. Need to focus on just rearranging full paragraphs, and maybe deleting extra info 

I did note that I may need to edit in html, unless I want a shit ton of $nbsp; is in my text.  Or just edit and then find and replace, but that does not always work.  Oh, wait, chatbot. 

Astronomy Toolkit run

Rearrange order of text
Make sure headers are nested properly
Delete any obviously extra text
The fucking website keeps crashing.  I had copied the text below and I need to refind the original text and copy it in.

The mass of an object is a measure of the amount of matter in it. One way to measure an object’s mass is to measure the force it takes to accelerate the object. It takes much more force to accelerate a car than a bicycle because the car has much more mass. A more common way to determine the mass of an object is to use a balance to compare its mass with a standard mass.

Although weight is related to mass, it is not the same thing. Weight refers to the force that gravity exerts on an object. This force is directly proportional to the mass of the object. The weight of an object changes as the force of gravity changes, but its mass does not. An astronaut’s mass does not change just because she goes to the moon. But her weight on the moon is only one-sixth her earth-bound weight because the moon’s gravity is only one-sixth that of the earth’s. She may feel “weightless” during her trip when she experiences negligible external forces (gravitational or any other), although she is, of course, never “massless.”



Next run:

Record the codes for auto-attribution for each page
Edit text - 
rearrange into a logical order
Remove idioms
Reduce extra test, switch to lists/tables
Remove unnecessary pictures
Remove italics
Start every page with heading?  
Have simple headings and subheadings for finding information
Make sure header start at h2 and are properly nested
Higlight text as mentioned in the style file, blue, green, red
Make a note to connect scientists in appendix with chapters. - they are usually in the text


12/29/25

Starting in Stellar Finale.  Finished in Cosmology, skipped active galaxies and galactic evolution in case Caitlin does not want them. 

12/28/25

Continuing through - also deleting duplicate openstax, skipping sun and powering stars

Made it to interstellar media

Run Summary:

Move learning objectives to main chapter
Move Link to learning to Further Exploration
Move Examples and Exercises to bottom, change headers
Delete duplicate Openstax
Remove footnotes - put in text, format html
Put in text connecting exploration and examples
Make sure table of contents is on
Move scientists to appendix - note link


12/27/25

Starting at color and temperature, gotten to telescopes



12/26/25

Next pass - entire book except first three - remove learning objectives and other links, and move exercises and examples to the bottom, 

I need to add equation building to my chatbot, or building another one. 

Future pass - when editing text - remove all italics.

12/25/25

Forgot to note where I stopped.  I am still in Active Galaxies atm  

Working on cosmology

Next remix- make sure that there are Key terms and alternative text  - complete

Next pass - entire book except first three - remove learning objectives and other links, exercises



Moving Appendices of scientists to ASTR 10



12/24/25

Replacing image thumbnails with pictures from openstax for milky way, galaxiesm cosmology

Starting back on black holes, going through and forking the Openstax pages, turning on the table of contents, and confirming the attributions.

Now doing another pass, putting Lumen into the Openstax chapters. 



12/23/25

ASTR10 Starting at Stars and Light

I made one pass through the ASTR 10 updating the openstax text to automatically attribute.

Now, I am going to make another pass and make sure that I have included all content on the main pages.  Just looking at chapters that still have resources, or the last couple that need combining. Starting with stellar tracking. Completed first pass

Working on mixing the extra chapters - black holes to cosmology. 

Working through Milky Way galaxy



12/22/26

Working on the transcluded pages.  Remember to add both Openstax and Lumen

Milky Way Openstax, 

Introduction to Astronomy has the codes, so copy those up

Galaxies, Active Galaxies, Quasars, Openstax  Galaxies, Evolution of Galaxies, just move those up?

Now, going through chapter by chapter and putting in the codes, or copying in text

Starting at chapter??




12/21/25

Took a couple days off to prep class.

Back to putting working with Chem Openstax  and Lower starting at the atom

Finished with the chemistry textbooks.  Not sure if all of the text was properly copied in, but I can check that when I am editing.  

Now I am going to go back through and freshly transclude the last couple chapters, black holes, Galaxies, and cosmology - removing science and society first

12/17/25

Embarassingly, still in Astronomy Toolkit, Introduction toPhysics 

But I did create several google sheets with information for specific OER sources, for attributions if needed. And spreadsheets for each chapter for ASTR 10 starting with toolkit.  Everything is in the Dr. Mastrapa google account. 

Got to elements and am importing some chemistry found an openstax general chemistry and a chem1 class

https://chem.libretexts.org/Bookshelves/General_Chemistry/Chemistry_2e_(OpenStax)

https://chem.libretexts.org/Bookshelves/General_Chemistry/Chem1_(Lower)



You know what?  Keeping track of everything separately is becoming tedious.  I am going to take advantage of this auto=attribution thing and just starting to copy in text. 



I think what I have to do, is to make sure that I keep a copy of all of the codes in comments or somethings before I edit to be sure everything gets credit.  And make sure that I re-copy anything from openstax.



Currently working my way through Openstax chemistry - https://phys.libretexts.org/Workbench/Solar_System_Sources/12%3A_Chemistry_2e_(OpenStax)/12.02%3A_Atoms_Molecules_and_Ions/12.2.04%3A_Atomic_Structure_and_Symbolism




12/16/25

Working on publishing a chatbot and sharing with Shagun and Chesa.  Done

Back to Astronomy 10, still in astronomy toolkit

12/15/25

Focusing on ASTR10 

This pass 

Copy in all chapters from ASTR 4, will finish them here
Move learning objectives to main page
Remove all links to learning and other boxes
Copy in codes from new Openstax for automatic attribution
Keep codes under attributions until loaded in spreadsheet. 
Track attributions in spread sheet and delete the ones that are automatic
Starting at Ch1 Astronomy Toolkit



12/12/25

Tracking Science and Society Progress

Meeting with Shagun

Pester her for next couple of week for eaccesibilty

FOCUS on 10 for winter

By July - both published and ready to share

Delmar - office hours - ask what he has done to attributions  - ask how to get tags

Get code number - for openstax

Copy and pasting within libretext should bring over

Let him know I am astronomy lead

Josh is working on a glossary

APA full hyperlink - italics

Share chatbot with shagun and chesa  

Look up resources folder - has AI stuff

About the book section - for AI  be very clear about use

Used in playlab - closed environment, IDEA, xlist specific uses

Use fior mechanical things - not as much te

Make a note to email every three weeks - check in



12/11/25

OK, Going through one concept at a time with Park for ASTR 4 - its pretty short

I am adding a chapter in the astronomy toolkit regarding physics

Finished updating the work plan spreadsheets.  The meeting is going to go however its going to go. 



12/10/25

Picking up on pass through Openstax for ASTR4  - Done with Openstax

Next Step

Pass through ASTR10 

move learning objectives to chapter heading
remove links to learning and other boxes
Highlight words
Green for key terms
Blue for a link that doesn’t exist yet
Red - notes on what needs doing
Actually, I am looking through Introduction to Physics, Park and starting with first three chapters in ASTR 4  I am starting with light, but I should go back through and do all of Park

https://phys.libretexts.org/Bookshelves/Conceptual_Physics/Introduction_to_Physics_(Park)/04%3A_Unit_3-_Classical_Physics_-_Thermodynamics_Electricity_and_Magnetism_and_Light/11%3A_Light/11.03%3A_Production_and_Properties_of_Electromagnetic_Waves





12/9/25

ASTR 10 - introductory to Astronomy - Lumen - going through page by page, I was in telescopic instruments

Doing Solar System, Rocky Planets in ASTR 4

It seems like I have to take Openstax section by section for ASTR 4 and paste them in

Finished Intro astronomy lumen up to the Sun, back to ASTR10  

Got up to Galaxies and quit there until i hear back from Caitlin

Now, Lumen Lab??  Finding stuff in lab,  

Next ASTR 4 and Openstax - I am at Earth’s Atmosphere



12/8/25

Coninuing on ASTR 10 astronomical instruments

Making pages CC By

First Pass - putting in content from spreadsheet

Second Pass -, 

move learning objectives to chapter page 
put in content from resources/ go through astronomy resources
I realized, a little late, that the stellar astronomy textbook is mostly from openstax, so I should have been transcluding pages this whole time.  Whatever.

Starting the second pass.  Going through Introduction to Astronomy



12/7/25

I created a new book called Topics in Physical Science and added the plate tectonics and climate 

Finished going through the CC BY Geology books

Going to switch back to ASTR 10 for a bit

Re-organized chapters by topic based on ASTR 10 Tracking sheet.  Made it to telescopic instruments putting content into pages



12/6/25

Jumping right back in - cleaning up geology

Separated Plate Tectonics and Geology, need to clean up plate tectonics

There is a section on Volcanism in 5.13 Climates and Tectonism - maybe I don’t need thatbecause it is more closely connected with climate - tho interesting



12/5/25

Starting back up with geology in Earth chapter.  

It might be better to just go through the SS sources book and make sure I am using everything. 

Right now, looking at Physical Geology Earle - remember to copy the image attributions into the captions  

Finished Earle, starting on Schulte - schulte used some lumen, so may not need it. 

Got through all the rock types in Schulte and am cleaning up the geology page



12/4/25

Finished checking ASTR 10 up through Night Sky Navigation, and asked Caitlin about restructuring of chapters.  

Focusing back on ASTR 4 - tacking in all material in resources.  

Solar System - went through resources - finished up to what fo geolofists do? In Ear;e



12/3/25

Starting on ASTR 10

Matching First three chapters

First adding Key Terms and Alt text

Next - get extra information from stellar into first three chapters in Stellar, note in Stellar that I will copy in info, also for Sun and Solar System??

fFinished the pass through of adding key terms, etc.  Am working on getting the Stellar book organized.  Putting everything on the same page.  I am in Night sky Navigation in the unused pages, looking at Newton



12/2/25

Continued cleaning up chapters in ASTR 4 - making sure there are no subchapters etc., added in key terms and alt text pages

Finished at Small Bodies.  



When done with this pass do the same for ASTR 10??



12/1/25

Continuing work on lining up both tracking sheets and content for the first three chapters of both textbooks

The details for the chapters are in the google sheet for AST 10 and I am editing the chapters in ASTR 4.  Confusing, I know.  

Finished outline on Astronomy Toolkit and working on Introduction to Astronomy/Origins of Astronomy. Getting rid of subchapters

Deleted Cultural Impact

11/30/25

Reorganizing the Tracking OER Curation pages,  Doing first three chapters in ASTR10, and just noting copy in ASTR 4

Making notes in both tracking sheets and libretext where material is overlapped and which textbook or tracking sheet I am working in.  



11/26/25

The AI seems to be working, and I am spending a lot of time tweaking it.  For now, I am shifting to just writing. In Sun Chapter

Using Tracking OER Curation sheet and Solar System Textbook Resources - combine??  Change AI to work with Curation sheet?



11/25/25

Sunny Chatbot - Updated data input for attributions. Copying in from spreadsheet.  

Also having it list a table of prompts 

Working on references in Cultural Influence of the Sun.  Need to research and write that later. 



11/24/25

Back to editing chatbot and hopefully starting on Solar Chapter editing.

I am focusing on finishing implementing multiple chapters in a citation and other corrections.  

When I start it up again, I will ask it for questions. Created a project #SunnyChatbot to track future improvements

Multiple Chapter HTML Format: There's an incomplete pattern in the HTML formatting section. The instructions mention using ",,," to represent continuing patterns, but the actual HTML example doesn't fully demonstrate how to handle multiple chapters with proper comma placement and "and" before the final item.


Variable Notation Inconsistency: The instructions use different bracket types for variables - sometimes [brackets] and sometimes {brackets}. For example: "Chapter Title[Chapter Link]" vs "Textbook Title{Textbook Link]" - this should be consistent.


Missing Closing Bracket: In the text format example, there's "Textbook Title{Textbook Link]" which mixes bracket types.


Incomplete Multiple Chapter HTML: The Multiple Chapter HTML Format section shows the pattern but doesn't complete the full example with all the chapters, commas, and "and" formatting.


Step Numbering: In the workflow, there are some nested numbering issues that could be confusing to follow.


Learning Objectives Section: The instructions mention various formatting tasks but don't provide specific formatting examples like they do for attributions.
Redundancy in Step 2.1.9 - The instructions repeat the same action twice for both "yes" and "no" responses, which seems like it should have different outcomes.


Missing Example in Multiple Chapters - In the "Multiple Chapter Example Text" section, there's an incomplete chapter title: "7.2:" Overview of our Planetary System" should probably be "7.2: Overview of our Planetary System"


HTML Title Inconsistency - In the Multiple Chapter Example HTML, one link shows "A Tour of the Universe" in the display text but "1.7: A Tour of the Universe" in the title attribute, while others are consistent.


Unclear Variable Handling - The instructions mention treating Author as a "string" but don't specify how to handle multiple textbooks with different authors in a single attribution.


Missing Guidance - No clear instructions for handling situations where someone provides partial information and wants to come back to complete it later.


Format Clarity - The bracket notation [Chapter Link] in examples might be confusing since it's showing where variables go, but could be mistaken for actual formatting.
These are all valid, but I am making some notes for improvement and moving on.  

In Chapter 5, the Sun, implementing Thumbnails Captions

Skipping Cultural Influence for now



11/22/25

Editing Solar Chapter and working on playlab chatbot at the same time.  

Chatbot 

Named the chatbot Sunny

Update my prompts from is to includes so I can write complete sentences.

Put in some instructions for asking questions about how the chatbot works.  

Will keep all of my summaries in the document Solar System AI Log

I asked the bot to help improve my instructions, here are some suggestions I will fix right now. 

Learning Objectives Section: The workflow says to ask "what Rachel wants done with the learning objectives" but doesn't specify what formatting options are available. It might be helpful to know what typical formatting tasks you'd like me to offer (like converting to HTML lists, numbering them, etc.).


Author Link Handling: In the example, the author link is shown as empty [] in the text format, but the HTML format has a working link. Should I ask for clarification when no author link is provided, or is it acceptable to leave it blank?


Multiple Authors: The example shows multiple authors separated by commas, but the instructions ask for "the Author" (singular). Should I ask how to handle multiple authors when they're provided?


Chapter vs Section: The format says "This section was adapted from..." but asks for "Chapter Title" - should I be flexible about whether it's a chapter or section?


"Done with Instructions" trigger: The instructions say to restart when the response includes "done with instructions" - should I also watch for similar phrases like "finished with questions" or "no more questions"?




11/21/25

Trying to implement AI tools

Creating Notebook LM (mastraparachel@fhda.edu account)for each textbook, starting with Solar System

Including these files

Table of Contents OER Solar System Textbook

NotebookLM was a bust for this application, switching to Playlab.  This may work much better, and it can save to google docs - implement that next

OK.  That was not a lot of work, and it gave me suggestions:

## Session Summary



### Activities Completed:

- **Attribution Formatting**: Successfully formatted one attribution citation for:

  - Chapter: "1.7: A Tour of the Universe" from OpenStax Astronomy 2nd edition

  - Authors: Andrew Fraknoi, David Morrison, and Sidney Wolff

  - License: Creative Common Attribution License 4.0

- **Output Formats**: Provided both plain text and HTML formatted citations ready for use in your OER textbooks



### AI Citation (APA Format):

OpenAI. (2024). *ChatGPT* (GPT-4) [Large language model]. https://chat.openai.com/chat



**Note**: This citation should be adapted based on your institution's specific AI citation guidelines, as standards are still evolving.



### Suggestions to Improve This App:

1. **Batch Processing**: Add capability to format multiple attributions at once from a spreadsheet or list

2. **Template Variations**: Include additional citation formats (MLA, Chicago style) for different institutional needs

3. **Validation Features**: Add URL checking to ensure links are active and properly formatted

4. **Save/Export Options**: Allow users to save formatted citations to a file or clipboard

5. **Preview Mode**: Show a visual preview of how the HTML will render before finalizing

6. **Quick Edit**: Allow users to make minor edits without re-entering all information

7. **Common Sources Database**: Build a library of frequently used textbook information to speed up the process



Thank you for using the OER Textbook Formatter, Rachel! Feel free to return anytime you need help with formatting attributions or other textbook elements.



8/24/25

Whoops.  Forgot to log.

Backed up ASTR 4

Went over what caitlin finished

Caitlin will do science and society for ASTR 10.  I can make them overlap with ASTR 4.

Need to finish project tracking draft today  - need to figure out science and society - number and location

My method for replicating the first two chapters between the textbooks - I am going in the OER remixer and rearranging the chapters, with a lot of pages representing topics.  However, Shagun does not like a lot of sub and sub-sub chapters, so I will be collapsing multiple pages into single long pages.  I have started doing that with my Solar System Chapter in case you want to see an example.  Appartently, lots of pages is bad for accessibility.  

Overlap 

Clones - Ch1 Introduction to Astronomy  Ch 2 Night Sky Navigation  - figure out which book has most progress - edit that one, copy to the other.  Ch3 Astronomical IInstruments and Observations (write in stellar)

AST4 The Sun, - spectroscopy - summarize from ASTR10 Stars and Light, Spectral Appearances

ASTR 10 The Sun and OUr Solar System - Summarize from ASTR 4 - The Sun, The Solar System  and Powering the Stars - Summarize from ASTR 4 The Sun



ASTR 4 - Solar System - star formation section - summaraize from ASTR 10 Star Formation and Evolution



ASTR 4 - no cosmology???

ASTR4 Exoplanets, pull in star colors, luminosity, etc. 



8/14/25

Committed to  both textbooks, need to make a plan for scaling back:

Removing chapter text review.  
No ADAPT
Moving all references to the end of each chapter
Moving all learning objectives to main chapter page
No further exploration
Eliminating individual definition boxes, and changing to one Key Terms at the end of each chapter anchor definition to each word
Combine multiple pages together down to single, long pages


What I will do:

Figure out how to back up - may have to do it a page at a time 
a.                  Copy current structure in remixer

b.                  Copy each page as I change it in the new version. 

Keep careful record of all sources in spreadsheets.  
a.                  Get the original spreadsheet from Caitlin or recreate - probably the matrix one

b.                  Create a new sheet ASTR 10 OER tracking

Define new workflow for each page
a.                  Chapter UDL - start with learning objectives, create sections based on, or work with current sections and create them

b.                  Each section

i.Import text, images from Lumen, Openstax

ii.Create attribution for page

iii.Caption, alt text, attribute images

iv.Format text

v.Create key terms page and define terms, anchor, etc

Keep Summary Pages
Have references at the end of each chapter
Key terms - bulleted list, elements - anchor - bold term in page, link - anchor save with a name and then hyperlink to definition
a.                  De

Alt text - details in caption  - look at images in decreasing order of use
a.                  Details in caption - write alternative text description

b.                  Otherwise say details in text.

c.                   In caption - make a title of a the image

d.                  At end of chapter have a section called alternative text descriptions - make anchors  and link to alternative text description 

Use periods in alt text  - link public domain  - wikipedia 
Stop hyperlinking
Write alternative text description when talking about the images in detail
Keep attributions and references on same place
Activities - canvas commons oer commons - discussion question - 5-7 per chapter
Dont use ADAPT  - can use formative but  - no ADAPT



8/12/25

Just volunteered for both textbooks for double money.  Got a lot of work coming up.  

Finishing solar system and sending to shagun, then re-arranging schedule unless she wants to meet.



8/11/25

Libretext has been down all weekend.  Focusing on outlining.  Updating OER curation sheet



Look in OER_scratch.txt for captions, attributions, sources




8/5/25

Changing some organization for simplification

Break scratch textbooks into two: Solar System Templates, Solar System Sources



Let’s make this a multi step process

Remix Map

Open tracking OER spreadsheet
Fill in links to spreadsheet for the chapter
Make a note about how much of the material and location I plant to use


Transcluding

4.                  Open tracking OER spreadsheet

5.                  Fill in links to spreadsheet for the chapter

6.                  Note if you are using the entire page or just a section

7.                  Open Conductor and mix in the material that you are using the whole page. 

8.                  Add all material to Solar System Textbook for cutting and pasting small parts



Remixing

Open project link

Open solar system textbook in another weekend

Copy in small parts of 



8/2/25

Solar System 

Pluggin along



8/1/25

More Solar System

Created Appendix with list of astronomers - moving all historical information there. 

7/31/25

Solar System

Changing terminology to Inner and Outer planets - editing



7/30/25

Continuing with Solar System



7/27/25

Moving all of the data tables to the ends of chapters, but before comparative planetology, changing name to Summary of - can be remixed for simple list of planetary facts without background, can include links to chapters with further information

Back to Solar System



7/25/25

Back to Solar System

Process for rough draft

For each page, 

Include objectives or chapter summary
Import any existing OER - include in tracking sheet
Make any notes in red highlight
Make a list of tables or images that I want to include - add to OER tracking sheet
Add attributions and sources, or placeholders
If adding definitions, add word to glossary
Run accessibility check


7/22/25

Moving through rough drafts

Chapter 4 - Solar System

Using a different project - Solar System Astronomy in Libretext conductor - storing templates so I can copy and paste - see if I can have different books open - I heard that if you have multiple windows of the same book open, it crashes.  

Actually, I am taking the time to copy all of Openstax astronomy into Solar System Astronomy, and fork each page as I need it, so I can just copy window to window instead of transcluding.  I will save transcluding for times when I use the entire page, or a big section.



7/20/25

Going over Sun chapter.  Filling in requirements, highlighting notes. 



7/14/25

Yesterday finished filling in the curation spreadsheet

Am now working on properly including all sources on pages

Still have sources that I need to find, especially DEI and cultural impact



7/13/25

Focusing on Sun Chapter

Outline and transclude or copy in material from Openstax Astronomy



7/10/25



Working on astronomy now - basic outline

Shrank all thumbnail images

Citing Understanding Science

You may cite the website using this format:

Understanding Science. 2022. University of California Museum of Paleontology. 3 January 2022 <http://www.understandingscience.org>.

… with the ‘3 January 2022’ being the date you accessed Understanding Science.

You may cite an individual article using this format:

“Asteroids and dinosaurs.” Understanding Science. University of California Museum of Paleontology. 3 January 2022 <https://undsci.berkeley.edu/asteroid...inished-story/>.

… with the ‘3 January 2022’ being the date you accessed the article.



7/4/25

Continuing below, starting at 1.2.2

Skipping learning objectives for now, will go back and add later



7/3/25

Starting at chapter 1

            Filling in OER excel sheet, including OER and other resources I need - moved to Google to display properly + color coding

            Include outline of material in each page in libretext

            Include learning objectives - just for main chapters for now,  work on sub-chapters later?



7/1/25

Reminder that libretext tracks changes.  Don’t need to cover details.

Re-organizing Chapter 1 - How to Use This Textbook

Also, filling in excel spreadsheet OER Tracking for each chapter, so that I can keep track of what I am using, and what needs help. 



6/26/25 

Creating learning objectives with Notebook LM 

Create Learning objects for chapter 1 based on the Student Learning Outcomes and the Solar System Learning Objectives 

• 

Students will be able to effectively navigate and utilize the textbook's organizational structure, including its chapter breakdown, to efficiently access the comprehensive account of modern planetary astronomy, detailed appearances and physical characteristics of major planets revealed by space probes, and various modes of astronomical research described throughout the book 

. 

• 

Students will be able to apply units of measurement and scientific notation to accurately represent and comprehend the vast scales and distances within the universe, thereby fostering an increased sense of place and scale 

. 

• 

Students will develop proficiency in utilizing scientific notation and understanding units of measurement as fundamental tools, which are crucial for interpreting and evaluating quantitative data and theories related to solar system astronomy based upon the scientific method 



Don’t really need these since chapter 1 is chapter 0.  

Feeding in the RSI material about outcomes and these web sites 

https://resources.depaul.edu/teaching-commons/teaching-guides/course-design/Pages/course-objectives-learning-outcomes.aspx 

https://tips.uark.edu/using-blooms-taxonomy/ 



Using all sources, create learning objectives for Chapter 2. 

Here are the learning objectives for Chapter 2: 

• 

Students will be able to describe the historical origins and evolution of astronomical observation, including how early civilizations used the sky for keeping time, navigation, and predicting the future 

. This objective fosters an increased sense of how our species reached its current understanding of our world’s place in the larger scheme of things 

. 

• 

Students will be able to explain the fundamental principles of modern astronomical research, including the nature of light, the operation of various types of telescopes and detectors, and the application of spectroscopy 

. This objective aims to generate a familiarity with the various modes of research which astronomers use to investigate other planets, including automated spacecraft 

. 

• 

Students will be able to evaluate astronomical news items or theories concerning solar system astronomy by applying the principles of the scientific method 

. This objective is directly supported by the "Astronomy Now" section and "The Nature of Science" resources within Chapter 2 

. 

• 

Students will be able to articulate foundational concepts related to the structure of the universe, including the Earth-Moon-Sky system and basic orbital mechanics 

. This understanding contributes to an increased sense of place and scale in the universe 

. 

• 

Students will be able to summarize the core ideas and goals of astrobiology, encompassing the cosmic context for life and the search for extraterrestrial intelligence 

. This objective helps students to appraise the benefits to society of planetary research and exploration 



Try Khanmigo? 



6/20/25 

Building out structure for entire book 

Making Structure of the book in Conductor 

Copying notes into chapter subheadings, so I can copy in Openstax when I need it. 

5/14/25 

Working on Moon body 



6/13/25 

Building out topic structure in chapters 

NEVER COPY TEXT FROM A WORD DOC – double check any text that you paste in – make sure that you can edit it 
Can copy in from google docs 

5/12/25 

Setting up strucutre of Mercury chapter in Libretext 

Filling in image thumbnails for all chapters with caption and attribution in the chapter page 



5/10/25 

Breaking up textbook into more chapters so that I don’t have such deeply nested files.  The Moon and Mercury are now their own chapters.  

Roughly agreed on a style file for chapters. 



6/3/35 

Chapter 5 Mercury and the Moon 

Building outline structure of chapter in Tracking OER spreadsheet 

Editing some chapters about the Moon, highlighting things I need 





Textbook Outline 

Sources  

Solar System Textbook Dana Backman, Mike Seeds 

Web Sites: NASA and Wikipedia 



Introduction to Astronomy 
Origins of Astronomy 
Why observe the sky? 
2.                  The First Observers 

Tools – Eyes, Hands, Maps/Charts, astrolabe 
2.                  The Celestial Sphere 

Famous stars, constellations, Names? 
2.                  Model that represents positions of objects in the sky. As the first astronomers would see  

3.                  Angular distance/relative positions 

3.                  Str uctures  

Stonehenge, Newgrange, temple of isis, dendera egypt, Sun dagger, new mexico, mayan books destroyed by spanish could predict motions of venus and phases of moon 
4.                  Extra 

Greeks –Plato, Eudoxus, aristotle, aristarchus, Eratoshtenes, ptolemy 
3.                  Keeping Time 

Measuring a Day – Why? 
Motion of Sun and Stars 
2.                  Telling time of day by the Sun 

3.                  Telling time of night by the Moon  - include? 

4.                  Ancient astronomers knew that the stars were up during the day – why do you think some people get this wrong now? 

2.                  Tracking a month – Why? 

Phases of the Moon 
Names of the phases 
2.                  Moon orbit – synchronous rotation (1) - without tidal forces 

2.                  Moon related holidays 

3.                  Tracking a Year – Why? 

ecliptic 
2.                  The Zodiac 

4.                  Navigation 

Finding directions 
Zenith, cardinal directions 
2.                  Using the sun during the day 

Cardinal directions 
3.                  Using the stars 

North Star 
2.                  Using the stars to sail the ocean 

Constellations 
2.                  Sextant 1700s? 

5.                  Predicting the Future 

Eclipses ((pen)umbra, total/totality) total vs partial – why not eclipses twice a month? Is above or below Moon 
Lunar eclipse – full moon only (but not all full moons) 
Red color (view from Moon) artmosphere lit by Sun – scattered blue light 
2.                  Knew earth was spherical because of circular shadow on Moon 

2.                  Solar eclipse (new moon only, but not all new moons) mayan monsters eating moon 

Hsi and ho beheaded by emperor –failed to predict eclipse of october 22, 2137 
2.                  How to safely observe and eclipse – define risk, provide resources 

3.                  Path of totality 

4.                  Annular eclipse – apogee/perigee 

5.                  Corona 

6.                  Extra diamon ring effect 

3.                  How to predict 

Mapped path of moon in sky 
2.                  Found nodes – points where path of Moon crossed path of Sun (ecliptic) 

3.                  Eclipse season – when Sun is near Moon’s nodes – observations + maps! 

2.                  Planets: The Wandering Stars 

Fixed Stars 
2.                  Retrograde Motion  #1 

3.                  Geocentric model/epicycles? 

3.                  Astrology 

2.                  Astronomy Now 

How Modern, Western? Astronomy Works 
Objective Observations/Measurements 
2.                  Scientific Method – for each experiment 

3.                  Scientific Communication – for development of the field 

4.                  Science Dialect- words that mean different things in science 

2.                  Light – Astronomy's Main Source of DataLight 

What is Light? 
2.                  Speed of light/Scientific Notation 

3.                  Different Types of Light: The Electromagnetic Spectrum 

3.                  Telescopes – how to catch light 

Changing Views of the Solar System 
Geocentric Model 
Reasonable based on observations 
2.                  Parallax  

3.                  Became less predictable with time 

2.                  Heliocentric Model 

Telescope Observations 
Galilean Moons 
2.                  Phases of Venus 

2.                  Explained retrograde motion 

3.                  Improved predictions 

4.                  Extra = copernicus, Galileo 

2.                  What types of light can reach the surface of the Earth – do they need to know this – do we get to any types of light other than visible? 

Electromagnetic spectrum (1) different types of light 
2.                  Define wave properties of light 

3.                  Define wavelength, frequency, amplitude, crest, trough, etc 

4.                  Lambda * nu = c 

5.                  Ground based vs. Planes/balloons vs satellites 

3.                  Detectors 

Better than eyes or photographs 
Photometer – measures brightness of object very accurately 
2.                  CCD – photons  

2.                  Need different detectors for different types of light 

3.                  Extra 

Historical – photographic plates 
4.                  Modern/large telescope 

Location requirements 
2.                  Impact on local populations – environment & cultural 

5.                  Extras 

Refracting, refectors 
Newtonian/Cassegrain 
2.                  LGP, resolving power, magnifying power 

4.                  The Universe 

Age of Universe/Big Bang  
2.                  Size of the Universe 

3.                  Content of the Universe 

4.                  Our time and place in the universe 

3.                  Astrobiology – move to Earth? 

What is Life? 
Words in Science 
2.                  Consensus 

3.                  The Checklist 

2.                  Requirements for Life 

Life as we know it 
Origin 
2.                  DNA 

Molecules – need to talk about atoms/elements 
3.                  Diversity & Complexity 

Single-celled vs. Multi-celled 
2.                  Intelligence 

3.                  The Search for Life 

Extinct vs. Extant 
2.                  Follow the Water 

3.                  Sample Return 

4.                  The Drake Equation 

2.                  Solar System Structure and Formation 

Structure of the Solar System 
Orbits 
Ellipses 
Semi major axis, eccentricity, foci 
2.                  How to make an ellipse 

3.                  Kepler’s Laws 

Ellipse 
2.                  Equal areas equal times (speeding up and slowing down – angular momentum 

3.                  P2 = a3 

2.                  Prograde and retrograde motion/parallax 

3.                  Gravity  

Laws of Motion ? 
2.                  Inverse square law 

3.                  Orbital and escape velocity? 

4.                  Extra: Brahe, Kepler, Newton 

2.                  Terrestrial Planets 

3.                  Gas Giants 

4.                  How Did We Get Here?  

2.                  History of the Universe 

Big Bang 
2.                  Stellar Formation & Evolution 

3.                  Galaxies 

4.                  You Are Here 

3.                  The Solar Nebula Model 

Nebula Composition 
How do we know 
2.                  Primitive material – comets, asteroids, meteorites 

3.                  Observations of other nebula – transmission spectroscopy? 

2.                  Stages of nebula model 

Angular momentum 2 
3.                  Planet Formation 

Planetesimals 
2.                  Protoplanets 

4.                  Ice Line 

Temperature – movement of particles 
2.                  Scale - Fahrenheit/Celsius/Kelvin 

3.                  The Sun 

Cultural Influence 
2.                  Exploration 

Remote Sensing Overview 
2.                  Observations from Earth 

3.                  Spacecraft 

Preview Types of Spacecraft? 
2.                  Robotic vs Crewed 

3.                  Flyby, Orbiter, Lander, Rover, Drone 

3.                  The Sun We Can See 

Interior – below photosphere, atmosphere – above photosphere 
2.                  Need figure of temperature change from photos = chromos = corona 

3.                  Photosphere 

Temperature - Blackbody radiation 
Thermal energy/heat 
2.                  Temperature – motion of particles in object  

3.                  Wien’s Law – max wavelength inversely proptional to temperature. 

2.                  5780 K 

3.                  Light that reaches the Earth comes from here 

4.                  1/3000 atm pressure 

5.                  Denser at bottom – opaque to light beneath 

4.                  What are stars made of? 

Atoms 
Nucleus, protons, neutrons, electrons 
2.                  Elements – different number of protons 

3.                  Electron Energy levels 

2.                  Light and matter interactions 

Ground state 
2.                  Excited state – emission 

3.                  Photon Properties of light 

E = hc/lambda = h*nu 
2.                  Transition absorbs or emits photon 

3.                  Series? Balmer, Lyman, etc 

4.                  Photon energy -> corresponds to specific transition energy 

5.                  Specific photon energy = specific photon wavelength 

6.                  Atomic Spectra – visible wavelength 

Kirchoff’s Laws – need images of each typer of spectrum 
2.                  Continuous spectra (blackbody)  

3.                  Emission spectra 

4.                  Absorption spectra 

5.                  Usually plotted intensity vs wavelength need chart example, ideally compared with color rainbow image 

7.                  Chemical composition 

What something is made of 
2.                  Can only prove that something is there, not prove that something is not  

3.                  Sun’s spectrum is absoprtion – continuous from surface, passing through atmosphere that removes  

4.                  Cecilia Payne – 1925 PhD detrmined how to analyze Sun and stars - need image, interpretation of spectra 

Can identify what is there 
2.                  Can calculate amount of atoms of a particular element 

3.                  90 % hydrogen, 10% mostly helium 

4.                  Ca Na Fe have strong features but are low abundance because they are more effecient at absorbing photons in the temperature/pressure conditions of the photosphere 

5.                  If the line of an element can’t be seen – might still be there 

Too hot or too cold 
2.                  Not the right density 

3.                  May not be producing the lines in the wavelength range that you are looking in 

4.                  Still not sure about CNO abundance – need to know more about conditions in chromo 

6.                  Spectrum of photosphere 

Lower, denser layer produces continuum 
2.                  Higher, transparent layer – absorbs photons, spectra of hydrogen, helium, and others 

8.                  Granulation – need image of photosphere 

Convection – hot centers rising, cool edges sinking – describe physics of convection – need figure 
2.                  A little bigger than Texas 

3.                  Last 10-20 minutes 

9.                  Supergranules 

Twice the size of Earth 
2.                  2 days 

3.                  Come from deeper than granules 

10.              Limb darkening 

Looking at center of disk, looks deeper than looking at limb 
5.                  Chromosphere 

Above photosphere, blends into corona 
2.                  Can only be seen by eye during eclipse 

3.                  Pink – red, blue, violet Balmer lines – Emission spectrum 

4.                  Pressure 1/10,000 atm at bottom, 1/100 billion atm near corona 

5.                  Atoms in lower chromosphere is ionized 

4500 K near photosphere 
2.                  Near corona hot enough to release x-rays 

6.                  Filtergram 

Most of chromosphere is transparent, but some atoms absorb forming very strong absorptions 
2.                  Image of Sun at wavelength of strong absorption can show structure of chomosphere   - image?? 

3.                  Shows spicules at edges of supergranules – need image? - cooler gas from lower chromosphere 

7.                  Far-UV or X-ray images 

6.                  Corona 

Inner parts can be seen during eclipse 
2.                  Coronagraph – blocks photosphere – corona goes out to 20 solar radii – 10% of way to Earth 

3.                  Spectrum – emission lines  of highly ionized gases  

Ions – atom that has gained or lost one or more electrons 
2.                  Amount of ionization increases with altitude 

3.                  Ionized gas = plasma 

Phases of matter? 
4.                  Temperature – 500.000 K near chromo – up to 2 million K – emits X-rays, but very low density, so not a lot of X-rays 

5.                  Magnetic carpet 

SOHO mission 
2.                  Looped magnetic fields extend up through photosphere – some loops as large as Earth 

3.                  Turbulence from below photosphere moves loops around, heating gas 

4.                  Hinode mission – detected gravity waves traveling up from photosphere – heating ga 

5.                  Also IRIS data – uv images, of upper chromosphere and lower corona – check for results?? 

6.                  Ionized gas flows along magnetic field lines – loops, back into Sun, open – solar wind 

7.                  Solar Wind 

Low-density 
2.                  Near Earth - 300-800 km/s, gusts 1000 km/s b 

3.                  Heliopause – solar wind meets interstellar space 

4.                  Sun loses 1 million tons / second 


4.                  Solar Activity 

What we see on the outside of the Sun depends on what is going on inside 
2.                  No light from below photosphere = no information 

3.                  Helioseismology 

Convection in Sun produces vibrations 
2.                  Most common is 5 minutes, others range 3-20 minutes 

3.                  Convection means parts of the Sun are moving towards or away from the Earth 

4.                  Doppler effect  -red shift = away, blue shift = toward   need figure demonstrating doppler effect 

Radial velocity ( velocity is a vector) 
2.                  Calculate doppler shift?  Vr/c = delta lambda/lambda_zero 

5.                  Preview – geologists know earth’s interior by studying seismic waves 

6.                  Astronomers use GONG (Global Oscillation Network Group) data, to model the interior of the Sun.  need illustraion of sound waves in Sun and models of Doppler shifts from SOHO data 

Mapped out temperature, density , internal rotation rate 
2.                  Convection region is 29% of solar radius 

4.                  Sunspots           

Safe observing of Sun – never look at the Sun, especially through any magnification (burning leaves with magnifying glass 
2.                  Seen by Galileo? 

3.                  Sunspots are cooler, darker spots, on photosphere, formin groups, last on time scales of weeks and months -   need image od Sunspots w/time 

4.                  Amount of sunspots have 11 year cycle – sunspot minimum and maximum 

5.                  Maunder buttergly diagram – sunspots appear high latitudes at beginning of cycle and closer to equator at end 

6.                  Zeeman effect – atoms in a magnetic field – changed energy levels, can absorb photons at a greater range of wavelengths – spectral line split into several components  

7.                  Sunspots contain magnetic fields, suppress flow of heat from below, it comes out around the edges 

8.                  Maunder minimum? 

9.                  Sun releases more energy/radiation during sunspot maximum 

10.              Active reagions Can see loops of magnetic fields in chromo and corona 

5.                  Magnetic Cycle  

Dynamo effect – convecting ionized material creates magnetic field, same flow of liquid metal core in Earth (preview) 
2.                  Differential rotation  

Photosphere – equator rotates fastest 
2.                  Convection layer – different depths rotate at different speed 

3.                  Babcock model 

Magnetic cycle is due to tangling and untangling of magnetic field, need illustration of tangled field lines 
2.                  Sunspot pairs appear where loops break through surface of photosphere 

3.                  Suspot pairs have reversed polarity N & S of equator – need image showing N S and S N pairs  

4.                  22 year long magnetic pole reversal 

5.                  Model predcits butterflyu 

6.                  Structures – prominences, filaments 

7.                  Flare – loop contact – big release of energy 

CME coronal mass ejection – very large CME 
8.                  Coronal hole –  

where magnetic field line does not loop back 
2.                  Source of solar wind 

9.                  Solar weather – 1859 solar eruptions ?  need to monitor 

10.              Aurora? 

11.              Nucleosynthesis 

elements 
4.                  The Earth 

Earth-Moon System 
Synchronous rotation – time to complete orbit = time to complete rotation 
Tidally locked – 
 gravity of Earth pulls on Moon forming bulge,  
2.                  Tidal friction - Earth pulls on bulge as it rotates away 

3.                  has slowed down rotation of Moon over time until bulge permanently pointed at Earth 

2.                  Works both ways, Earth has slowed down as well,  

may eventually become locked to the Moon,  
2.                  Exercise: consequences of becoming tidally locked to Moon 

so only one side of Earth can see the Moon,  
2.                  Permanent tides – constant sea level 

3.                  Sun may become a red giant first 

2.                  Center of Mass 

3.                  Eclipses 2 –  

view from space plane of Moon’s orbit is tilted relative to orbit of earth around the Sun 
2.                  Line of nodes 

3.                  Saros cycle – needs long records of eclipses 

4.                  Tides 

Gravity review 
2.                  Shape of tides 

3.                  Spring, neap 

4.                  Rotation of earth 

5.                  Synchronous rotation 2 – tidal friction, also called tidally locked 

6.                  Tidal effect of Moon on Earth 

2.                   

2.                  The Earth 

History and culture – creation myths 
2.                  Locating on Earth – lat & long 

3.                  Precession 

4.                  The Seasons 

Distance 
Evidence – opposite seasons in northern and southern hemisphere 
2.                  Earth perihelion is in January 

2.                  Equinox/solstice 

3.                  Length of day + angle of light (photons?) 

5.                  Geology 


Age of rocks 
Relative ages vs absolute ages 
2.                  Isotopes 

2.                  Volcanism 

Magma below the surface, lava above 
2.                  Magma – melt of lower crust and upper mantle.  Heat rises from below, melts rocks at lower pressure 

3.                  Heat rises from the core, but it is not core material that comes to the surface 

4.                  Viscosity of lava – different types of volcanoes 

Basalt – very low viscosity – spreads over large areas. 
6.                  History of Earth 

Formation 
2.                  Internal Heat 

Heat of formation 
2.                  Radioactivty 

3.                  Heat source of surface activity – volcanism, plate tectonics 

3.                  Differentiation 

7.                  Extra 

Milankovitch cycles 
5.                  The Moon and Mercury 

The Moon 
Influence on Culture 
2.                  Exploration 

Observations From Earth 
Atmosphere 
Basically none = no sound 
2.                  Evidence 

Stars do not fade at limb (edge) due to atmosphere (transit – later used to measure atmospheres) 
3.                  Terminator, - line between light and dark is very sharp – no air to scatter light.   

2.                  Surface 

Lunar highlands 
Mountains – not from plate tectonics but overlapping craters 
2.                  Crater saturation – any new crater must destroy an old one 

2.                  Lowlands 

3km lower than highlands 
2.                  Maria (MAH ree uh) latin for seas, single mare (MAHR- ray)– smooth dark planes – early observers thought they were lakes, or oceans but have ridges, faults, & craters 

3.                  Lava flows but no volcanoes 

A few small lava domes 
2.                  Sinuous rilles – collapsed lava tubes 

3.                  Impact Cratering 

Steps 
High velocity object coming at target 
2.                  Hits surface – meorite is heated and can be melted or vaporized – gnerally destroyed if not slowed down by atmosphere 

3.                  Object explodes – excavating bowl shape, ejecta blasted out 

4.                  Rebound creates central peak 

5.                  some eject falls back in – can contribute to central peak? 

6.                  For larger craters – slumping of sides creates rings 

2.                  Secondary craters – created by eject of large impacts 

3.                  Rays – bright streaks radiating out from crater – trails left by flying boulders 

Sign of “youth”   
2.                  Rays are disrupted by micrometeorite impacts, and darkened by sunlight 

3.                  Example Tycho is only about 100 million years old 

4.                  Micrometeorites – small craters created by microscopic size meteorites 

5.                  Multi-ringed basins – very large crater with multiple ridges – example Mare Orientale 

6.                  Crater diameter ~10x diameter of object 

4.                  Have not seen a lot of impacts, very littls change in surface since first telescope observations 

5.                  Crater ages 1 - relative ages vs absolute ages 

2.                  Race to the Moon 

Soviet Unions and US 
USSR gets first robotic missions, image of the far side, lander, rover, robotic sample return 
2.                  NASA lands first people 

2.                  Spacecraft Design 

Command module  
3 Astronaut living space 
2.                  Life support, food, communication, navigation, computers 

2.                  Lunar Module 

Had only enough fuel and supplies for trip to Moon and back 
2.                  Min weight max manueverability 

3.                  2 astronauts – no seats 

4.                  Flexible walls 

5.                  Legs not strong enough to support the LM on Earth 

6.                  Left descent rocket and support stage on the Moon 

7.                  Docking – hard 

8.                  Transferred rocks and astronauts and jettisoned LM 

3.                  Jul 1969 – December 1972 

12 people (1 geologist) 
2.                  380 kg of rock – Planetary Materials Laboratory at JSC Houston 

3.                  Apollo 11 Mare Tranquilitatis 

4.                  Apollo 12 Oceanus Procellarum 

5.                  Apollo 13 “Houston, we’ve had a problem” 

6.                  Apollo 14 Fra Mauro – ejecta from Mare imbrium  

7.                  Apollo 15 Apennine Mountains, Hadley Rille 

8.                  Apollo 16, 17 highlands 

9.                  Make a table of missions 

10.              Left stuff on the surface 

Flag, rovers, etc 
2.                  Sesimometers 

3.                  Mirrors? - laser ranging 

3.                  Spacecraft  https://en.wikipedia.org/wiki/List_of_missions_to_the_Moon 

Remote Sensing w/ Images/ Intro to photogeology 
Image resolution/pixels 
2.                  Light direction & shadow –interpreting structures 

3.                  False color/representational-color 

2.                  Luna missions, Zond, KOSMOS 

Russians got first image of far side 
2.                  https://moon.nasa.gov/resources/26/first-photo-of-the-lunar-farside/ 

3.                  Roscosmos – Luna 25 

3.                  Pioneer/Ranger, Explorer 

4.                  Japan – Hiten, Geotail, Nozomi, SELENE, Hakuto-R, SLIM 

5.                  US WIND, Clementine, HGS-1, Lunar Prospector, WMAP, SMART-1, STEREO, ARTEMIS, LADEE, TESS, CAPSTONE 

6.                  China Chang’e, Chang’e 2, 3, 4, 5,  Queqiao 

Chang’e 4 first to soft land on far side of the moon 
7.                  India Chandrayaan, 2, 3 

Chandrayaan 3 soft landed on south pole 
8.                  Isreal – Beresheet 

9.                  Korea - Danuri 

10.              GRAIL  https://science.nasa.gov/mission/grail/ 

Ebb and Flow 
2.                  Measured gravity data 

3.                  Mascons (mass concentrations) in basins are mixture of surface rock melt and denser mantle rock that flowed up from below 

11.              Clementine, Lunar Prospector, LRO & LCROSS 

Detected water in permanently shadowed craters 
2.                  Crashed part of spacecraft into crater to create plume – confirmed with other part of LCROSS 

3.                  Overall Moon is dry, so water must be remainders of asteroid and comet impacts 

12.              More recent results?? 

13.              Artemis  

Plans for human travel 
2.                  Launches a lot of small satellites 

3.                  Table of Moon Statistics 

Orbit: average distance/semi-major axis, inclination of orbit, orbital period sidereal vs. Phase cycle?  inclination of equator to orbit 
2.                  Orbit: diameter, mass, density, surface gravity, escape velocity, surface temperature, average albedo, oblateness? 

3.                  https://science.nasa.gov/moon/facts/ 

4.                  https://science.nasa.gov/moon/facts/ 

4.                  Geology of the Moon (Selenology?) 

Apollo samples 
All igneous 
2.                  Very dry -   Earth rocks 1-2% water 

3.                  Lunar maria 

Dark basalts 
2.                  Iron, manganese, titanium  dark color 

3.                  Vesicular – trapped gas bubbles – extrusive, solidified on surface, not under pressure 

4.                  2-4 byo – after the end of the late heavy bombardment 

4.                  Highlands 

Low density rocks 
2.                  Ca- Al, oxygen rich – float to the top of a melt.  

3.                  Some are Anorthosite – light color of highlands 

4.                  4-4.5 byo 

5.                  Breccia – fractured rocks fused together – repeated cratering impacts 

6.                  Regolith –  

layer of powdered rock and framents 
2.                  Maria – 10 m deep, highlands 100 md eep 

3.                  1 % is fragments of meteorites  

5.                  History of the Moon 

Formation – Large Impact 
After Earth differentiated 
2.                  Theia – Mars –size impactor  

3.                  Ejected material into orbit around the Earth – formed the Moon 

4.                  Evidence 

Low density of Moon 
2.                  Low amount of Iron 

3.                  Elemental abundances similar to Earth’s mantle 

4.                  Angular momentum 2?  of Earth-Moon System explained by glancing impact  

5.                  Moon formed without volatiles – dryness of rocks 

2.                  Magma ocean - Must have started in molten state because lower density rocks were able to float to the surface.  

3.                  Differentiation  

Low density materials crystalize and float to the top 
2.                  Denser material sink to the center and form the core 

3.                  Core, , mantle, crust 

4.                  Crust solidified 4.6-4.1 bya 

5.                  Overall Low density – core must be small 

6.                  No magnetic field – core must not be very molten now, maybe a little 

4.                  Cratering  

Cratering Rate 
Mostly constant for the last 2.5 billion years 
2.                  Late Heavy bombardment 

4.1-3.8 bya 
2.                  Clean up of solar sys formation 

3.                  Still a thing??  

2.                  Heavy bombardment – clearing up of planet formation 

Constant rain of dust, with sporadic pebble size impact 
2.                  Large impacts every few centuries 


3.                  Late heavy bombardment –  

Spike in impacts 
2.                  Planetary migration? 

3.                  Still a thing?? 

4.                  Large, multi-ring basins – Mare Imbrium, Orientale 

5.                  Mare Imbrium (get images of formation?) 

4 byo 
2.                  275 km diameter impactor 

3.                  Ejecta covered 16% of surface 

4.                  Lava flows started after LHB and filled all but the highest parts of the basin 

5.                  Very few craters on youngest flows 

6.                  Jumbled terrain – seismic waves from impact broke the other side of the Moon 

6.                  South Pole – aitkin 

Diameter 2500 km, up to 13 km deep  
2.                  No lava flows – thinner crust on Earth facing side of Moon due to tidal eddects? 

5.                  Basin flooding and modification 

4-2 billion years ago 
2.                  Lunar interior still warm.  

3.                  Melts came up through cracks and flowed over the surface 

4.                  Some basins have lava overflowed – change shape from circular 

5.                  Further crater/impact gardening (still a term?) also changes shape of basins 

6.                  Sinuous rilles – channels carved by lava (collapsed lava tubes?) 

7.                  Wrinkle ridges- weight of maria caused compression of crater 

8.                  Maria broke faults at edges??? 

9.                  Maria – multiple layers of accumulate modification – flooding, cratering, tectonics, etc. 

6.                  Cooling 

Differentiated – so must have been molten 
2.                  Cooling  

Rate of cooling proportional to surface area/volume 
Volume – amount of heat 
2.                  Surface area – amount of places heat can escape 

3.                  Cupcake cools faster than a cake 

2.                  Flow of internal heat drives surface activity – volcanism 

3.                  Moon has lost most of internal heat – surface is mostly inactive  

4.                  Compare surface activity to Moon 

7.                  Erosion 

Only modern surface acitvity  
2.                  Large mpacts – rare 

3.                  Small impacts – slow change over time.   

4.                  Solar wind 

5.                  Astronaut footprint - https://www.space.com/14740-footprints-moon.html 

2.                  Mercury 

2.                   

History & culture? 
Innermost planet – close to Sun in the sky, as seen from Earth 
2.                  Telescope observations 

1880 Schiaperelli  
Observed features on the surface 
2.                  Thought that Mercury also had synchronous rotation/ tidally locked to Earth.  

2.                  Radio observations  

1962 – found that Mercur’s dark side was warmer than it should be if permanently facing away from the Sun 
2.                  1965 Arecibo bounced radio signal off Mercury – able to measure doppler in signal – rotation period of 59 days 

3.                  Tidal connection between Sun and Moon different than tidal lock 

4.                  Resonance  

Mercury rotates 1.5 times per orbit – need image of mountain on Mercury facing away and toward Sun 
2.                  Rotation period is 2/3 of orbital period 

3.                  Resonance called 3:2   

3 rotations per 2 orbits  
2.                  Moon is 1:1 

5.                  Solar Mercury Day 

2 Mercury years or 176 days 
3.                  Spacecraft exploration 

Mariner 10 
3 flybys of Mercury in 1974 and 1975 
2.                  Did not get entire planet – get image 

3.                  Weak magnetic field 1 % of Earth’s? 

2.                  MESSENGER – spell out acronym! 

2011 –orbit insertion 
2.                  Mapped entire planet surface 

3.                  Used gravity to model the interior 

4.                  Weak magnetic field 1 % of Earth’s 

5.                  Purposely crashed on 2015 - 

Forward contamination, planetary defense 
3.                  Polar water 

Radar Arecibo data saw water at poles 
2.                  Possibly from comet impacts??? 

4.                  Mercury Geology 

Looks like the Moon –  
mostly craters with some large basins 
2.                  Some craters are very old, some are very young, rayed 

2.                  Caloris basin 

1550 km – impactor about 100 km 
2.                  Multiple rings up to 3 km high 

3.                  Caloris – latin for heat – one of two hot poles that face the sun at perihelion 

4.                  Impact threw eject up to 1000 km and cracked the opposite side of the planet (similar to imbrium on Moon) seismic waves 

5.                  Filled with lava (though not as much as Orientale and Imbrium) some from impact, some from large cracks  

3.                  Lobate scarps (not seen on Moon)  

Wrinkles  
2.                  Up to 3 km high 

3.                  Compression from cooling and contraction of planet 

4.                  Plains 

Lava flows 
Lighter color than maria on Moon, different composition???? 
2.                  Most of surface is heavily cratered 

3.                  Intercrater plains 

Lower crater density that cratered plains – these are younger than heavily cratered plains 
2.                  Craters <15 km 

3.                  Some ejecta from  large impacts 

4.                  Smooth plains 

Younger than intercrater plains 
2.                  Lava flows that occured after heavy bombardment 

3.                  Mostly near Caloris – formed soon after impact 

5.                  Mercury Interior 

Mercury density 5.43 g/cm3 - much higher than the Moon – highest among planets/moons? 
2.                  Mercury must have a metal core 

3.                  Mercury is small and should have cooled enough to solidify core, so should have no – magnetic field 

4.                  Radar images show tidal flexing of surface of Mercury during elliptical orbit = outer core must still be molten  

5.                  Sulfur could lower melting point of core, and there is a decvent amount of sulfur and other volatile compounds – what are volatiles doing that close the Sun? 

6.                  Core is very large relative to planet size – larger than predicted by regular condensation sequence 

Giant impact that stripped away some of crust and mantle? -  
reformed crust and mantle would be low on volatiles (like the Moon) 
2.                  Hollows on surface show slow sublimation of volatiles 

2.                  Inner solar nebula depleted in volatiles due to activity of young Sun 

Check recent research of planet formation? 
6.                  Mercury History 

Formation  
Inner part of nebula 
Metal rich materials 
2.                  Early impact or solar flares 

2.                  Heavy cratering 

Crater age of surface? 
2.                   Mercury gravity higher so eject travels 65% 

3.                  Inter crater plains occurred during heavy bombardment 

4.                  Near end of HB – Caloris 

5.                  Smooth plains may come from Caloris impact?? Or occurred at same (geologic) time? 

3.                  Interior cooling,  

planetary contraction = lobate scarps 
2.                  No plate tectonics 

4.                  Mostly old surface 

Micrometeorite gardening 
2.                  Larger impacts forming rayed craters  

3.                  Extreme heat and cold breaks down rocks 

3.                  Comparative Planetology: The Moon and Mercury 

Exercise – Moon or Mercury pictures 
2.                  Similarities 

Heavilty cratered surface 
2.                  Size 

3.                  Color 

4.                  Exosphere 

5.                  Volatiles in permanently shadowed craters 

3.                  Differences 

Moon density << Mercury density -> Moon weight/gravity < Mercury gravity 
2.                  Lava plains are not as dark as Maria – composition? 

3.                  Mercury orbits Sun, the Moon orbits Earth 

4.                  Mercury is close to the Sun 

5.                  Mercury has lobate scarps – moon does not (smaller core?) 

Why no lobate scarps on Earth – core still warm, has not shrunk 
6.                  Mercury does not have large, dark lava plains 

6.                  Venus and Mars 

7.                  Jupiter and Saturn – The Gas Giants 

8.                  Uranus and Neptune – The Ice Giants 

9.                  Moons 

10.              Dwarf Planets and Small Bodies 

11.              Exoplanets 

Stars 
Light 
2.                  Kepler – space telescope – not because of waveklegnth, but sensitivity 

12.              Needs a home? 

Metric units of measurement  
2.                  Perihelion, aphelion – orbits? 

13.              Extra topics 

Atoms 
Electron orbits 
Coulumb force 
2.                  Binding energy 

3.                  Quantum mechanics 

4.                  Permitted orbits 

3.                   

2.                  Gravity – Relativity 

3.                  Light –  

wavelength, frequency, amplitude 
2.                  Photon – energy equation 

3.                  Units for measuring wavelength, angstroms, etc 

4.                  Telescopes 

SOFIA – airborne telescope 
2.                  Space telescopes 

HST 
2.                  JWST 

3.                  X-ray and gamma ray 

4.                  Radio 

5.                  Telescope mounts 

6.                  Large scale mirrors – active optics 

7.                  Adaptive optics 

8.                  Interferometry 

9.                  Particle/ gravity wave 

14.              Ideas 

Compare 60’s space race with today’s 


