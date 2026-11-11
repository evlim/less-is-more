# Research and limits

These sources inform the skill's judgment. They do not validate a universal CTA count, an attention score, a prescribed color palette, or a conversion promise.

| Source | Useful implication | Limit |
| --- | --- | --- |
| [Christopher Healey: Perception in Visualization](https://www.csc2.ncsu.edu/faculty/healey/PP/) | Relative differences in visual features can support rapid detection. Inspect the target together with its distractors. | Findings from visual-search research do not directly prove a CTA's business effect. Feature combinations and task matter. |
| [NN/g: Visual Hierarchy in UX](https://www.nngroup.com/articles/visual-hierarchy-ux-definition/) | Use relative scale, contrast, and grouping to communicate importance. | A heuristic inspection is not a measured gaze path. |
| [NN/g: Progressive Disclosure](https://www.nngroup.com/articles/progressive-disclosure/) | Keep common essentials available and make the route to specialized options obvious. | Hiding a frequent control can increase effort; a sparse initial screen can still be hard to use. |
| [NN/g: Aesthetic and Minimalist Design](https://www.nngroup.com/articles/aesthetic-minimalist-design/) | Remove irrelevant competition while retaining what helps the task. | Minimalism does not require a particular aesthetic or a lower feature count. |
| [W3C: WCAG 2.2](https://www.w3.org/TR/WCAG22/) | Preserve accessible contrast, non-color cues, keyboard access, visible focus, and meaningful structure. | Passing a few checks does not establish full conformance. Native applications also need their platform's accessibility guidance. |

## Accessibility details when reducing emphasis

For web interfaces, WCAG 2.2 AA requires at least **4.5:1** contrast for ordinary text and **3:1** for large text, with specified exceptions. Required visual information identifying controls and their states generally needs **3:1** contrast against adjacent colors; this is not a requirement to draw every button boundary. Consult [text contrast](https://www.w3.org/WAI/WCAG22/Understanding/contrast-minimum.html) and [non-text contrast](https://www.w3.org/WAI/WCAG22/Understanding/non-text-contrast.html) for definitions and exceptions.

[Target Size (Minimum)](https://www.w3.org/WAI/WCAG22/Understanding/target-size-minimum.html) generally requires **24 by 24 CSS pixels**, subject to defined exceptions including sufficient spacing. **44 by 44 CSS pixels** belongs to the enhanced AAA criterion, not the universal AA minimum. Preserve generous usable areas when making a control visually quieter; follow platform conventions for native units and targets.

Use text, shape, or another appropriate cue alongside color. Check focus and disclosure behavior in addition to appearance. Accessibility and discoverability constrain the ways an interface can be simplified.

## What counts as evidence

- A rendered comparison can establish that elements moved or changed emphasis.
- A task-based observation can reveal whether someone finds and completes a path in the observed conditions.
- Comparable analytics can show an association with an outcome. Check tracking changes, traffic sources, devices, returning users, and concurrent product changes.
- A well-designed experiment offers stronger causal evidence, subject to its assumptions and limitations.

Do not turn these sources into mandatory numerical scoring. The skill applies their principles to the user's actual task.
