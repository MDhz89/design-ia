---
name: landing-generator
description: Use when analyzing an existing Lovable application to plan, build, visually audit, or review a public product landing page from its code, rendered UI, or screenshots, including requests to detect AI-generic patterns and propose a more authored direction without implementation; not for greenfield apps, unrelated feature work, or generic marketing pages without an existing product.
---

# Landing Generator

## Purpose

Analyze the current existing application and create a product-specific landing
page without requiring a manually written product brief.

The current project is the source of truth for product facts. This file is the
master entry point for the discovery, design, implementation, and review process.

Do not create product documentation or analysis files unless the user explicitly
requests them.

## Supporting guidance

Load supporting references only when their phase requires them:

- Read `references/design-principles.md` and
  `references/anti-ai-patterns.md` while planning the narrative and visual
  direction.
- Read `references/brand-hierarchy-and-composition.md` when selecting logo
  variants, assigning brand colors, sizing metrics, ordering text and product
  evidence, or emphasizing plans and CTAs.
- Read `references/authorship-and-art-direction-audit.md` when auditing a
  rendered landing, reviewing screenshots, diagnosing why a page feels
  AI-generated, or proposing a more product-specific visual direction.
- Read `references/accessibility.md` before implementation and verification.
- Read `references/landing-page-process.md` after discovery, when planning or
  implementing the page.
- Read `references/interaction-and-motion.md` when defining hover states,
  filters, product reveals, sticky sections, or scroll-linked storytelling.
- Read `references/conversion-actions.md` when selecting or implementing the
  primary CTA, forms, WhatsApp links, phone links, or other lead-capture paths.
- Read `references/landing-page-review.md` when reviewing an existing result or
  performing final verification.

They extend this master procedure and must not be treated as separate product
inputs. If only this file is available, follow the essential rules included
below and continue without blocking.

## Instruction precedence

When instructions appear to conflict, use this order:

1. The user's explicit request.
2. Verified facts and constraints in the current application.
3. This master procedure.
4. Global design and accessibility rules.
5. Workflow defaults.

Accessibility and truthful product representation are never optional. Existing
visual patterns may be improved when they reduce clarity, accessibility, or
landing-page effectiveness.

## Operating principles

- Inspect before designing or changing code.
- Infer what the project supports; do not invent what it does not reveal.
- Do not ask the user for information that can be discovered reliably.
- Do not create a permanent brief, copy file, or design-direction file.
- Keep discovery notes in the current task only.
- Ask only for missing information that would materially change the result.
- Do not block implementation for minor marketing details.
- Reuse the existing stack, components, terminology, and visual identity when
  they are suitable.

## Select the operating mode

Infer the mode from the user's instruction:

- **Discover and plan:** inspect the application and propose the landing before
  implementation.
- **Build:** implement an approved or sufficiently defined landing direction.
- **Audit and propose:** inspect an existing rendered landing or screenshots,
  diagnose generic patterns, and propose prioritized changes without modifying
  files.
- **Review and correct:** inspect, implement approved corrections, and verify the
  completed result.

When the user asks to analyze, evaluate, diagnose, critique, or propose, use
**Audit and propose** and do not modify code. End with a concrete proposal that
can be approved and implemented in a later message.

## Phase 1: Project discovery

Inspect the project systematically without modifying code.

Read, when available:

1. README files and existing documentation.
2. Project configuration and dependencies.
3. Routes, navigation, and public or authenticated layouts.
4. Main pages and shared components.
5. Types, models, schemas, and database definitions.
6. API services, queries, mutations, and server functions.
7. Forms, validation rules, calculations, and state transitions.
8. Authentication, roles, permissions, and feature guards.
9. Dashboards, reports, tables, audit history, and status views.
10. Design tokens, typography, icons, images, and other brand assets.
11. Available logo variants, including wordmarks, isotypes, horizontal lockups,
    light and dark versions, and their existing usage.

Focus on behavior that is implemented, not merely named or suggested.

## Phase 2: Build a temporary product model

Infer the smallest useful model needed to design the landing:

### Product and audience

- What the application actually does.
- What business process it supports.
- Primary operational users.
- Likely buyer or decision-maker.
- Previous manual process or business problem, when supported.
- Primary conversion action, when supported.
- Verified conversion channels and where submitted lead data can be delivered.

### Workflow and value

- Core workflow from entry to completion.
- Main modules and entities.
- Important roles, permissions, validations, and state transitions.
- Automation, calculations, reporting, and operational visibility.
- Errors, delays, or risks the implemented rules help prevent.

### Product evidence

- Interface screens that can demonstrate the workflow.
- Real dashboards, tables, forms, charts, states, and audit views.
- Existing metrics calculated by the application.
- Visual assets that belong to the actual product.

