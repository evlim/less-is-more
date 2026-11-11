---
name: less-is-more
description: "Keep calls to action and visual hierarchy clear as interfaces gain features. Use when designing, adding UI features, reviewing a crowded screen, or simplifying a landing page, app, dashboard, editor, or mobile flow. Analyze visual pop-out, preattentive attributes, competing actions, and progressive disclosure while preserving accessibility and useful functionality. Framework-independent; not a mandate for a minimalist visual style or fewer features."
license: MIT
---

# Less Is More

Help people recognize what to do next. Treat attention as limited: a new capability needs a deliberate place in the workflow, not automatic visual prominence. Preserve the product's character, useful density, and the user's requested scope.

## Establish the task before changing the look

Inspect the existing interface and relevant project guidance. Identify the user, their current task, and the screen's state. If the main task is reasonably clear, proceed and state the assumption briefly; ask only when competing interpretations would materially change the design.

Separate presentation decisions from product requirements. Preserve existing interaction and data semantics. When a new feature's behavior is unspecified, label assumptions or resolve the important requirement; do not invent eligibility rules, discard valid results, or change what an action does just to simplify its presentation.

Describe the intended next outcome in plain language, such as **choose a destination**, **compare suitable plans**, **resume editing**, or **resolve an alert**. Then identify the controls and information that support it.

A primary action is not necessarily a button. Search, a selectable item, direct destination links, or an editable canvas may be the main interaction. Several entry points can serve the same outcome: destination search and country/region links can both start a comparison. Optional data or validity filters refine that task. Do not demote these useful alternatives just to achieve a one-button layout.

Prefer a clear primary path within each meaningful task region. Repeated result cards, independent panes, and equally valid choices may have several actions. Do not impose a universal CTA count or pick an arbitrary preferred item. Reassess the hierarchy when state changes: selection, editing, loading, errors, empty results, and completion can require different next steps. A critical warning may legitimately take priority over the usual CTA.

## Give every addition a placement decision

For a substantial change, make a small inventory: element, user need, importance now, current emphasis, and proposed placement. For a small change, reason through the affected elements without producing a formal audit.

| Role in the current task | Default treatment |
| --- | --- |
| Main action or necessary decision information | Keep visible and easy to identify where the decision happens. |
| Frequent supporting control | Keep available with quieter emphasis and a clear label. |
| Occasional or advanced capability | Use a predictably labeled disclosure, panel, or settings destination. |
| Useful only after a selection or in a particular state | Reveal it in that context, preserving a discoverable route when needed. |
| Unrelated task or duplicate entry point | Relocate, combine, or remove redundancy within the requested scope. |

Consider frequency, consequences, dependencies, discoverability, and the cost of another interaction. A feature's novelty or implementation effort does not determine its prominence. Hide only when the user can reliably find it and does not need it to make the current decision. Quieter styling is often enough.

Prefer integrating a new capability into its existing task: a search mode near search, assistance beside its input, export near the selected content. Avoid adding a new hero card, navigation item, banner, and button for every feature. If the addition competes with the main path, reduce or relocate existing emphasis before making the primary action louder.

## Inspect what attracts attention

Judge the whole rendered viewport, including headers, promotional badges, illustrations, sticky elements, and repeated cards. Examine both the main path and its strongest competitors.

Compare hue and saturation, luminance contrast, size/area, shape and orientation, and motion. These can contribute to rapid visual detection, often called **preattentive processing** or **visual pop-out**. Their effects depend on surrounding elements, combinations of features, and the viewer's task; they are not a formula for conversions.

Also inspect typography, position, whitespace, proximity, alignment, borders, shadows, and grouping. These help organize a hierarchy, but do not label every layout technique a preattentive attribute. A tiny animated badge can compete with a large button; many bright buttons can erase relative priority.

- Reserve the strongest appropriate treatment for the current task or critical status. Use existing design tokens and semantic colors; no color is universally the best CTA color.
- Reduce competing fills, badges, borders, repeated headings, and decoration before increasing size or saturation. Remove low-value default labels while retaining meaningful differences.
- Keep supporting controls legible and obviously interactive. Use weight, fill, grouping, and placement to lower prominence; do not make them look disabled.
- Write action labels that name the outcome. Keep essential context close to the choice. Give distinct behaviors distinct affordances rather than making an entire complex card unexpectedly navigate.
- Use motion only when it communicates useful state or directs necessary attention, and respect reduced-motion preferences.

A brief glance, thumbnail, squint, or grayscale review can reveal competing emphasis. These are diagnostic heuristics, not eye tracking, accessibility testing, or proof of comprehension. Confirm with realistic tasks when possible. See [research and limits](references/principles.md) when a rationale or accessibility threshold is needed.

## Simplify without concealment

Keep material costs, limitations, consequences, errors, and required disclosures understandable at the decision point. Do not hide cancellation, refusal, privacy choices, recovery, or destructive consequences to favor a business metric. Respect requirements for equally prominent choices. An information dialog may hold supporting detail; it must not be the only place to discover a fact essential to choosing correctly.

For progressive disclosure, use a label that predicts the contents. Keep the route available to keyboard, touch, and assistive technology; expose expanded/selected state and handle focus appropriately. Show active filters or changed settings in the collapsed summary when they affect the result. Preserve values when closing or reopening. Avoid hover-only access, unexplained icons, and a generic overflow menu full of frequent actions.

Preserve contrast, accessible names, focus visibility, meaningful order, usable targets, zoom/reflow, and semantic structure. Never encode importance or state through color alone. A smaller visual role need not mean a smaller hit area. Dense expert tools can remain dense when grouping and local hierarchy support the work.

## Verify the change and leave a usable record

When implementation is requested, make the smallest coherent change using the existing framework and components. A review request calls for findings, not unsolicited edits. Do not replace the design system, delete capabilities, or add dependencies merely to follow this skill.

Use the available preview and interaction tools to inspect the actual result. Check relevant wide and narrow layouts, long/localized labels, keyboard and touch operation, and affected expanded, selected, loading, error, empty, or success states. Verify that the main task still works, secondary features remain findable, and sticky layers or dialogs do not cover actions or focus. Run the project's relevant checks. If rendering or interaction testing is unavailable, identify that limitation instead of claiming visual verification.

For ongoing feature work, consult existing design notes before adding emphasis. When implementation is authorized, record durable decisions in the project's existing design documentation, or a small appropriate note if none exists: the primary outcome by screen/state, equivalent entry points, supporting actions, disclosure locations, and why exceptions matter. Update that record when the task changes. Do not silently rewrite global agent instructions. A skill is reusable guidance, not guaranteed permanent memory; its installation and selection depend on the host.

Report briefly what the main path is, what changed in prominence or placement, what remains accessible, and what was verified. Use [the examples](references/examples.md) for ambiguous multi-action cases or a new feature that seems to demand another CTA.

If outcome data is available, use task completion, time, errors, abandonment, and secondary-feature findability as appropriate. Keep event definitions, denominators, time windows, and traffic mix comparable. Distinguish visual observation, usability evidence, and measured association. Do not equate fewer elements with better UX, clicks with purchases, or a before/after trend with causal improvement.
