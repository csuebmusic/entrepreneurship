# conventions

Editorial conventions and locked design decisions for the course. Authoritative: if something here disagrees with an earlier chat message, this file wins, and the conflict gets flagged so we reconcile it.

## the course

One course, two numbers, off one repo. MUS 603 is the graduate version; MUS 303 is the undergraduate version and satisfies GE-UD-C. Enrollment does not overlap, and the content is a shared spine. Only one number runs in a given term. The 303/603 deltas live in levels.md.

Active term: Fall 2026, MUS 603, online synchronous, Mondays 6–9pm by Zoom.

## repo layout

- Root holds the student-facing HTML (the syllabus, the weekly module pages, and the final-portfolio page) and the course outline (course-outline.md). There are no separate component guides: each weekly module page carries its component's definition, guiding questions, and brief.
- assets/ holds style.css and images/.
- under-the-hood/ holds design-support internals: this file, STATUS.md, levels.md, and any source analysis. It is not for course content.
- reading notes/ holds a Markdown summary of each week's readings (weekNN.md), instructor-facing, drawn from the chapters themselves before the weekly page is drafted.
- README.md is the instructor's index: the current list of student-facing links for copying into Canvas, plus the layout. Update it whenever a student-facing page is added or renamed.

GitHub Pages serves main at the root path. There is no index page; the HTML pages are linked directly from Canvas. Pages are self-contained and browser-only.

The repository is public, which includes under-the-hood/ and reading notes/. Keep anything sensitive out of it.

No student information goes in the repository: no names, no submitted work, no grades or feedback, no enrollment or accommodation details. Student material stays in Canvas.

## palette and type

Warm chalk paper with a deep pine-teal accent, chosen to sit apart from MUS 302's cream-and-rust and from the music-curriculum oxblood memo look. Reference the variables by name; never hardcode hex in page CSS.

- --bg #f4f2ec, --bg-alt #ebe7db
- --ink #23241e, --ink-soft #5c5d53
- --accent #1d6a5e, --accent-deep #16544a, --accent-soft #e1e9e4
- --rule #d8d4c9

Every ink-on-surface and accent-on-surface pair in use clears WCAG AA at 4.5:1. Check any new pair before adding it.

DM Sans for body, DM Mono for labels, dates, and data. Loaded from Google Fonts with system fallbacks. The pages are not fully offline.

Page width is one variable, `--measure` (58rem), with the body size (1.125rem) tuned to it so the line holds at roughly eighty to ninety characters. Change `--measure` alone to widen or narrow every page at once; raising it much past 60rem without also raising the body size pushes the line past a comfortable length. Below 620px the body drops back to 1.0625rem.

## course work

- Reflection: one to two pages, written before class, engaging the week's reading and connecting it to a decision in the student's own practice. It seeds discussion and is not part of the portfolio. Fourteen across the term; week 4 has none.
- Portfolio Component: the week's durable artifact, drafted, workshopped, and revised into the final portfolio. Seventeen across the term; week 3 produces two and week 4 produces three. Week 13 is reflection only, and week 4 is components only.

These names are locked.

Weekly Reflections and Portfolio Components carry 65% of the course grade and the final portfolio and presentation 35%. Inside the 65%, every Reflection and every Component carries equal weight. Assessment detail, the 0 to 4 anchors, and the Canvas grading scheme live in course-outline.md.

## writing and register

The instructor's "how I want you to communicate" profile governs three layers by destination. Process (reasoning, verification, judgment calls) belongs in chat with her and nowhere else. Instructor-facing files, which include this file, STATUS, levels, commit messages, and the colleague breakdown on a graded item, record state and rules rather than deliberation: the decision, the rule, the current status, the open question, without why the rule was chosen or what was weighed against it. Student-facing and public-facing text carries no process and no justification, and the style rules below are airtight there.

