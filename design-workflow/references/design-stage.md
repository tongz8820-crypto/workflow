# Design Stage

Use this reference when meaningful design decisions remain open. The goal is to reduce uncertainty and produce an implementable decision record, not to create options for their own sake.

## Establish context

Read available evidence first. Determine:

- the primary user and their goal;
- the artifact's job and the most important action or message;
- where and how it will be used;
- existing brand, design system, codebase, screenshots, or reference material;
- technical, accessibility, content, schedule, and delivery constraints;
- decisions already made and decisions genuinely still open.

Ask a question only when its answer would materially change the design. Consolidate closely related unknowns. For minor choices with a defensible default, decide and record the assumption.

## Choose the appropriate exploration depth

### Direct direction

Use when the brief is mostly defined. Produce one recommended direction and identify the few decisions needing confirmation.

### Comparative exploration

Use when the user asks for alternatives or the problem has multiple plausible structures. Usually produce two or three substantively different options. Vary structure, hierarchy, interaction, density, or tone rather than only color.

### Low-fidelity exploration

Use wireframes when the flow, navigation, information hierarchy, or page structure is uncertain. Keep visual styling intentionally limited so structural feedback is not confused with aesthetic feedback.

Do not generate multiple directions for exact reproduction, a small follow-up, or an already-approved design.

## Define the design system at the right fidelity

When an existing system is available, extract concrete values rather than inventing replacements:

- color and semantic roles;
- typography families, sizes, weights, and line heights;
- spacing and density;
- radius, borders, shadows, and elevation;
- components, variants, and interaction states;
- motion principles and accessibility requirements.

For greenfield work, commit to a coherent direction tied to the brief. Avoid silent defaults. A direction should be concrete enough that two implementers would make similar choices.

## Include system and state thinking

Identify reusable components and document only the variants and states the product needs. Cover relevant default, hover, active, focus, disabled, loading, empty, success, and error states. Do not invent component-library scope unsupported by the artifact.

## Design decision record

Conclude the stage with this compact structure:

```markdown
# Design decision

## Goal and audience
[Who, context, primary task or message]

## Selected direction
[Structure, interaction model, visual tone, and why]

## Alternatives considered
[Only meaningful alternatives and why they were not selected]

## Required content and states
[Screens, sections, components, data, and edge states]

## Design system inputs
[Existing sources or newly agreed tokens]

## Delivery medium
[Selected medium, or the remaining decision]

## Acceptance criteria
[Observable conditions for successful implementation]

## Open decisions and placeholders
[Only unresolved items]
```

Stop here when the user requested design or planning only. Proceed to medium selection or implementation only when the request includes that scope.

