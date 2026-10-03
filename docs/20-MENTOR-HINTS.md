# M002: mentor hints and answer directions

[Expanded workshop map](WORKBOOK-INDEX.md) · [Repository overview](../README.md)

Use this chapter after making an attempt. It provides reasoning directions and evaluation criteria, not finished feature patches. A learner can choose a different design when the revised contract is explicit and the evidence supports it.

## Retrieval card 01: answer direction

**Question:** Explain semantic element through this project

Markup selected for meaning, such as a heading or time.

Look for a concrete connection to `public/index.html` or `public/index.html and public/style.css`. A strong answer names an input or condition, the responsible operation and the resulting behavior. Merely repeating the vocabulary word is insufficient. If your example differs from the reference, check whether it is supported by the contract before treating a different outcome as a defect.

## Retrieval card 02: answer direction

**Question:** Explain border box through this project

A declared width that includes padding and border.

Look for a concrete connection to `public/index.html` or `public/index.html and public/style.css`. A strong answer names an input or condition, the responsible operation and the resulting behavior. Merely repeating the vocabulary word is insufficient. If your example differs from the reference, check whether it is supported by the contract before treating a different outcome as a defect.

## Retrieval card 03: answer direction

**Question:** Explain inline whitespace through this project

Space between inline-level boxes that can consume horizontal room.

Look for a concrete connection to `public/index.html` or `public/index.html and public/style.css`. A strong answer names an input or condition, the responsible operation and the resulting behavior. Merely repeating the vocabulary word is insufficient. If your example differs from the reference, check whether it is supported by the contract before treating a different outcome as a defect.

## Retrieval card 04: answer direction

**Question:** Explain alternative text through this project

A useful textual replacement for an image's information.

Look for a concrete connection to `public/index.html` or `public/index.html and public/style.css`. A strong answer names an input or condition, the responsible operation and the resulting behavior. Merely repeating the vocabulary word is insufficient. If your example differs from the reference, check whether it is supported by the contract before treating a different outcome as a defect.

## Retrieval card 05: answer direction

**Question:** Predict: Desktop width

Text and illustration sit side by side

Look for a concrete connection to `public/index.html` or `public/index.html and public/style.css`. A strong answer names an input or condition, the responsible operation and the resulting behavior. Merely repeating the vocabulary word is insufficient. If your example differs from the reference, check whether it is supported by the contract before treating a different outcome as a defect.

## Retrieval card 06: answer direction

**Question:** Predict: 320px width

The columns stack without horizontal page scrolling

Look for a concrete connection to `public/index.html` or `public/index.html and public/style.css`. A strong answer names an input or condition, the responsible operation and the resulting behavior. Merely repeating the vocabulary word is insufficient. If your example differs from the reference, check whether it is supported by the contract before treating a different outcome as a defect.

## Retrieval card 07: answer direction

**Question:** Predict: notice.svg missing

The informative alt text still describes the illustration

Look for a concrete connection to `public/index.html` or `public/index.html and public/style.css`. A strong answer names an input or condition, the responsible operation and the resulting behavior. Merely repeating the vocabulary word is insufficient. If your example differs from the reference, check whether it is supported by the contract before treating a different outcome as a defect.

## Retrieval card 08: answer direction

**Question:** Identify which facts should still be readable if every style rule disappears.

The date uses time, the illustration uses figure and figcaption, and the notice has a real heading. Choosing these elements first keeps information available independently of the visual arrangement.

Look for a concrete connection to `public/index.html` or `public/index.html and public/style.css`. A strong answer names an input or condition, the responsible operation and the resulting behavior. Merely repeating the vocabulary word is insufficient. If your example differs from the reference, check whether it is supported by the contract before treating a different outcome as a defect.

## Retrieval card 09: answer direction

**Question:** Explain why two 50% inline-block boxes can unexpectedly wrap.

This constraint is educational rather than a claim that inline-block is the universal modern layout choice. Widths of 55% and 40% leave space for inline whitespace. Border-box keeps padding within the declared widths.

Look for a concrete connection to `public/index.html` or `public/index.html and public/style.css`. A strong answer names an input or condition, the responsible operation and the resulting behavior. Merely repeating the vocabulary word is insufficient. If your example differs from the reference, check whether it is supported by the contract before treating a different outcome as a defect.

## Retrieval card 10: answer direction

**Question:** Choose a different breakpoint based on a visible content failure, not a device brand.

A small screen benefits from ordinary block flow rather than shrinking both columns indefinitely. The responsive rule changes layout while preserving the same content and source order.

Look for a concrete connection to `public/index.html` or `public/index.html and public/style.css`. A strong answer names an input or condition, the responsible operation and the resulting behavior. Merely repeating the vocabulary word is insufficient. If your example differs from the reference, check whether it is supported by the contract before treating a different outcome as a defect.

