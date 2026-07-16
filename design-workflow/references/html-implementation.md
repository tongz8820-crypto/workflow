# HTML and Web Implementation

Read this reference only after HTML, H5, a web framework, or a browser prototype has been selected as the delivery medium.

## Preserve the approved direction

Inspect the existing codebase, framework, components, tokens, and conventions before editing. Reuse them when they satisfy the approved design. Do not replace the stack or introduce a new component system merely to express the design.

Implement the smallest coherent surface that satisfies the approved scope. If the design decision record conflicts with the codebase or the platform, surface the conflict instead of silently changing either.

## Build with web-native structure

- Use semantic HTML and native controls before ARIA or custom interaction roles.
- Use the existing layout approach; otherwise choose Grid for two-dimensional composition and Flexbox for one-dimensional alignment.
- Express repeated visual decisions as the project's existing tokens or CSS custom properties.
- Reuse components for repeated patterns, but do not create a library for a single-use element.
- Use real or clearly marked placeholder content. Do not invent unsupported metrics, testimonials, or product claims.
- Make responsive behavior follow actual usage priorities rather than merely shrinking the desktop layout.

## Implement relevant states

For each interactive element, implement the states its behavior requires:

- visible default affordance;
- hover where pointer input exists;
- active or pressed feedback;
- keyboard-visible focus;
- disabled state with an understandable reason when relevant;
- loading, success, and error feedback for asynchronous actions;
- empty and validation states for data and forms.

Use touch targets, contrast, labels, semantics, and keyboard behavior appropriate to the target users and accessibility level. Treat common numerical guidelines as baselines to verify in context, not substitutes for testing.

## Use motion deliberately

Motion should explain state, hierarchy, or continuity. Keep routine feedback fast, avoid animation that blocks task completion, and respect `prefers-reduced-motion`. Do not add animation simply to make the artifact look more designed.

## Add variants or tweak controls conditionally

Add multiple live variants or a tweak panel only when the user wants stakeholders to compare or tune options inside the artifact. Keep such controls separate from production UI and exclude them from the shipped experience unless they are a product feature.

## Verify in the browser

Verification should match the implementation risk:

- render the affected screens at representative viewport sizes;
- check overflow, wrapping, alignment, and content density;
- exercise the full interaction path, including errors and recovery;
- verify keyboard order, visible focus, labels, and reduced motion;
- run existing tests, type checks, and builds when code changed;
- distinguish verified behavior from assumptions or unavailable external services.

For an HTML slide deck, additionally verify fixed aspect ratio, scaling or letterboxing, navigation, slide bounds, typography at presentation distance, printing/export, and offline asset availability. Use HTML decks for web-native or interactive value; use the presentation workflow when editable `.pptx` delivery is the real requirement.

