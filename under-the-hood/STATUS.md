# status

Current build state. Read first. Overwritten each session that ships work, resolved items deleted rather than struck through; the git log is the history. Three sections: what's done, what's next, what's open.

Active term: Fall 2026, MUS 603 (graduate).

## done

- Course outline and 15-week schedule locked (course-outline.md): six modules, weekly topics, three to four readings per week across the six-text shelf, 603 outcome traces, and the fifteen Portfolio Components mapped onto the fixed Monday calendar. Readings carry page ranges (Kolb, Rabideau, Andrews, Landry printed pages; NYFA PDF positions; McCurdy by chapter).
- The reflection and portfolio component defined and hashed out per week (course-outline.md): a prompt and a component description for each week.
- Reading core set: Kolb, NYFA, and Rabideau anchor; Andrews, Landry, and McCurdy are drawn on as assigned; Branagan removed.
- Palette chosen and shared stylesheet written (assets/style.css): warm chalk paper, pine-teal accent, DM Sans and DM Mono. Contrast checked against WCAG AA: every ink-on-surface and accent-on-surface pair in use clears 4.5:1, the lowest in use being accent on accent-soft at 5.18.
- Student-facing syllabus written and catalog-compliant (syllabus.html): all CSUEB required elements in the 601 house structure, description and outcomes verbatim from the catalog, units 3, A–F, the approved AI policy, the 65/35 split, the bibliography with verified publication data, and the schedule as six modules.
- Grade scale corrected (syllabus.html, Aug 5). The inherited MUS 111 table carried two incompatible conversions of the same 0–4 average: a GPA column and a percentage column. On a 0–4 scale a 3.0 average is 75% of points, so the GPA column read B and the percentage column read C. Dropped the percentage column, expanded the GPA column into the eleven grade-point anchors, added a worked example. The same flaw sits in the MUS 111 master and is not yet fixed there.
- Canonical internal docs scaffolded: this file, conventions.md, levels.md.
- All fifteen module pages built (week01.html through week15.html) with reading notes; weeks 1 and 4 are async (the opening week and Labor Day), week 13 is Reflection-only. The weekly spine is complete.
- Calendar shifted back one week (Aug 4 revision): week 1 runs asynchronously in the opening week (Tuesday, Aug 18 start, no Monday meeting), which pulls every week one Monday earlier and makes Fall Recess (Nov 23) a true break with no content. Async weeks are 1 and 4. Every date on every page re-verified against the 2026 calendar (Aug 10): all thirteen Mondays, all Friday component deadlines, and both Sunday async deadlines land on the weekday they claim.
- Page measure widened (Aug 10): `--measure` 46rem to 58rem with the body at 1.125rem, so the column fills a desktop screen while the line holds at roughly eighty to ninety characters. One variable drives every page; see conventions.md.
- Register sweep on the student pages (Aug 10): announcement and justification sentences cut across the syllabus and all fifteen module pages. The recurring offenders were the intro line under "the reading" that pre-summarised the citation list below it, end-of-paragraph lines announcing the reflection or component that follows in its own section, and attribution sentences standing in front of the claim they introduce.
- McCurdy ch. 4 em dash ruled on: the em dash inside "It's Not about the Money—Yet!" stays. It is the book's own title, a citation rather than prose.

## next

- Decide whether the fifteen component guides are still wanted. The weekly module pages already carry each component's definition, guiding questions, and written brief, which is what the guides were scoped to do. Building them risks two sources of truth for the same assignment.
- Canvas source: the Markdown for each week's Reflection and Portfolio Component (weekN/reflection.md, weekN/portfolio-component.md) in the two-part paste-block format, plus per-component rubrics.
- Final-portfolio landing page (HTML), including the presentation format and what the graduate implemented layer requires.
- index.html at the repo root. GitHub Pages currently serves README.md through the default theme at the site root, which puts the internal repo description in front of anyone who lands there. A short index linking the syllabus and the fifteen weeks also gives students a way in that does not depend on Canvas.
- Source charts: the chapter-by-chapter, by-subject, and subject-outcome overlay built in earlier sessions are not yet in the repo; add under under-the-hood/ if we want the analysis alongside the outline.

