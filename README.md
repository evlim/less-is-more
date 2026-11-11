# Less Is More

**Keep the next action clear as your product grows.**

A framework-independent agent skill for developers adding features without letting the interface become a wall of competing buttons, badges, and panels.

The skill asks the agent to identify the user's main task, inspect what draws attention, and decide which features should be prominent, quieter, contextual, or available through a clear disclosure. It covers visual pop-out and preattentive attributes alongside grouping, typography, spacing, and accessibility.

It works with the interface and framework you already use: web, mobile, desktop, dashboards, editors, and other visual applications. No runtime package, UI library, or paid service is required. Agents need appropriate tools to implement and verify changes in your environment.

## Use it

The portable skill is in **[skills/less-is-more](skills/less-is-more/SKILL.md)** and follows the [Agent Skills format](https://agentskills.io/specification).

Ask a skills-capable agent to install that directory from this repository:

```text
Install the less-is-more skill from
https://github.com/evlim/less-is-more/tree/main/skills/less-is-more
```

For Codex with the built-in installer:

```text
$skill-installer install https://github.com/evlim/less-is-more/tree/main/skills/less-is-more
```

You can also copy the entire `skills/less-is-more` directory into your agent's documented skills location. Keep its references and license together. Installation, automatic selection, and invocation syntax depend on the host; consult its current instructions. Codex setup is documented in [Build skills](https://learn.chatgpt.com/docs/build-skills). Agents without skill support can read `SKILL.md` as task guidance, with the referenced files available when needed.

Then use a request such as:

```text
Use less-is-more to add export and saved views to this dashboard.
Keep the report's main task clear and make the new controls easy to find.
```

```text
Use less-is-more to review this landing page. The main action is choosing
a destination, through search or a direct country/region link. Data and
trip duration are optional refinements. Identify competing emphasis.
```

```text
Use less-is-more when adding this feature. Implement the change, check
the affected screen states, and update our existing design notes so the
next feature preserves the intended hierarchy.
```

In hosts that support `$` invocation, use `$less-is-more`. For ongoing adoption, reference the skill in your team's existing UI development guidance and keep the screen's primary tasks in project design notes. Skill installation alone is not a guarantee that every future task will load it.

## What changes in the agent's decisions

| Situation | Decision the skill encourages |
| --- | --- |
| A new capability is added | Decide where and when it belongs before giving it prominent styling. |
| Search and direct links serve the same goal | Preserve useful entry points; do not force a one-button page. |
| Everything looks primary | Reduce competing emphasis before enlarging the main action. |
| An advanced feature is rarely needed | Use a discoverable, accurately labeled disclosure. |
| A warning affects the user's decision | Give it appropriate visibility, even ahead of the usual CTA. |
| A dense professional tool is useful | Improve grouping and local hierarchy without removing needed controls. |
| The page looks simpler | Verify task completion, accessibility, and feature findability. |

**Less Is More** names a recurring decision principle. **Minimalist** could imply a prescribed visual style. This skill preserves a product's character and supports multiple legitimate actions. It does not require monochrome screens, one CTA per page, or fewer features.

## Origin and evidence

The skill grew out of reviewing the evolving [eSIM Grab](https://esimgrab.com/) interface: keeping destination choice clear while expanding the search and comparison experience. Its examples generalize that problem for other products. The repository contains original guidance, not the application's private source or analytics.

Simpler appearance does not prove better conversion. The skill distinguishes visual changes, usability observations, and measured outcomes. [Research and limits](skills/less-is-more/references/principles.md) explains the sources and accessibility boundaries; [examples](skills/less-is-more/references/examples.md) covers common tradeoffs.

## Review and contribute

Use the [behavioral evaluation cases](evals/scenarios.md) when changing the guidance. Check what the agent actually decides, rather than matching its wording. Contributions should improve decisions across products and frameworks, preserve useful alternatives and accessibility, and avoid adding rules based on one aesthetic preference.

## License

[MIT](LICENSE). You may use, adapt, and redistribute the skill with the license notice. Referenced external material remains under its respective terms.