## Retrieval card 11: answer direction

**Question:** What does your strongest check not prove?

Use the scope recorded in VERIFICATION.md; do not infer production readiness from a small local fixture.

Look for a concrete connection to `public/index.html` or `public/index.html and public/style.css`. A strong answer names an input or condition, the responsible operation and the resulting behavior. Merely repeating the vocabulary word is insufficient. If your example differs from the reference, check whether it is supported by the contract before treating a different outcome as a defect.

## Retrieval card 12: answer direction

**Question:** Which parts remain understandable when the stylesheet is disabled?

Treat the notice as useful information that happens to have a layout. First preserve the questions a visitor asks: what is happening, when, where and how to contact someone. Then reason about rectangles, padding and inline whitespace. If a style experiment makes the venue impossible to read, the experiment has violated the content contract even when the screenshot looks cleaner.

Look for a concrete connection to `public/index.html` or `public/index.html and public/style.css`. A strong answer names an input or condition, the responsible operation and the resulting behavior. Merely repeating the vocabulary word is insufficient. If your example differs from the reference, check whether it is supported by the contract before treating a different outcome as a defect.

## Story 07: Add a rainy-day note

**First hint:** The desired improvement is “Clarify an alternate fictional venue.” Start by identifying which existing boundary already knows the necessary information. Do not copy that information into new state until you can explain why derivation is insufficient.

**Second hint:** Follow this source-specific route: Add ordinary text near the location; use a meaningful subheading; check its order without styles.. Keep each stage independently inspectable. If a step requires a policy choice, write the choice before implementing it.

**Third hint:** Your strongest completion evidence should establish: Both venues and the condition for using each remain readable at 320px.. Invent a plausible wrong implementation and make your example disagree with it.

**Decision still left to you:** Choose wording that avoids ambiguity. The guide intentionally does not settle this. Evaluate your answer by clarity of the contract, consistency of the implementation and quality of verification, not by guessing the author's preferred wording.

## Story 08: Add a short preparation list

**First hint:** The desired improvement is “Tell visitors what to do before arriving.” Start by identifying which existing boundary already knows the necessary information. Do not copy that information into new state until you can explain why derivation is insufficient.

**Second hint:** Follow this source-specific route: Group related instructions in a list; keep event facts outside the illustration; inspect spacing and source order.. Keep each stage independently inspectable. If a step requires a policy choice, write the choice before implementing it.

**Third hint:** Your strongest completion evidence should establish: List meaning survives disabled CSS and keyboard users can reach any links.. Invent a plausible wrong implementation and make your example disagree with it.

**Decision still left to you:** Choose three fictional preparations. The guide intentionally does not settle this. Evaluate your answer by clarity of the contract, consistency of the implementation and quality of verification, not by guessing the author's preferred wording.

## Story 09: Show event duration explicitly

**First hint:** The desired improvement is “Avoid asking visitors to calculate the time span.” Start by identifying which existing boundary already knows the necessary information. Do not copy that information into new state until you can explain why derivation is insufficient.

**Second hint:** Follow this source-specific route: Add a duration sentence; verify it matches the fictional start and end times; inspect print preview.. Keep each stage independently inspectable. If a step requires a policy choice, write the choice before implementing it.

**Third hint:** Your strongest completion evidence should establish: The duration and visible times agree in both screen and print views.. Invent a plausible wrong implementation and make your example disagree with it.

**Decision still left to you:** Choose a concise duration format. The guide intentionally does not settle this. Evaluate your answer by clarity of the contract, consistency of the implementation and quality of verification, not by guessing the author's preferred wording.

## Story 10: Add directions as text

**First hint:** The desired improvement is “Make the final approach understandable without a map service.” Start by identifying which existing boundary already knows the necessary information. Do not copy that information into new state until you can explain why derivation is insufficient.

**Second hint:** Follow this source-specific route: Add numbered fictional directions; identify the entrance consistently; link from the venue paragraph.. Keep each stage independently inspectable. If a step requires a policy choice, write the choice before implementing it.

**Third hint:** Your strongest completion evidence should establish: The local fragment resolves and directions remain usable if the illustration fails.. Invent a plausible wrong implementation and make your example disagree with it.

**Decision still left to you:** Choose the landmark descriptions. The guide intentionally does not settle this. Evaluate your answer by clarity of the contract, consistency of the implementation and quality of verification, not by guessing the author's preferred wording.

## Story 11: Distinguish decorative artwork

**First hint:** The desired improvement is “Compare informative and decorative image roles.” Start by identifying which existing boundary already knows the necessary information. Do not copy that information into new state until you can explain why derivation is insufficient.

