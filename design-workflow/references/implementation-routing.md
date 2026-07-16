# Implementation Routing

Use this reference after the design is sufficiently defined. Select the delivery medium from the user's explicit requirement first; use the decision factors below only when the medium is genuinely open.

## Routing table

| Medium | Prefer when | Route |
| --- | --- | --- |
| HTML/H5/web application | Interaction, live data, responsive behavior, link sharing, or browser-native delivery matters | Read `html-implementation.md`, then use the relevant frontend or site-building workflow |
| PowerPoint or Slides | Non-technical editing, corporate templates, speaker notes, meeting-room compatibility, or `.pptx` delivery matters | Use the installed presentation skill; do not substitute HTML without agreement |
| Figma or FigJam | Collaborative design review, component libraries, variables, prototyping, or developer handoff in Figma matters | Use the relevant Figma skill and its prerequisites |
| Word or PDF | Paginated reading, formal reports, print, redlining, or fixed-document delivery matters | Use the documents or PDF skill |
| Native application | Platform conventions, native navigation, device APIs, or store delivery matters | Use the relevant platform and code workflow |
| Static image | A single visual, illustration, poster, or raster deliverable is required | Use the appropriate image generation or editing workflow |

Do not choose HTML solely because the design can be represented in HTML. Choose it when browser delivery or web-native behavior is part of the value.

## Selection factors

When the medium is open, compare:

- required interactivity and live data;
- who must edit the result after delivery;
- collaboration and review environment;
- offline, projector, print, or device constraints;
- accessibility and platform expectations;
- required file type;
- deployment and maintenance ownership.

Recommend one medium and state the decisive trade-off. Present alternatives only when they remain genuinely competitive.

## Implementation handoff

Pass these decisions into the selected implementation workflow:

- selected medium and output file type;
- approved design decision record;
- source assets and design-system references;
- required interaction and content states;
- responsive, accessibility, print, or platform constraints;
- verification method;
- placeholders or external dependencies.

Once routed, let the medium-specific workflow control implementation details. This skill remains responsible for preserving the approved design intent and for invoking the appropriate quality gate at review or delivery.

## When the preferred capability is unavailable

Do not silently replace the selected medium with HTML or another convenient format. State which capability or dependency is unavailable and preserve the design decision record. Then provide the most useful non-surprising fallback within the user's scope, such as:

- a medium-neutral implementation specification;
- a content and layout outline ready for the intended tool;
- an asset and handoff checklist;
- an alternative medium only after the user agrees to the trade-off.

The fallback should help the intended delivery continue without pretending that a different file type is equivalent.