Never invent customers, testimonials, logos, integrations, metrics, industries,
or results.

## Phase 3: Classify confidence

Classify conclusions internally:

- **Confirmed:** directly visible in code, UI, data models, or documentation.
- **Strong inference:** supported by multiple project signals.
- **Uncertain:** cannot be established reliably from the project.

Use confirmed facts freely. Phrase strong inferences carefully. Do not turn
uncertain conclusions into marketing claims.

If a critical uncertainty would change the audience, proposition, CTA, or page
architecture, ask one concise grouped question. Otherwise proceed and list the
uncertainty at the end.

## Phase 4: Present a concise discovery summary

Before implementation, present:

1. Product definition.
2. Primary user and likely buyer.
3. Business problem and main workflow.
4. Most relevant business rules or differentiators.
5. Product evidence available for the page.
6. Critical uncertainty, if any.
7. Proposed landing narrative and sections.
8. Proposed CTA behavior and any data or destination it still requires.
9. Proposed brand hierarchy, including logo usage, dominant accent color, and
   the elements that should receive or surrender visual emphasis.

Keep this summary short and decision-oriented. Do not output a technical
inventory or create it as a file.

## Phase 5: Design and implement

Follow `references/landing-page-process.md` when available.

Base the narrative on the discovered workflow. A useful default is:

1. Specific product proposition.
2. Recognizable business problem.
3. Real product demonstration.
4. Main workflow.
5. Important controls or business rules.
6. Operational visibility or supported outcomes.
7. Final call to action.

Change the sequence when the actual product suggests a clearer story. Every
section must have a distinct purpose.

### Essential design rules

- Prefer product evidence, typography, spacing, and composition over decoration.
- Use the existing visual identity when it is coherent and accessible.
- Select logo variants for legibility rather than shrinking one asset into every
  placement.
- Establish one dominant brand accent and use secondary colors intentionally.
- Keep labels, section numbers, metrics, prices, and badges subordinate to the
  message unless one of them is the actual evidence being sold.
- Place explanatory content before its visual evidence in the reading order
  unless the narrative provides a specific reason to reverse it.
- Vary section composition according to content.
- Avoid generic centered heroes, decorative gradients, glowing shapes, repeated
  card grids, excessive pills, fake social proof, and unsupported claims.
- Describe business controls and outcomes instead of CRUD operations.
- Design deliberate hover, focus, active, selected, loading, and disabled states.
- Reserve strong scroll motion for one or two narrative moments with clear value.
- Use motion only to explain state, progression, hierarchy, or product behavior.

### Implementation constraints

- Preserve existing application routes, authentication, and business flows.
- Prefer a dedicated public route unless the project already defines another
  appropriate entry point.
- Reuse the current stack and component system.
- Do not replace dependencies or add a UI framework without a clear need.
- Use semantic HTML and visible keyboard focus.
- Respect reduced-motion preferences.
- Ensure responsive behavior without hiding essential content or actions.
- Avoid unnecessary asset weight and runtime complexity.
- Do not leave any CTA, navigation item, or interactive control without a real
  destination, state change, or verified action.

## Phase 6: Verify

Use `references/landing-page-review.md` when available.

At minimum, verify:

- The page represents the actual product.
- Every claim is supported by the project or user-provided facts.
- Product evidence appears prominently.
- Brand assets remain recognizable and visual emphasis follows the intended
  reading order.
- Copy explains business value rather than generic CRUD functionality.
- Sections do not repeat the same structure without a content reason.
- Existing routes and primary application flows still work.
- Every CTA completes a real and tested conversion path.
- Hover, focus, filter, scroll, and form interactions work as intended.
- Keyboard, reduced-motion, mobile, and desktop behavior are usable.
- No fake testimonials, logos, metrics, customers, or integrations were added.

## Audit an existing landing

When using **Audit and propose**, inspect the rendered page, supplied screenshots,
and relevant source when available. Follow
`references/authorship-and-art-direction-audit.md`.

Return:

1. The current first impression.
2. What already works and should be preserved.
3. The exact pattern clusters that create an AI-generated impression.
4. The interchangeability result: what could belong to an unrelated product.
5. The product-specific visual idea currently missing.
6. A prioritized proposal for composition, typography, evidence, brand, motion,
   and conversion.
7. Risks and information or assets required before implementation.

Do not return vague advice such as “make it more modern,” “add personality,” or
“improve hierarchy.” Tie every recommendation to observed evidence and describe
the intended perceptual effect.

## Completion report

Report concisely:

- What was implemented.
- Which product evidence was used.
- What was verified.
- Any important information that remains uncertain.

Do not create new documentation files to store this report unless requested.
