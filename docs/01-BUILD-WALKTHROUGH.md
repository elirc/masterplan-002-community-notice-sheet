# Building Community Notice Sheet, one decision at a time

[Learning route](00-START-HERE.md) · [Code tour](03-CODE-TOUR.md)

This is a reconstruction of how to approach the finished reference. It explains visible design choices; it is not a transcript of hidden reasoning or a claim that a fictional team performed these steps.

## Start from the contract

One fictional notice remains meaningful without CSS. Its desktop columns use inline-block and the box model; no Flexbox or Grid is used. The illustration has a useful text alternative and the narrow view returns to ordinary block flow.

The smallest useful result answers this user need: A neighborhood group needs a readable one-page notice with an obvious heading and contact link. Write the examples before choosing file names. Keep the scope small enough that the decisive behavior fits in one trace.

## Step 1: Write a useful notice first

A page needs to answer what, when, where and how to ask a question. Fill those facts in HTML before choosing colors. The example address is fictional. The illustration supports the event, but it does not carry the only statement of the time or location. That separation matters when images fail, when someone uses a text-oriented browser, or when a reader skims headings.

**Pause and produce evidence:** Styles disabled. Predict the outcome, then compare it with the reference. In your notes, distinguish what the code says should happen from what you actually observed.

## Step 2: Measure the boxes

Read the project-specific rules at the bottom of style.css. The copy reserves 55% and the figure 40%; padding belongs inside those widths because border-box is applied consistently. Inline-block elements still participate in inline formatting, so source whitespace has width. Predict what happens if both widths become 50% and then test it in developer tools without saving the change.

**Pause and produce evidence:** Desktop width. Predict the outcome, then compare it with the reference. In your notes, distinguish what the code says should happen from what you actually observed.

## Step 3: Design for awkward content

Replace the location with a long but realistic place name. At a narrow viewport, the text must wrap within the content column rather than disappearing under overflow:hidden. The reference switches to a single column below 650px. It does not move the contact information into an image or depend on a hover interaction to reveal essential facts.

**Pause and produce evidence:** 320px width. Predict the outcome, then compare it with the reference. In your notes, distinguish what the code says should happen from what you actually observed.

## Step 4: Verify meaning as well as appearance

A screenshot can show attractive boxes while hiding broken reading order. Disable the stylesheet, inspect the heading hierarchy and open the page using only the keyboard. The automated asset check proves files exist, not that the alternative text is well written. The browser evidence records a missing-image probe; you still need to judge whether the replacement description is useful.

**Pause and produce evidence:** notice.svg missing. Predict the outcome, then compare it with the reference. In your notes, distinguish what the code says should happen from what you actually observed.

## Keep the implementation reviewable

A useful commit has one understandable reason to exist. Separate the initial working slice, the checks that expose its important boundaries, and the teaching material that explains it. The published commits in this repository were assembled from verified working files; they are real commits, not fabricated evidence of a long historical development process.

For your own variation, commit at a point where the behavior and evidence agree. Describe the trigger, the resulting behavior and the check in the commit message or review note. Avoid mixing a rule change with unrelated formatting because it makes the learning decision harder to see.

## Stop before adding a platform

The next useful improvement is a sharper example or clearer explanation, not a database, account system or framework migration. Add an abstraction only when it names a real repeated responsibility. You should be able to describe what becomes easier to change after the abstraction and what new complexity it introduces.

**Independent design choice from the original brief:** Choose meaningful elements and write the image alternative text.

The reference made one choice, documented in the code tour. You may choose differently in a branch if you first revise the contract and acceptance examples. A deliberate alternative is a stronger learning artifact than an unexplained copy.
