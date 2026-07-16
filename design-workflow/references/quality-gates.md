# Quality Gates

Use this reference for a requested review, an authorized optimization pass, or a final delivery check.

## Choose the operating mode

### Review mode

Use when the user asks to inspect, audit, critique, or explain. Report evidence-backed findings and recommendations. Do not modify files.

Review only artifacts explicitly supplied, named, or unambiguously in scope. When the target is missing, ask for it and describe the evidence needed; do not convert unrelated workspace files into conditional findings.

### Optimization mode

Use when the user asks to improve, fix, polish, or prepare for delivery. Review first, apply scoped fixes, then re-verify. Preserve approved brand and product decisions unless the user authorizes a redesign.

### Final gate

Use before delivery when implementation is complete. Check blockers and high-impact quality issues; do not reopen settled aesthetic exploration merely to create more options.

## Review dimensions

### Purpose and hierarchy

- Can the target user identify the primary message or action quickly?
- Do size, position, weight, color, and spacing reflect actual importance?
- Is supporting material appropriately subordinate?
- Does every visible element serve the task, narrative, or necessary structure?

### Rhythm and system consistency

- Do spacing, typography, color, radius, and elevation follow the selected system?
- Are repeated patterns consistent or deliberately different?
- Are off-scale values intentional and documented rather than accidental?
- Are component variants and states complete for the implemented scope?

### Accessibility

- Verify contrast against the required level using actual resolved colors.
- Check semantic structure, headings, labels, alternative text, and native controls.
- Check keyboard reachability, logical focus order, visible focus, and modal behavior.
- Check color-independent state communication, motion preferences, errors, and relevant target sizes.

Treat pure white/black as a possible aesthetic signal, not an accessibility failure by itself. Contrast, brand intent, environment, and user needs determine whether it should change.

### Interaction and feedback

- Does each action provide immediate and understandable feedback?
- Are loading, success, failure, empty, validation, and recovery paths represented where relevant?
- Are hover, active, focus, disabled, and selected states distinguishable without contradicting the design system?
- Does state persist only where persistence benefits the task?

### Generic-pattern check

Question gradients, decorative emoji, familiar card recipes, fashionable fonts, warm-editorial palettes, excessive rounding, and filler sections when they look like unexamined defaults. Keep them when they trace to the brief, brand, medium, or an explicit design decision.

The test is not whether a pattern is common; it is whether the artifact has a defensible reason for using it.

### Medium-specific verification

Apply the selected medium's own delivery requirements. For HTML, use `html-implementation.md`. For presentations, Figma, documents, PDFs, native applications, and images, use their dedicated workflows rather than importing web assumptions.

## Finding format

For each actionable finding, report:

- severity: blocker, high, medium, or low;
- evidence: file, screen, component, or observed behavior;
- impact: user or delivery consequence;
- recommendation: smallest change that resolves the issue;
- confidence or verification limitation when evidence is incomplete.

In optimization mode, record what was fixed, what remains, and what was deliberately preserved.