**Second hint:** Follow this source-specific route: Add a small purely decorative local asset; use empty alt for that asset only; retain meaningful alt for the original illustration.. Keep each stage independently inspectable. If a step requires a policy choice, write the choice before implementing it.

**Third hint:** Your strongest completion evidence should establish: Removing artwork loses no essential event facts and roles are explained.. Invent a plausible wrong implementation and make your example disagree with it.

**Decision still left to you:** Choose decoration that carries no unique information. The guide intentionally does not settle this. Evaluate your answer by clarity of the contract, consistency of the implementation and quality of verification, not by guessing the author's preferred wording.

## Story 12: Add an organizer identity

**First hint:** The desired improvement is “Explain who answers the example contact address.” Start by identifying which existing boundary already knows the necessary information. Do not copy that information into new state until you can explain why derivation is insufficient.

**Second hint:** Follow this source-specific route: Add a fictional organizer name in text; keep link purpose clear; test a long name at narrow width.. Keep each stage independently inspectable. If a step requires a policy choice, write the choice before implementing it.

**Third hint:** Your strongest completion evidence should establish: The organizer label and contact link stay connected without clipping.. Invent a plausible wrong implementation and make your example disagree with it.

**Decision still left to you:** Choose a fictional name and role. The guide intentionally does not settle this. Evaluate your answer by clarity of the contract, consistency of the implementation and quality of verification, not by guessing the author's preferred wording.

## Story 13: Add a cancellation notice

**First hint:** The desired improvement is “Communicate a changed event state clearly.” Start by identifying which existing boundary already knows the necessary information. Do not copy that information into new state until you can explain why derivation is insufficient.

**Second hint:** Follow this source-specific route: Add a prominent textual status near the heading; retain the original event context; avoid color-only meaning.. Keep each stage independently inspectable. If a step requires a policy choice, write the choice before implementing it.

**Third hint:** Your strongest completion evidence should establish: A stylesheet-free reading clearly says the event is canceled.. Invent a plausible wrong implementation and make your example disagree with it.

**Decision still left to you:** Choose whether to retain the original date. The guide intentionally does not settle this. Evaluate your answer by clarity of the contract, consistency of the implementation and quality of verification, not by guessing the author's preferred wording.

## Story 14: Create a second notice variant

**First hint:** The desired improvement is “Practice content reuse without a framework.” Start by identifying which existing boundary already knows the necessary information. Do not copy that information into new state until you can explain why derivation is insufficient.

**Second hint:** Follow this source-specific route: Copy the small page into a separate practice fixture; change event facts consistently; share the stylesheet through a relative link.. Keep each stage independently inspectable. If a step requires a policy choice, write the choice before implementing it.

**Third hint:** Your strongest completion evidence should establish: Each page answers what, when, where and contact without mixing events.. Invent a plausible wrong implementation and make your example disagree with it.

**Decision still left to you:** Choose which content genuinely differs. The guide intentionally does not settle this. Evaluate your answer by clarity of the contract, consistency of the implementation and quality of verification, not by guessing the author's preferred wording.

## Story 15: Explain the box model visually

**First hint:** The desired improvement is “Add a developer worksheet beside the guide.” Start by identifying which existing boundary already knows the necessary information. Do not copy that information into new state until you can explain why derivation is insufficient.

**Second hint:** Follow this source-specific route: Record declared widths; calculate padding inside border-box; compare a temporary content-box experiment.. Keep each stage independently inspectable. If a step requires a policy choice, write the choice before implementing it.

**Third hint:** Your strongest completion evidence should establish: The worksheet predicts the observed wrap instead of hiding overflow.. Invent a plausible wrong implementation and make your example disagree with it.

**Decision still left to you:** Choose measurement values for the experiment. The guide intentionally does not settle this. Evaluate your answer by clarity of the contract, consistency of the implementation and quality of verification, not by guessing the author's preferred wording.

## Mentor feedback rubric

| Dimension | Beginning | Developing | Independent evidence |
|---|---|---|---|
| Trace | Names files only | Follows one ordinary case | Predicts a new boundary and explains its owner |
| Test design | Copies output | Uses a stated expectation | Rejects a plausible wrong candidate |
| Design | Repeats a slogan | Names an alternative | Compares costs using a concrete change |
| Agent use | Accepts a generated answer | Checks suggested edits | Supplies own proposal and adjudicates critiques |
| Handoff | Claims it works | Lists actual checks | Explains behavior, evidence and limits coherently |

Use the rubric to choose the next practice action, not to label yourself permanently. A learner may be independent at source tracing and still need help designing a failure case. Target the missing skill with one smaller exercise.