## open

- **Zoom link on the public syllabus.** syllabus.html publishes the personal meeting room link and ID on a public GitHub Pages site, and the ID is the office phone number. Decide whether the link moves to Canvas with the syllabus pointing there.
- **SLO 3 has no deliverable.** The outcome names résumés, cover letters, and online media. Online media is covered in week 12; no component asks for a résumé, CV, or cover letter. Andrews ch. 8 (week 4) teaches those tools, so week 4 or week 12 is where a professional-materials component would sit.
- **SLO 4's "implement" is asserted rather than assigned.** The syllabus and levels.md both promise that the graduate marketing components move past a framework into an implemented form. Every component as written produces a document. Week 12's Outreach and Platform Strategy is the natural place to require enactment (run the first stage, report what happened), or it becomes a requirement of the final.
- **Component name collision.** Week 5's Portfolio Component is called "Positionality and Access Reflection," which collides with Reflection as the locked name for the other weekly genre. The page has to spend a sentence disambiguating it. "Positionality and Access Statement" would match the other statement components.
- **Reading load spread.** New pages per week, excluding the unpaginated McCurdy chapters: week 6 is 110, week 3 is 92, week 13 is 82, against week 8 at 22 and week 2 at 26 plus a McCurdy chapter. Weeks 7, 8, and 11 look heavy on the schedule but are largely re-reads of sections already assigned.
- **Repeat readings display as errors.** NYFA ch. 11 appears in weeks 6, 7, 8, and 11; Andrews ch. 3 in 6, 7, and 11; Landry chs. 1 and 2 twice each. The module pages name the specific section each time, but the syllabus schedule line shows only the chapter number, so a student reads it as a mistake. Adding the section to the schedule line fixes it.
- **The first ten days are front-loaded.** Week 1's reflection is due Sun Aug 23, week 2's Mon Aug 24, and both components Fri Aug 28: four deliverables in six days, before anyone has been to a seminar. Moving week 1's Creative Identity Statement to Fri Sep 4 is the cheapest relief, at the cost of doubling with the Mission and Vision Statements.
- **Weighting inside the 65%.** Whether the fifteen Reflections and fifteen Components carry equal weight, or components carry more, is still undecided, and Canvas needs it before the term opens.
- **Late policy on a 0–4 scale.** The syllabus says late work takes half credit (50%), which reads as a percentage rule on a rubric that scores 0 to 4. State it as the score halved.
- Canvas grading scheme: Canvas computes percent of points earned, so a 3.0 average displays as 75% and the default scheme would post it as a C. Upload a custom scheme keyed to the anchor midpoints so the posted letter matches the syllabus: A 96.25, A– 87.5, B+ 78.75, B 71.25, B– 62.5, C+ 53.75, C 46.25, C– 37.5, D+ 28.75, D 25, F below 25. Until that is uploaded, the syllabus line saying the letter follows the scale is a promise the LMS is not keeping.
- Syllabus fill-ins for Fall 2026: office hours day and time, the final-presentation date and time, the section number, and the feedback turnaround (currently stated as within one week).
- Modality: the catalog lists on-ground; Fall 2026 runs online synchronous. Confirm the online offering is approved through scheduling.
- Fonts load from Google Fonts, so the pages are not fully offline. Decide whether to self-host DM Sans and DM Mono.
- The shared visual-language block in the project instructions still carries 302's placeholder palette; update it with this course's variables (recorded in conventions.md).
- McCurdy readings stay chapter-only: it is a reflowable ebook with no fixed pages. NYFA uses PDF page positions, taken from the real PDF's bookmarks (that digital edition has no printed folios).
- The week-folder filename convention is reflection.md / portfolio-component.md; the project-instructions example (activity-a.md / portfolio-builder.md) predates the rename and should be reconciled.
- The repo is public, which includes under-the-hood/ and reading notes/. Nothing in them is sensitive, but they are readable by anyone who finds the repo.
