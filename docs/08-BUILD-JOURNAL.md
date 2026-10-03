# Build journal: Community Notice Sheet

[Code tour](03-CODE-TOUR.md) · [Actual verification](VERIFICATION.md)

This is a retrospective teaching narrative about the implementation in this repository. It is not a verbatim conversation, fabricated team debate or hidden chain-of-thought transcript. The design explanations below are reviewable rationales tied to the source. Dates and check results belong to the verification record.

## The starting problem

A neighborhood group needs a readable one-page notice with an obvious heading and contact link.

The main temptation was to make the project larger than its learning target. The useful boundary is **semantic html and the box model**. A finished small example lets you inspect the whole path and ask what each part contributes. Extra infrastructure would add more things to configure before the central idea became clear.

## The first contract

One fictional notice remains meaningful without CSS. Its desktop columns use inline-block and the box model; no Flexbox or Grid is used. The illustration has a useful text alternative and the narrow view returns to ordinary block flow.

The contract turned broad intent into examples that can disagree with an implementation. That matters because a plausible-looking result can hide a wrong boundary rule. The examples in the concepts guide were chosen to expose those distinctions, not to make the demo look flawless.

## Decision note 1: Choose HTML by meaning

The date uses time, the illustration uses figure and figcaption, and the notice has a real heading. Choosing these elements first keeps information available independently of the visual arrangement.

**What a learner should challenge:** Identify which facts should still be readable if every style rule disappears.

**Evidence to consult:** inspect the owning source file, the contract examples and the verification scope. If your alternative satisfies the same behavior with a different structure, compare the maintenance cost instead of assuming one syntax is automatically correct.

## Decision note 2: Keep the assignment’s inline-block constraint

This constraint is educational rather than a claim that inline-block is the universal modern layout choice. Widths of 55% and 40% leave space for inline whitespace. Border-box keeps padding within the declared widths.

**What a learner should challenge:** Explain why two 50% inline-block boxes can unexpectedly wrap.

**Evidence to consult:** inspect the owning source file, the contract examples and the verification scope. If your alternative satisfies the same behavior with a different structure, compare the maintenance cost instead of assuming one syntax is automatically correct.

## Decision note 3: Let narrow content stack

A small screen benefits from ordinary block flow rather than shrinking both columns indefinitely. The responsive rule changes layout while preserving the same content and source order.

**What a learner should challenge:** Choose a different breakpoint based on a visible content failure, not a device brand.

**Evidence to consult:** inspect the owning source file, the contract examples and the verification scope. If your alternative satisfies the same behavior with a different structure, compare the maintenance cost instead of assuming one syntax is automatically correct.

## What the checks contributed

The static asset check caught missing local resources, while the browser checks exercised layout, keyboard entry and project-specific content changes. Neither check alone would justify a blanket accessibility claim.

The record in VERIFICATION.md reports actual local observations. A GitHub Actions workflow is provided, but its remote result must be inspected separately after a push. A screenshot documents one rendered state; it is not a substitute for the interaction and boundary checks.

## What you should do differently on your own build

Start from the same user need but write your own examples first. Choose a small variation from the story list. Predict behavior, implement a slice and compare the result with your prediction. The reference helps you judge a finished result; your journal should record your own uncertainties and discoveries rather than adopting this narrative as if you experienced it.

## The handoff

The next learner can start from README, locate `notice-copy and notice-art`, reproduce the example table and attempt one bounded story. That is the intended handoff quality: a working result plus enough evidence and explanation to continue safely. The six practice stories remain unfinished for the learner.
