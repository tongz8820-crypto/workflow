# Source and adaptation notes

This skill is an adapted, stage-aware reorganization of selected design procedures from:

- Repository: `Trystan-SA/claude-design-system-prompt`
- Source URL: https://github.com/Trystan-SA/claude-design-system-prompt
- Reviewed commit: `3c3ddb07d7aa3fef051d83608596470c95cfd8fe`
- Source license: MIT

## Material retained

- design discovery and aesthetic-direction principles;
- wireframe and variation methods;
- design-token and component-system thinking;
- accessibility, hierarchy, interaction-state, and generic-pattern reviews;
- HTML as a capable medium for interactive prototypes and web-native presentations.

## Material changed

- Replaced the HTML-first environment assumption with medium selection and routing.
- Converted universal aesthetic prohibitions into context-dependent heuristics.
- Made design, implementation, review, and optimization separate operating modes.
- Removed references to unavailable host tools, starter components, tweak protocols, and verifier mechanisms.
- Removed mandatory variation counts and automatic tweak controls outside exploratory work.
- Prevented review-only requests from silently modifying files.
- Delegated PowerPoint, Figma, documents, PDFs, native applications, and images to their medium-specific workflows.
- Narrowed triggering to open, cross-stage, or cross-medium work so clear single-medium tasks can use their dedicated skills directly.
- Made explicit user intent take precedence over missing design context during stage selection.

## Files consulted

The adaptation was informed by the source repository's Codex variant, including its system prompt and the procedures for discovery, aesthetic direction, wireframes, variations, design-system extraction, component extraction, accessibility, generic-pattern review, hierarchy and rhythm, interaction states, prototypes, decks, tweak controls, and final polish.

