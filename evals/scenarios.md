# Behavioral evaluation cases

Use these to check meaningful decisions after changing the skill. Give an independent agent the skill and one request at a time. Request a concrete design proposal or use an isolated mock project for implementation. Do not allow evaluation tasks to change production systems.

These are manual behavioral checks, not an automated benchmark. A formatting validator cannot prove the skill makes good design decisions.

## 1. Multiple entry points, one outcome

Request: A travel landing page has destination search, optional data and days inputs, direct country/region links, an animated referral banner, and a separate large trip-planner button. Add multi-country search and simplify the screen.

Evaluate whether the result identifies choosing a destination as the outcome; preserves useful search and direct-link paths; keeps refinements optional; integrates the new mode coherently; and considers the banner's relative salience. Reject an arbitrary one-button design or compulsory filters.

## 2. Expert workspace gains features

Request: A native editing app has a dense timeline, common edit commands, autosave status, and undo. Add export presets and AI assistance without making it harder to keep editing.

Evaluate contextual placement, continued access to common actions, local hierarchy, preserved save/undo state, and native accessibility checks. Reject a mandatory spacious redesign, hidden frequent controls, or reliance on web-specific code.

## 3. Simplicity and consequential choices

Request: Simplify a subscription screen with upgrade, cancellation, recurring charges, and a failed-payment warning. Make the screen feel less overwhelming.

Evaluate visibility of costs, consequences, refusal/cancellation, and recovery. Reject a design that hides material information or weakens alternatives to increase upgrades. Critical status may take priority.

## 4. Repeated actions and noisy cards

Request: A comparison grid has twelve choices, each with a primary open action, a brightly filled coupon-copy button, a pulsing New badge, and details. The first result is not recommended. Make the next step clearer.

Evaluate consistent per-item actions, restrained supporting emphasis, preserved material differences, and no arbitrary promotion of the first result. Reject global one-CTA enforcement.

## 5. Evidence without a live preview

Request: Review a UI source diff without a browser. The redesign removed two banners, visits doubled, and recorded checkout clicks rose from 90/1,000 visits to 150/2,000. Write the review conclusion.

Evaluate whether the agent reports visual verification limits and distinguishes more clicks from a higher rate. The observed rates are 9% and 7.5%; neither the diff nor these aggregates establish causality or completed purchases. Reject claims of proven conversion uplift.

Record the skill revision, input, actual response, passed/failed behaviors, and any follow-up edits. Do not prefill results or treat these expected behaviors as measured outcomes.
