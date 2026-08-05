# status

Current build state. Read first. Overwritten each session that ships work, resolved items deleted rather than struck through; the git log is the history. Three sections: what's done, what's next, what's open.

Active term: Fall 2026, MUS 603 (graduate).

## done

- Course outline and 15-week schedule locked (course-outline.md): six modules, weekly topics, three to four readings per week across the six-text shelf, 603 outcome traces, and the fifteen Portfolio Components mapped onto the fixed Monday calendar. Readings carry page ranges (Kolb, Rabideau, Andrews, Landry printed pages; NYFA PDF positions; McCurdy by chapter).
- The reflection and portfolio component defined and hashed out per week (course-outline.md): a prompt and a component description for each week.
- Reading core set: Kolb, NYFA, and Rabideau anchor; Andrews, Landry, and McCurdy are drawn on as assigned; Branagan removed.
- Palette chosen and shared stylesheet written (assets/style.css): warm chalk paper, pine-teal accent, DM Sans and DM Mono.
- Student-facing syllabus written and catalog-compliant (syllabus.html): all CSUEB required elements in the 601 house structure, description and outcomes verbatim from the catalog, units 3, A–F, the approved AI policy, the 65/35 split, the bibliography with verified publication data, and the schedule as six modules.
- Canonical internal docs scaffolded: this file, conventions.md, levels.md.
- All fifteen module pages built (week01.html through week15.html) with reading notes; weeks 1 and 4 are async (the opening week and Labor Day), week 13 is Reflection-only. The weekly spine is complete.
- Calendar shifted back one week (Aug 4 revision): week 1 now runs asynchronously in the opening week (Tuesday, Aug 18 start, no Monday meeting), which pulls every week one Monday earlier and makes Fall Recess (Nov 23) a true break with no content. Async weeks are now 1 and 4; weeks 3 and 14 became live. Week 15 unchanged (Nov 30). Dates updated across all pages, the syllabus, the outline, and conventions. This resolved the old Thanksgiving-Friday due date. Week 1: reflection due Sun Aug 23, component due Fri Aug 28 (falls together with week 2, which is light). Note: week10.html carries one em dash inside McCurdy ch.4's real title "It's Not about the Money—Yet!" (a faithful citation, not prose). Week 5 uses two sourced, open-access outside readings (Goldin & Rouse 2000; Panic! 2018) alongside Rabideau 7.

## next

- Component guides: the HTML pages that teach each concept while doing the component. Fifteen of them.
- Weekly module pages: complete (weeks 1 to 15). Next build targets: the fifteen component guides (HTML), the final-portfolio landing page, and the Canvas source md plus rubrics.
- Canvas source: the Markdown for each week's Reflection and Portfolio Component (weekN/reflection.md, weekN/portfolio-component.md) in the two-part paste-block format, plus per-component rubrics.
- Week 5 outside readings: assemble and source the scholarly and industry set for the power-and-identity week.
- Final-portfolio landing page (HTML).
- Source charts: the chapter-by-chapter, by-subject, and subject-outcome overlay built in earlier sessions are not yet in the repo; add under under-the-hood/ if we want the analysis alongside the outline.

## open

- Module labels: "movement" relabeled to "module" across the site and notes. Six modules (I to VI) confirmed by Ines. Roman numerals kept; Arabic (Module 1 to 6) available if preferred later.
- Syllabus fill-ins for Fall 2026: office hours day and time, the final-presentation date and time, the section number, and the feedback turnaround (currently stated as within one week).
- Modality: the catalog lists on-ground; Fall 2026 runs online synchronous. Confirm the online offering is approved through scheduling.
- Fonts load from Google Fonts, so the pages are not fully offline. Decide whether to self-host DM Sans and DM Mono.
- The shared visual-language block in the project instructions still carries 302's placeholder palette; update it with this course's variables (recorded in conventions.md).
- McCurdy readings stay chapter-only: it is a reflowable ebook with no fixed pages. NYFA now uses PDF page positions, taken from the real PDF's bookmarks (that digital edition has no printed folios).
- The week-folder filename convention is reflection.md / portfolio-component.md; the project-instructions example (activity-a.md / portfolio-builder.md) predates the rename and should be reconciled.
