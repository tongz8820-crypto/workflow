---
name: design-workflow
description: Stage-aware workflow for visual products. Use when a UI, H5/web experience, prototype, presentation, Figma design, document, or other visual artifact still has open design decisions, an undecided delivery medium, a request spanning design through implementation, or a cross-medium review or optimization need. Separate design decisions from implementation and load HTML guidance only after HTML/web is selected. Do not use when the medium and requested action are already clear and a dedicated medium-specific skill can act directly, or for an isolated mechanical edit with an exact target and change.
---

# Design Workflow

Treat design and implementation as related but distinct stages. The user should not pay the cost of open-ended exploration after a direction is settled, and implementation rules for one medium should not leak into another.

## 1. Inspect before deciding

Read the brief and any supplied code, screenshots, brand material, design system, or prior decision record. Inspect only artifacts the user supplied, named, or placed unambiguously in scope. Do not treat an adjacent workspace file as the target merely because it is available. If no target artifact can be identified, request it or state that an evidence-based review cannot proceed. Reuse decisions that are already explicit. Do not ask the user to repeat information available in the supplied context.

## 2. Honor explicit intent, then classify the stage

The user's requested action takes priority over missing background information:

- "design", "explore", or "compare" selects design work;
- "implement", "build", or "make this" selects implementation, with only the missing decisions required to implement addressed;
- "review", "audit", or "explain" selects non-mutating review;
- "fix", "improve", or "polish" authorizes scoped optimization followed by verification.

Do not send an explicit review request back to design merely because audience, brand, or another input is incomplete. Report how the missing context limits confidence or ask only when the answer is necessary for a useful review.

When the requested action spans stages or is genuinely unclear, choose the earliest unresolved stage:

Choose the earliest unresolved stage:

1. **Design** — the goal, audience, structure, interaction model, or visual direction is still open.
2. **Medium selection** — the design is sufficiently defined, but the delivery medium is not.
3. **Implementation** — the direction and delivery medium are already selected.
4. **Review** — an artifact exists and the user wants findings, optimization, or a release check.

If the request contains a precise mechanical change, such as changing one known spacing value, skip this workflow and make the scoped change using the relevant implementation workflow. If the medium and action are already explicit, prefer the dedicated medium-specific skill without adding this routing layer.

## 3. Load only the guidance required

| Situation | Read |
| --- | --- |
| Design decisions are open | `references/design-stage.md` |
| Delivery medium is open | `references/implementation-routing.md` |
| HTML, H5, web, React, Vue, Svelte, or browser prototype is selected | `references/html-implementation.md` |
| The user asks for review, optimization, or pre-delivery verification | `references/quality-gates.md` |

For PowerPoint, Figma, documents, PDFs, native applications, or another non-web medium, use `references/implementation-routing.md` and then the available medium-specific skill. Do not load or apply `html-implementation.md` merely because HTML is technically possible.

## 4. Respect stage boundaries

- In the **design stage**, explore only decisions that remain open. Stop with a design decision record when the user requests a plan rather than an implementation.
- In the **implementation stage**, follow the approved direction. Do not generate extra concepts, change the information architecture, or add tweak controls unless the user requests renewed exploration.
- In **review mode**, report findings without modifying files unless the user also asks for fixes. When fixes are authorized, make only the changes supported by the findings and re-verify them.
- If a discovery during implementation invalidates an approved decision, surface the conflict and return only that decision to the user. Do not silently redesign the whole artifact.

## 5. Use conditional design heuristics

Treat the following as prompts for judgment, not universal defects:

- Produce multiple variations when the brief is open or the user asks for alternatives.
- Add live tweak controls when stakeholders need to compare or tune options in the artifact.
- Question pure white/black, common fonts, gradients, and familiar card treatments only when they appear to be unexamined defaults rather than brand or accessibility choices.
- Run a full quality gate before delivery or when requested; use a narrower check during early iteration.

## 6. Handoff contract

Before implementation, make the following explicit in the conversation or a project document:

- user and task goal;
- selected direction and any important rejected alternatives;
- required screens, sections, states, or slides;
- visual tokens or source design system;
- selected delivery medium and why it fits;
- acceptance criteria and known placeholders.

If these are already established, summarize rather than reopening them.

## 7. Completion criteria

A task is complete when:

- the current stage was correctly identified;
- only relevant reference guidance was loaded;
- the selected medium's implementation workflow was followed;
- requested verification was performed in proportion to risk;
- unresolved decisions and unverified behavior are stated plainly.

This skill is adapted from the design procedures in Trystan-SA/claude-design-system-prompt. See `SOURCE.md` and `LICENSE`.

