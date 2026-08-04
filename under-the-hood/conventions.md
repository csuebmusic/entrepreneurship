# conventions

Editorial conventions and locked design decisions for the course. Authoritative: if something here disagrees with an earlier chat message, this file wins, and the conflict gets flagged so we reconcile it.

## the course

One course, two numbers, off one repo. MUS 603 is the graduate version; MUS 303 is the undergraduate version and satisfies GE-UD-C. Enrollment does not overlap, and the content is a shared spine. Only one number runs in a given term. The 303/603 deltas live in levels.md.

Active term: Fall 2026, MUS 603, online synchronous, Mondays 6–9pm by Zoom.

## repo layout

- Root holds the student-facing HTML (the syllabus, the weekly module pages, and later the component guides and the final-portfolio page) and the course outline (course-outline.md).
- assets/ holds style.css and images/.
- under-the-hood/ holds design-support internals: this file, STATUS.md, levels.md, and any source analysis. It is not for course content.
- Week folders (week01/ and so on) hold the Markdown source for Canvas-only items: weekN/reflection.md and weekN/portfolio-component.md. These are not rendered on the live site.
- reading notes/ holds a Markdown summary of each week's readings (weekNN.md), instructor-facing, drawn from the chapters themselves before the weekly page is drafted.

GitHub Pages serves main at the root path. There is no index page; the HTML pages are linked directly from Canvas. Pages are self-contained and browser-only.

## palette and type

Warm chalk paper with a deep pine-teal accent, chosen to sit apart from MUS 302's cream-and-rust and from the music-curriculum oxblood memo look. Reference the variables by name; never hardcode hex in page CSS.

- --bg #f4f2ec, --bg-alt #ebe7db
- --ink #23241e, --ink-soft #5c5d53
- --accent #1d6a5e, --accent-deep #16544a, --accent-soft #e1e9e4
- --rule #d8d4c9

DM Sans for body, DM Mono for labels, dates, and data. Loaded from Google Fonts with system fallbacks; the pages are not yet fully offline (see STATUS). The shared visual-language block in the project instructions still carries 302's placeholder palette and should be updated with the variables above.

## course work

- Reflection: one to two pages, written before class, engaging the week's reading and connecting it to a decision in the student's own practice. It seeds discussion and is not part of the portfolio.
- Portfolio Component: the week's durable artifact, drafted, workshopped, and revised into the final portfolio. Fifteen across the term; week 13 is reflection only.

These names are locked; they replaced "Activity A" and "Portfolio Builder." The week-folder filenames follow: reflection.md and portfolio-component.md. The project-instructions example filenames (activity-a.md, portfolio-builder.md) predate the rename and should be reconciled there.

## writing and register

The instructor's "How I want you to communicate" profile governs all student-facing and public-facing text and is airtight there: student-facing pages and feedback, repo READMEs, Canvas announcements, anything shared beyond the instructor. Process (reasoning, verification, judgment calls) stays in the between-us layer: working exchanges and the instructor-facing side of any file, which includes this file, STATUS, levels, commit messages, and the colleague breakdown on a graded item.

Style, airtight in anything student-facing or public-facing: prose, not bullet fragments, except for genuine lists. No em dashes; en dashes in number ranges are fine. Do not stack negatives; state what a thing is. Cut hedging. Do not announce what the next sentence will do. Headings stay lowercase and minimal. State the point and leave the process out.

Register shifts by level. 303 includes non-majors, so define business vocabulary (positioning, business model canvas, revenue streams, sliding scale) on first use. 603 is graduate, so assume more and push the analysis further. Either way, define each framework term the first time it appears and keep it consistent; vocabulary builds across the term.

## sourcing

Factual claims in student-facing content need grounding: industry practice, legal and financial specifics, statistics, and case-study facts about real artists and organizations. This matters most in the legal week (13) and the financial week (14). When uncertain, search before writing; if a claim cannot be sourced, drop it or flag it. Bibliographic and case-study facts come from the source itself, not from memory.

## git

Commit directly to main with the project token, one logical change per commit, descriptive multi-line messages, and push after each. For destructive or wide-reaching operations (reorganizations, mass renames, deletions), describe the plan and wait for confirmation. Commits are authored as the instructor. STATUS is current state; the git log is the historical record.

## file conventions

Student-facing durable references are HTML on the live site. Instructor-facing materials are Markdown. Canvas-only items (reflection prompts, portfolio-component assignments, discussion and quiz items) keep their Markdown source in the week folders and are copied into Canvas by hand. The weekly module pages carry the reflection and portfolio-component prompts on the page itself (see "weekly module pages" below), so the prompts live on the live site as well as in Canvas. Whether to also keep separate week-folder Markdown source for the gradable Canvas versions is open.

Instructor-facing Markdown that feeds Canvas is written in two parts: a structured top half for reading and editing (headings, rubric, outcomes addressed, level notes, internal notes), then a horizontal rule, then a "PASTE INTO CANVAS BELOW THIS LINE" block in plain prose for direct paste. Both halves carry the same substance; do not let them drift.


## weekly module pages

Each week has one HTML page, weekNN.html at the repo root, linked from Canvas. The page is comprehensive but lean, and it guides rather than spoon-feeds: the reader should leave knowing what to read, what to notice, and what to make, and should still have to do the thinking.

Build in this order: read that week's chapters from the texts, not from memory; write the summaries into reading notes/weekNN.md; then draft the page from those notes.

Page structure:
- eyebrow (week number and date), title (the week's topic), subtitle (the movement), and a one or two sentence lede.
- a weekbar: the at-a-glance line naming the reading, what is due before class, and the portfolio component.
- "this week": the framing. It poses the week's question and the tensions across the readings and points at what to notice. It does not pre-digest each chapter's argument. Define each framework term on first use.
- "the reading": a guided list. Each reading gets its citation with page range, a sentence or two on what it is and why it is here, and a mono "look for" line aimed at the part that matters most.
- "reflection": marked due before class, prompt in a callout, with a note that it does not go in the portfolio.
- "portfolio component": the component name, what it is and why it matters, guiding questions, and a short written brief in a callout. End on the brief; no closing "what a strong X is" line and no forward or next-week note.

Due dates on the page are concrete. The reflection is due before that week's Monday session; the portfolio component is due the following Friday, by 11:59 pm, on Canvas, so students build it after the seminar discussion. The two asynchronous weeks (3 and 14) have no live session; there the reflection is due the Sunday evening before the async Monday, and the component the following Friday, both on Canvas.

Leave off the page: outcome-tracing and next-week notes. Those traces live in course-outline.md and levels.md, not on the student page.

Styling: reuse the shared weekly-page components in style.css (weekbar, rd, callout, duetag, qlist) rather than adding per-page CSS.
