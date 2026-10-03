# Six junior practice stories

[Debugging lab](04-DEBUGGING-LAB.md) · [Hints — use after an attempt](06-HINTS-AND-ANSWERS.md)

These are new exercises beyond the finished reference. No story is marked complete for you. Start a branch such as practice/story-01 and write acceptance examples before editing. Each plan leaves the actual code, wording and one design choice to you.

## Story 01: Add an accessibility note

**User need:** As a learner or user of Community Notice Sheet, I want this small improvement so the behavior is easier to use, explain or verify.

**Feature boundary:** Add a short section describing the fictional entrance and quiet area using meaningful headings.

**Implementation plan:**

1. Trace `notice-copy and notice-art` and locate the smallest owning file from the code tour. Write how this story touches that responsibility.
2. Write a before/after example that demonstrates this acceptance requirement: It remains understandable without CSS and fits the existing heading hierarchy.
3. Choose the input shape, wording or layout policy yourself. Record one alternative and the reason you did not choose it.
4. Implement only the bounded change. If it crosses files, explain what each file owns rather than copying the same decision into several places.
5. Reproduce the acceptance example and one existing boundary case. Add an automated regression for executable logic, or an explicit browser/keyboard/content observation for a static change.
6. Review the diff, explain the change without reading the solution, and record remaining limits.

**Acceptance evidence:** It remains understandable without CSS and fits the existing heading hierarchy.

**Left for you:** exact fixture values, names, wording, the implementation and the tradeoff decision. Do not open the hints until you have an example and a first attempt.

**Stretch only after completion:** add one adversarial example that a plausible but incorrect solution would fail. Explain why that example is more informative than adding three ordinary examples.

## Story 02: Add a second contact method

**User need:** As a learner or user of Community Notice Sheet, I want this small improvement so the behavior is easier to use, explain or verify.

**Feature boundary:** Add a clearly labeled fictional contact link and compare it with the current email link.

**Implementation plan:**

1. Trace `notice-copy and notice-art` and locate the smallest owning file from the code tour. Write how this story touches that responsibility.
2. Write a before/after example that demonstrates this acceptance requirement: A reader understands the link purpose without nearby text.
3. Choose the input shape, wording or layout policy yourself. Record one alternative and the reason you did not choose it.
4. Implement only the bounded change. If it crosses files, explain what each file owns rather than copying the same decision into several places.
5. Reproduce the acceptance example and one existing boundary case. Add an automated regression for executable logic, or an explicit browser/keyboard/content observation for a static change.
6. Review the diff, explain the change without reading the solution, and record remaining limits.

**Acceptance evidence:** A reader understands the link purpose without nearby text.

**Left for you:** exact fixture values, names, wording, the implementation and the tradeoff decision. Do not open the hints until you have an example and a first attempt.

**Stretch only after completion:** add one adversarial example that a plausible but incorrect solution would fail. Explain why that example is more informative than adding three ordinary examples.

## Story 03: Improve the broken-image experience

**User need:** As a learner or user of Community Notice Sheet, I want this small improvement so the behavior is easier to use, explain or verify.

**Feature boundary:** Review the illustration’s alt and caption as separate jobs.

**Implementation plan:**

1. Trace `notice-copy and notice-art` and locate the smallest owning file from the code tour. Write how this story touches that responsibility.
2. Write a before/after example that demonstrates this acceptance requirement: When the image fails, essential event facts remain readable and the alt is not a filename.
3. Choose the input shape, wording or layout policy yourself. Record one alternative and the reason you did not choose it.
4. Implement only the bounded change. If it crosses files, explain what each file owns rather than copying the same decision into several places.
5. Reproduce the acceptance example and one existing boundary case. Add an automated regression for executable logic, or an explicit browser/keyboard/content observation for a static change.
6. Review the diff, explain the change without reading the solution, and record remaining limits.

**Acceptance evidence:** When the image fails, essential event facts remain readable and the alt is not a filename.

