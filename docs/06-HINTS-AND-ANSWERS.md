# Hints and answer directions

[Return to the stories](05-PRACTICE-STORIES.md)

There are intentionally no complete feature patches here. Use one hint, return to your code and produce evidence. Your design can differ from the reference when you state and verify the new contract.

## Story 01: Add an accessibility note

**Hint 1 — ownership:** Begin from the section and heading structure in `public/index.html`. Add a short section describing the fictional entrance and quiet area using meaningful headings.

**Hint 2 — reasoning:** Revisit the decision “Choose HTML by meaning”. Ask yourself: Identify which facts should still be readable if every style rule disappears.

**Answer direction:** A defensible solution demonstrates this observable result: It remains understandable without CSS and fits the existing heading hierarchy. The exact code is not prescribed. If your change achieves that result by changing an unrelated original rule, revise either the implementation or the story contract explicitly.

**Self-review:** Could the UI or helper appear correct while the underlying rule remains wrong? Could the underlying calculation be correct while stale presentation misleads the user? Choose the question that applies and write one distinguishing example.

## Story 02: Add a second contact method

**Hint 1 — ownership:** Begin from the email link inside `.notice-copy`. Add a clearly labeled fictional contact link and compare it with the current email link.

**Hint 2 — reasoning:** Revisit the decision “Choose HTML by meaning”. Ask yourself: Identify which facts should still be readable if every style rule disappears.

**Answer direction:** A defensible solution demonstrates this observable result: A reader understands the link purpose without nearby text. The exact code is not prescribed. If your change achieves that result by changing an unrelated original rule, revise either the implementation or the story contract explicitly.

**Self-review:** Could the UI or helper appear correct while the underlying rule remains wrong? Could the underlying calculation be correct while stale presentation misleads the user? Choose the question that applies and write one distinguishing example.

## Story 03: Improve the broken-image experience

**Hint 1 — ownership:** Begin from `figure.notice-art` in `public/index.html`. Review the illustration’s alt and caption as separate jobs.

**Hint 2 — reasoning:** Revisit the decision “Choose HTML by meaning”. Ask yourself: Identify which facts should still be readable if every style rule disappears.

**Answer direction:** A defensible solution demonstrates this observable result: When the image fails, essential event facts remain readable and the alt is not a filename. The exact code is not prescribed. If your change achieves that result by changing an unrelated original rule, revise either the implementation or the story contract explicitly.

**Self-review:** Could the UI or helper appear correct while the underlying rule remains wrong? Could the underlying calculation be correct while stale presentation misleads the user? Choose the question that applies and write one distinguishing example.

## Story 04: Handle a longer venue name

**Hint 1 — ownership:** Begin from the `.notice-copy` width and the 650px rule in `public/style.css`. Add a long realistic location and adjust only the layout rules that need changing.

**Hint 2 — reasoning:** Revisit the decision “Let narrow content stack”. Ask yourself: Choose a different breakpoint based on a visible content failure, not a device brand.

**Answer direction:** A defensible solution demonstrates this observable result: Desktop and 320px views have no clipped text or document-level horizontal scrolling. The exact code is not prescribed. If your change achieves that result by changing an unrelated original rule, revise either the implementation or the story contract explicitly.

**Self-review:** Could the UI or helper appear correct while the underlying rule remains wrong? Could the underlying calculation be correct while stale presentation misleads the user? Choose the question that applies and write one distinguishing example.

## Story 05: Create a print-friendly notice

**Hint 1 — ownership:** Begin from `public/style.css`. Add a small print stylesheet that keeps the event facts clear on one page.

**Hint 2 — reasoning:** Revisit the decision “Choose HTML by meaning”. Ask yourself: Identify which facts should still be readable if every style rule disappears.

**Answer direction:** A defensible solution demonstrates this observable result: A print preview includes date, place and contact without depending on background colors. The exact code is not prescribed. If your change achieves that result by changing an unrelated original rule, revise either the implementation or the story contract explicitly.

**Self-review:** Could the UI or helper appear correct while the underlying rule remains wrong? Could the underlying calculation be correct while stale presentation misleads the user? Choose the question that applies and write one distinguishing example.

## Story 06: Compare two width allocations

**Hint 1 — ownership:** Begin from `notice-copy and notice-art`. Try a different copy/illustration ratio and write a short decision note.

**Hint 2 — reasoning:** Revisit the decision “Keep the assignment’s inline-block constraint”. Ask yourself: Explain why two 50% inline-block boxes can unexpectedly wrap.

**Answer direction:** A defensible solution demonstrates this observable result: Explain what changed in the computed boxes and why the resulting balance helps the actual content. The exact code is not prescribed. If your change achieves that result by changing an unrelated original rule, revise either the implementation or the story contract explicitly.

**Self-review:** Could the UI or helper appear correct while the underlying rule remains wrong? Could the underlying calculation be correct while stale presentation misleads the user? Choose the question that applies and write one distinguishing example.

## Answers to the trace questions

HTML declares the announcement and its heading → the browser gives elements their normal flow → .notice-copy and .notice-art become inline-block boxes → percentage widths reserve room for whitespace → the 650px rule stacks the boxes.

The expected examples are in the concepts table. Use them to check your reasoning, then supply a new example of your own. A copied sentence is not evidence that you can trace a changed input.

## When to ask for more help

Ask after you can show a concrete attempt, a specific uncertainty and an observation. Request a smaller hint before a full patch. If you do accept generated code, explain each changed line and run a counterexample you chose independently.
