# Code tour and architecture decisions

[Overview](../README.md) · [Concepts](02-CONCEPTS-AND-TRACES.md)

| File | Responsibility |
|---|---|
| [package.json](../package.json) | Names the module format, Node requirement and local commands; private prevents npm publication. |
| [.github/workflows/check.yml](../.github/workflows/check.yml) | Runs the committed checks on GitHub. A workflow file is not evidence that a remote run succeeded. |
| [public/index.html](../public/index.html) | Semantic notice content: headings, `time`, figure with alt text and the contact link. |
| [public/style.css](../public/style.css) | Presentation, focus indication and project-specific layout. |
| [tools/serve.mjs](../tools/serve.mjs) | Local preview infrastructure; only public/ is served. |
| [tools/check-site.mjs](../tools/check-site.mjs) | Checks referenced local assets exist, without pretending to judge usability. |

## Follow one path, not every file

Start at [public/index.html](../public/index.html) and locate `notice-copy and notice-art`. Use this trace as a map: HTML declares the announcement and its heading → the browser gives elements their normal flow → .notice-copy and .notice-art become inline-block boxes → percentage widths reserve room for whitespace → the 650px rule stacks the boxes.

The tooling is intentionally separate from the product concept. You can study the local server or CI after the main rule is clear. Neither an HTTP preview server nor a workflow configuration should become a prerequisite for understanding a layout rule.

## Decision: Choose HTML by meaning

The date uses time, the illustration uses figure and figcaption, and the notice has a real heading. Choosing these elements first keeps information available independently of the visual arrangement.

**Review question:** Identify which facts should still be readable if every style rule disappears.

**Your alternative:** Write a plausible different choice, then give a concrete example that reveals its cost. “More scalable” or “cleaner” is not enough; identify a changed dependency, a new state to manage, or a user-visible failure mode.

## Decision: Keep the assignment’s inline-block constraint

This constraint is educational rather than a claim that inline-block is the universal modern layout choice. Widths of 55% and 40% leave space for inline whitespace. Border-box keeps padding within the declared widths.

**Review question:** Explain why two 50% inline-block boxes can unexpectedly wrap.

**Your alternative:** Write a plausible different choice, then give a concrete example that reveals its cost. “More scalable” or “cleaner” is not enough; identify a changed dependency, a new state to manage, or a user-visible failure mode.

## Decision: Let narrow content stack

A small screen benefits from ordinary block flow rather than shrinking both columns indefinitely. The responsive rule changes layout while preserving the same content and source order.

**Review question:** Choose a different breakpoint based on a visible content failure, not a device brand.

**Your alternative:** Write a plausible different choice, then give a concrete example that reveals its cost. “More scalable” or “cleaner” is not enough; identify a changed dependency, a new state to manage, or a user-visible failure mode.

## Change boundaries

A small change should begin in the file that owns its meaning. Semantic information belongs in HTML before styling; layout belongs in the relevant CSS rule.

If a story crosses two files, say why. A new section may require markup, a navigation link or a layout rule to change together. That is a coherent feature boundary, not permission to rewrite unrelated parts of the project.

## Deliberate limits

No persistence, external integration or general framework is hidden behind these files. The preview server is a local development aid, not a production hosting system. A browser screenshot is one observation, not proof of every device or assistive technology. Keep these limits visible when describing your own work.