**Left for you:** exact fixture values, names, wording, the implementation and the tradeoff decision. Do not open the hints until you have an example and a first attempt.

**Stretch only after completion:** add one adversarial example that a plausible but incorrect solution would fail. Explain why that example is more informative than adding three ordinary examples.

## Story 04: Handle a longer venue name

**User need:** As a learner or user of Community Notice Sheet, I want this small improvement so the behavior is easier to use, explain or verify.

**Feature boundary:** Add a long realistic location and adjust only the layout rules that need changing.

**Implementation plan:**

1. Trace `notice-copy and notice-art` and locate the smallest owning file from the code tour. Write how this story touches that responsibility.
2. Write a before/after example that demonstrates this acceptance requirement: Desktop and 320px views have no clipped text or document-level horizontal scrolling.
3. Choose the input shape, wording or layout policy yourself. Record one alternative and the reason you did not choose it.
4. Implement only the bounded change. If it crosses files, explain what each file owns rather than copying the same decision into several places.
5. Reproduce the acceptance example and one existing boundary case. Add an automated regression for executable logic, or an explicit browser/keyboard/content observation for a static change.
6. Review the diff, explain the change without reading the solution, and record remaining limits.

**Acceptance evidence:** Desktop and 320px views have no clipped text or document-level horizontal scrolling.

**Left for you:** exact fixture values, names, wording, the implementation and the tradeoff decision. Do not open the hints until you have an example and a first attempt.

**Stretch only after completion:** add one adversarial example that a plausible but incorrect solution would fail. Explain why that example is more informative than adding three ordinary examples.

## Story 05: Create a print-friendly notice

**User need:** As a learner or user of Community Notice Sheet, I want this small improvement so the behavior is easier to use, explain or verify.

**Feature boundary:** Add a small print stylesheet that keeps the event facts clear on one page.

**Implementation plan:**

1. Trace `notice-copy and notice-art` and locate the smallest owning file from the code tour. Write how this story touches that responsibility.
2. Write a before/after example that demonstrates this acceptance requirement: A print preview includes date, place and contact without depending on background colors.
3. Choose the input shape, wording or layout policy yourself. Record one alternative and the reason you did not choose it.
4. Implement only the bounded change. If it crosses files, explain what each file owns rather than copying the same decision into several places.
5. Reproduce the acceptance example and one existing boundary case. Add an automated regression for executable logic, or an explicit browser/keyboard/content observation for a static change.
6. Review the diff, explain the change without reading the solution, and record remaining limits.

**Acceptance evidence:** A print preview includes date, place and contact without depending on background colors.

**Left for you:** exact fixture values, names, wording, the implementation and the tradeoff decision. Do not open the hints until you have an example and a first attempt.

**Stretch only after completion:** add one adversarial example that a plausible but incorrect solution would fail. Explain why that example is more informative than adding three ordinary examples.

## Story 06: Compare two width allocations

**User need:** As a learner or user of Community Notice Sheet, I want this small improvement so the behavior is easier to use, explain or verify.

**Feature boundary:** Try a different copy/illustration ratio and write a short decision note.

**Implementation plan:**

1. Trace `notice-copy and notice-art` and locate the smallest owning file from the code tour. Write how this story touches that responsibility.
2. Write a before/after example that demonstrates this acceptance requirement: Explain what changed in the computed boxes and why the resulting balance helps the actual content.
3. Choose the input shape, wording or layout policy yourself. Record one alternative and the reason you did not choose it.
4. Implement only the bounded change. If it crosses files, explain what each file owns rather than copying the same decision into several places.
5. Reproduce the acceptance example and one existing boundary case. Add an automated regression for executable logic, or an explicit browser/keyboard/content observation for a static change.
6. Review the diff, explain the change without reading the solution, and record remaining limits.

**Acceptance evidence:** Explain what changed in the computed boxes and why the resulting balance helps the actual content.