Style, airtight in anything student-facing or public-facing: prose, not bullet fragments, except for genuine lists. No em dashes; en dashes in number ranges are fine. An em dash inside a cited title stays, since the title is a citation rather than prose. Do not stack negatives; state what a thing is. Cut hedging filler, keeping real qualification where a claim is genuinely uncertain or contested. Do not announce what the next sentence will do or restate what the last one delivered. Do not justify: state the requirement, the fact, or the point, and stop, without explaining why a requirement is set as it is or what a design choice accomplishes. Headings stay lowercase and minimal. State the point and leave the process out.

Register shifts by level. 303 includes non-majors, so define business vocabulary (positioning, business model canvas, revenue streams, sliding scale) on first use. 603 is graduate, so assume more and push the analysis further. Either way, define each framework term the first time it appears and keep it consistent; vocabulary builds across the term.

## sourcing

Factual claims in student-facing content need grounding: industry practice, legal and financial specifics, statistics, and case-study facts about real artists and organizations. This matters most in the legal week (13) and the financial week (14). When uncertain, search before writing; if a claim cannot be sourced, drop it or flag it. Bibliographic and case-study facts come from the source itself, not from memory.

## git

Commit directly to main with the project token, one logical change per commit, descriptive multi-line messages, and push after each. For destructive or wide-reaching operations (reorganizations, mass renames, deletions), describe the plan and wait for confirmation. Commits are authored as the instructor. STATUS is current state; the git log is the historical record.

## file conventions

Student-facing durable references are HTML on the live site. Instructor-facing materials are Markdown.

The weekly module page is the single source for a week's Reflection prompt and Portfolio Component brief. There is no parallel Markdown source for Canvas: the prompts are copied into Canvas from the page. Two rubrics cover all weekly work, one for Reflections and one for Portfolio Components. They live in course-outline.md. There are no per-component rubrics.


## weekly module pages

Each week has one HTML page, weekNN.html at the repo root, linked from Canvas. The page is comprehensive but lean, and it guides rather than spoon-feeds: the reader should leave knowing what to read, what to notice, and what to make, and should still have to do the thinking.

Build in this order: read that week's chapters from the texts, not from memory; write the summaries into reading notes/weekNN.md; then draft the page from those notes.

When a chapter is assigned in more than one week, cite the section rather than the chapter, in the outline, in the syllabus schedule, and on the module page. Give the printed sub-range for Kolb, Rabideau, Andrews, and Landry. NYFA's digital edition has no printed folios: its ranges are positions in the course PDF, and a partial chapter names the section alone. McCurdy is a reflowable ebook with no fixed pages and is cited chapter-only.

Page structure:
- eyebrow (week number and date), title (the week's topic), subtitle (the module), and a one or two sentence lede.
- a weekbar: the at-a-glance line naming the reading, what is due before class, and the portfolio component.
- "this week": the framing. It poses the week's question and the tensions across the readings and points at what to notice. It does not pre-digest each chapter's argument. Define each framework term on first use.
- "the reading": a guided list. Each reading gets its citation with page range, a sentence or two on what it is and why it is here, and a mono "look for" line aimed at the part that matters most.
- "reflection": marked due before class, prompt in a callout, with a note that it does not go in the portfolio.
- "portfolio component": the component name, what it is and why it matters, guiding questions, and a short written brief in a callout. End on the brief; no closing "what a strong X is" line and no forward or next-week note.

Due dates on the page are concrete. The reflection is due before that week's Monday session; the portfolio component is due the following Friday, by 11:59 pm, on Canvas, so students build it after the seminar discussion. The two asynchronous weeks (1 and 4) have no live session; there the reflection is due the Sunday evening before, and the component the following Friday, both on Canvas.

Leave off the page: outcome-tracing and next-week notes. Those traces live in course-outline.md and levels.md, not on the student page.

Styling: reuse the shared weekly-page components in style.css (weekbar, rd, callout, duetag, qlist) rather than adding per-page CSS.
