# Landing Generator

## Purpose

Analyze the current existing application and create a product-specific landing
page without requiring a manually written product brief.

The current project is the source of truth for product facts. This file is the
master entry point for the discovery, design, implementation, and review process.

Do not create product documentation or analysis files unless the user explicitly
requests them.

## Supporting guidance

When the repository is available, read these files before implementation:

1. `global/design-principles.md`
2. `global/anti-ai-patterns.md`
3. `global/accessibility.md`
4. `workflows/landing-page-process.md`
5. `workflows/landing-page-review.md`

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

Keep this summary short and decision-oriented. Do not output a technical
inventory or create it as a file.

## Phase 5: Design and implement

Follow `workflows/landing-page-process.md` when available.

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
- Vary section composition according to content.
- Avoid generic centered heroes, decorative gradients, glowing shapes, repeated
  card grids, excessive pills, fake social proof, and unsupported claims.
- Describe business controls and outcomes instead of CRUD operations.
- Use motion only to explain state or progression.

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

## Phase 6: Verify

Use `workflows/landing-page-review.md` when available.

At minimum, verify:

- The page represents the actual product.
- Every claim is supported by the project or user-provided facts.
- Product evidence appears prominently.
- Copy explains business value rather than generic CRUD functionality.
- Sections do not repeat the same structure without a content reason.
- Existing routes and primary application flows still work.
- Keyboard, reduced-motion, mobile, and desktop behavior are usable.
- No fake testimonials, logos, metrics, customers, or integrations were added.

## Completion report

Report concisely:

- What was implemented.
- Which product evidence was used.
- What was verified.
- Any important information that remains uncertain.

Do not create new documentation files to store this report unless requested.