**Left for you:** exact fixture values, names, wording, the implementation and the tradeoff decision. Do not open the hints until you have an example and a first attempt.

**Stretch only after completion:** add one adversarial example that a plausible but incorrect solution would fail. Explain why that example is more informative than adding three ordinary examples.

<!-- expanded-story-clinics -->

## Additional planning checkpoints for stories 01–06

[Nine more stories, 07–15](11-NINE-MORE-STORIES.md) · [Expanded workshop map](WORKBOOK-INDEX.md)

Keep the original plans above. The following checkpoints add implementation and review depth without completing the exercise for you.

### Story 01 planning clinic: Add an accessibility note

**Before editing:** restate the boundary in your own words: Add a short section describing the fictional entrance and quiet area using meaningful headings. Identify the part of `public/index.html` or `public/index.html and public/style.css` that owns it. If your proposed design changes another owner, explain the dependency instead of opening every file for a broad rewrite.

**Acceptance matrix:** write ordinary, boundary and repeat/recovery rows that establish “It remains understandable without CSS and fits the existing heading hierarchy.” Include exact starting data or content and the expected retained information. Calculate expected values or inspect meaningful source order independently of the proposed implementation.

**First implementation slice:** make only enough of the change to demonstrate one acceptance row. Inspect the diff and predict the next row before running it. If your first slice is mostly setup or abstraction with no observable result, consider a smaller direct route.

**Review challenge:** sketch a plausible wrong solution that would pass a casual demonstration. Choose a counterexample that exposes its specific weakness. Ask an assistant to critique that example rather than immediately asking it to finish the entire feature.

**Evidence and explanation:** use npm test (local asset references), plus the relevant browser/content observation. Record the actual observation and the limit of the check. Finish by naming a design decision you made yourself and explaining why the neighboring original behavior still holds.

### Story 02 planning clinic: Add a second contact method

**Before editing:** restate the boundary in your own words: Add a clearly labeled fictional contact link and compare it with the current email link. Identify the part of `public/index.html` or `public/index.html and public/style.css` that owns it. If your proposed design changes another owner, explain the dependency instead of opening every file for a broad rewrite.

**Acceptance matrix:** write ordinary, boundary and repeat/recovery rows that establish “A reader understands the link purpose without nearby text.” Include exact starting data or content and the expected retained information. Calculate expected values or inspect meaningful source order independently of the proposed implementation.

**First implementation slice:** make only enough of the change to demonstrate one acceptance row. Inspect the diff and predict the next row before running it. If your first slice is mostly setup or abstraction with no observable result, consider a smaller direct route.

**Review challenge:** sketch a plausible wrong solution that would pass a casual demonstration. Choose a counterexample that exposes its specific weakness. Ask an assistant to critique that example rather than immediately asking it to finish the entire feature.

**Evidence and explanation:** use npm test (local asset references), plus the relevant browser/content observation. Record the actual observation and the limit of the check. Finish by naming a design decision you made yourself and explaining why the neighboring original behavior still holds.

### Story 03 planning clinic: Improve the broken-image experience

**Before editing:** restate the boundary in your own words: Review the illustration’s alt and caption as separate jobs. Identify the part of `public/index.html` or `public/index.html and public/style.css` that owns it. If your proposed design changes another owner, explain the dependency instead of opening every file for a broad rewrite.

**Acceptance matrix:** write ordinary, boundary and repeat/recovery rows that establish “When the image fails, essential event facts remain readable and the alt is not a filename.” Include exact starting data or content and the expected retained information. Calculate expected values or inspect meaningful source order independently of the proposed implementation.

**First implementation slice:** make only enough of the change to demonstrate one acceptance row. Inspect the diff and predict the next row before running it. If your first slice is mostly setup or abstraction with no observable result, consider a smaller direct route.

**Review challenge:** sketch a plausible wrong solution that would pass a casual demonstration. Choose a counterexample that exposes its specific weakness. Ask an assistant to critique that example rather than immediately asking it to finish the entire feature.

