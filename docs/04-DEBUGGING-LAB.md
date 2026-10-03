# Debugging laboratory

[Concepts](02-CONCEPTS-AND-TRACES.md) · [Practice stories](05-PRACTICE-STORIES.md)

These are deliberately proposed defects for a scratch branch. They are not claims that the shipped reference still contains these bugs. Keep main working and introduce only one change at a time.

## Case 1: The second column drops unexpectedly

**Introduce or discuss this mistake:** Give both inline-block columns width:50%.

**Discriminating experiment:** Observe wrapping even though the two percentages appear to total 100.

### Worked diagnosis

First state the expected contract: One fictional notice remains meaningful without CSS. Its desktop columns use inline-block and the box model; no Flexbox or Grid is used. The illustration has a useful text alternative and the narrow view returns to ordinary block flow. Then create the smallest example from the experiment above. Compare the observed result with the contract before changing more code. The likely cause is at this boundary: **Inspect whitespace, padding and the computed box model.**. Repair that boundary, rerun the example, and check one neighboring valid case so the repair does not merely special-case the chosen input.

The completed reasoning record is: symptom → contract violated → input that distinguishes hypotheses → owning line or rule → minimal repair → regression evidence. This is a worked diagnostic route; fill in your actual outputs when you run it. No invented console transcript is supplied.

## Case 2: The illustration is the only location information

**Introduce or discuss this mistake:** Move the location into a hypothetical image.

**Discriminating experiment:** Disable images and try to find the venue.

### Your investigation

1. Write two possible explanations before looking at the hints.
2. Predict what the experiment would show if each explanation were true.
3. Run or inspect the smallest discriminating case and record the result.
4. Identify the owning file and make one bounded repair.
5. Verify the original case and a neighboring case; explain why both matter.

**Location hint, only after your attempt:** Keep essential event facts as text in public/index.html.

## Case 3: A narrow page hides content

**Introduce or discuss this mistake:** Apply a fixed wide width and then overflow:hidden.

**Discriminating experiment:** At 320px, part of the notice becomes unreachable.

### Your investigation

1. Write two possible explanations before looking at the hints.
2. Predict what the experiment would show if each explanation were true.
3. Run or inspect the smallest discriminating case and record the result.
4. Identify the owning file and make one bounded repair.
5. Verify the original case and a neighboring case; explain why both matter.

**Location hint, only after your attempt:** Repair the width and stacking rule rather than hiding the symptom.

## If the first repair does not work

Do not pile on another unrelated edit. Read the diff and check whether the observed failure changed. If the hypothesis was wrong, write that down and restore only your own experimental change before testing the next hypothesis. A rejected hypothesis is useful progress when its evidence is clear.

When asking an assistant for help, provide the exact input, expected and observed result, the current diff and the file you believe owns the rule. Ask for one counterexample or diagnostic question first. Keep proposed causes separate from demonstrated causes.