**Evidence and explanation:** use npm test (local asset references), plus the relevant browser/content observation. Record the actual observation and the limit of the check. Finish by naming a design decision you made yourself and explaining why the neighboring original behavior still holds.

### Story 04 planning clinic: Handle a longer venue name

**Before editing:** restate the boundary in your own words: Add a long realistic location and adjust only the layout rules that need changing. Identify the part of `public/index.html` or `public/index.html and public/style.css` that owns it. If your proposed design changes another owner, explain the dependency instead of opening every file for a broad rewrite.

**Acceptance matrix:** write ordinary, boundary and repeat/recovery rows that establish “Desktop and 320px views have no clipped text or document-level horizontal scrolling.” Include exact starting data or content and the expected retained information. Calculate expected values or inspect meaningful source order independently of the proposed implementation.

**First implementation slice:** make only enough of the change to demonstrate one acceptance row. Inspect the diff and predict the next row before running it. If your first slice is mostly setup or abstraction with no observable result, consider a smaller direct route.

**Review challenge:** sketch a plausible wrong solution that would pass a casual demonstration. Choose a counterexample that exposes its specific weakness. Ask an assistant to critique that example rather than immediately asking it to finish the entire feature.

**Evidence and explanation:** use npm test (local asset references), plus the relevant browser/content observation. Record the actual observation and the limit of the check. Finish by naming a design decision you made yourself and explaining why the neighboring original behavior still holds.

### Story 05 planning clinic: Create a print-friendly notice

**Before editing:** restate the boundary in your own words: Add a small print stylesheet that keeps the event facts clear on one page. Identify the part of `public/index.html` or `public/index.html and public/style.css` that owns it. If your proposed design changes another owner, explain the dependency instead of opening every file for a broad rewrite.

**Acceptance matrix:** write ordinary, boundary and repeat/recovery rows that establish “A print preview includes date, place and contact without depending on background colors.” Include exact starting data or content and the expected retained information. Calculate expected values or inspect meaningful source order independently of the proposed implementation.

**First implementation slice:** make only enough of the change to demonstrate one acceptance row. Inspect the diff and predict the next row before running it. If your first slice is mostly setup or abstraction with no observable result, consider a smaller direct route.

**Review challenge:** sketch a plausible wrong solution that would pass a casual demonstration. Choose a counterexample that exposes its specific weakness. Ask an assistant to critique that example rather than immediately asking it to finish the entire feature.

**Evidence and explanation:** use npm test (local asset references), plus the relevant browser/content observation. Record the actual observation and the limit of the check. Finish by naming a design decision you made yourself and explaining why the neighboring original behavior still holds.

### Story 06 planning clinic: Compare two width allocations

**Before editing:** restate the boundary in your own words: Try a different copy/illustration ratio and write a short decision note. Identify the part of `public/index.html` or `public/index.html and public/style.css` that owns it. If your proposed design changes another owner, explain the dependency instead of opening every file for a broad rewrite.

**Acceptance matrix:** write ordinary, boundary and repeat/recovery rows that establish “Explain what changed in the computed boxes and why the resulting balance helps the actual content.” Include exact starting data or content and the expected retained information. Calculate expected values or inspect meaningful source order independently of the proposed implementation.

**First implementation slice:** make only enough of the change to demonstrate one acceptance row. Inspect the diff and predict the next row before running it. If your first slice is mostly setup or abstraction with no observable result, consider a smaller direct route.

**Review challenge:** sketch a plausible wrong solution that would pass a casual demonstration. Choose a counterexample that exposes its specific weakness. Ask an assistant to critique that example rather than immediately asking it to finish the entire feature.

**Evidence and explanation:** use npm test (local asset references), plus the relevant browser/content observation. Record the actual observation and the limit of the check. Finish by naming a design decision you made yourself and explaining why the neighboring original behavior still holds.
