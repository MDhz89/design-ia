# Authorship and art-direction audit

## Contents

- Objective
- Inputs and evidence
- Diagnose the first viewport
- Detect generic pattern clusters
- Run the interchangeability test
- Find the product-specific visual idea
- Evaluate controlled imperfection
- Propose a direction
- Output format
- Acceptance checks

## Objective

Determine whether an existing landing feels specifically art-directed for its
product or merely like a polished version of a familiar AI-generated template.
Produce an actionable proposal without editing the project.

Do not equate “human” with messy, vintage, serif, beige, hand-drawn, or
deliberately broken. Human authorship appears when the composition contains
specific, defensible decisions that emerge from the product, brand, audience,
and evidence.

## Inputs and evidence

Inspect as many of these as are available:

- Desktop and mobile renders.
- Screenshots supplied by the user.
- The live preview.
- Existing application screens.
- Logo and brand assets.
- Typography and design tokens.
- Product terminology, workflows, and business rules.
- CTA destinations and conversion behavior.

Separate direct observations from inferred intentions. Do not diagnose sections
that are not visible as if they had been inspected.

## Diagnose the first viewport

Treat the first viewport as a designed composition, not a checklist of required
hero components.

Identify:

- The element that receives attention first.
- The intended primary message.
- The dominant product evidence.
- The path the eye follows through message, evidence, and action.
- Whether the brand is recognizable before reading the product name.
- Which elements compete without adding meaning.
- Whether the composition could survive with fewer elements.

State the first impression in plain language, for example:

- “Professional and clear, but interchangeable with another B2B SaaS.”
- “Highly branded, but the product itself is difficult to understand.”
- “Visually distinctive, but the conversion action is subordinate.”

## Detect generic pattern clusters

Use `anti-ai-patterns.md`. Diagnose combinations, not isolated conventions.

Common clusters include:

### Assembled SaaS hero

- Pill badge.
- Oversized bold sans-serif headline.
- Accent-colored phrase.
- Explanatory paragraph.
- Filled and outlined CTA pair.
- Check-mark benefit row.
- Floating dashboard or browser window.

### Over-systemized composition

- Perfect 50/50 columns.
- Every element aligned to the same grid.
- Equal spacing between all content groups.
- Repeated card radius, border, shadow, and icon treatment.
- No deliberate interruption, overlap, crop, or density change.

### Generic product evidence

- Full dashboard shown at a distance.
- Browser chrome added without narrative value.
- Small UI details that cannot be read.
- Product mockup used as decoration rather than proof.
- Metrics or cards that could belong to another application.

### Cosmetic differentiation

- A generic layout differentiated only through color.
- Gradients applied to headline fragments without semantic meaning.
- Decorative motion added after the composition is already generic.
- Brand assets placed in the header but absent from the visual language.

Explain which cluster is present, which elements create it, and why the
combination affects perception.

## Run the interchangeability test

Mentally replace:

- Product name.
- Accent color.
- Headline nouns.
- Dashboard screenshot.

Then ask whether the structure could sell inventory software, a clinic platform,
logistics software, or another unrelated SaaS with minimal changes.

If yes, identify which parts are interchangeable. Do not conclude that the
product itself is generic; conclude that the presentation has not extracted
enough product-specific visual logic.

## Find the product-specific visual idea

Extract one central visual idea from implemented product behavior or evidence.
It should be difficult to reuse for an unrelated product.

Potential sources:

- A transformation from the previous manual process to the controlled state.
- A signature business rule or state transition.
- A product object, document, route, map, ticket, record, timeline, or report.
- A distinctive search, approval, assignment, calculation, or audit interaction.
- A real interface moment that demonstrates the main promise.
- Domain-specific structure, language, density, or material cues.

Express the idea as a relationship, not a decorative motif:

- “The physical archive resolves into searchable layers.”
- “The route becomes progressively controlled as each state is confirmed.”
- “The scattered requests converge into one auditable sequence.”

Do not turn domain clichés into decoration. Avoid literal gavels, clouds, gears,
rockets, floating folders, or stock illustrations unless they are real product
evidence or essential to the brand.

## Evaluate controlled imperfection

Look for one deliberate break from the default system:

- Composed line breaks rather than automatic wrapping.
- An intentional crop or overlap.
- A section whose density differs for narrative reasons.
- Asymmetric allocation of space.
- A product visual that escapes or interrupts the grid.
- A typographic contrast tied to meaning.
- An unusual alignment that strengthens reading order.

The break must remain:

- Legible.
- Accessible.
- Stable across responsive layouts.
- Consistent with the brand.
- Explainable in terms of hierarchy or narrative.

Do not recommend randomness, inconsistent spacing, arbitrary rotation, fake
handmade effects, or reduced usability. Controlled imperfection is selective
authorship, not simulated incompetence.

## Propose a direction

Recommend the smallest set of high-impact changes that create a new composition.
Prioritize in this order:

1. Product-specific visual idea.
2. First-viewport composition and reading path.
3. Product evidence selection and crop.
4. Typographic behavior and intentional line breaks.
5. Brand hierarchy and color ownership.
6. CTA hierarchy and real conversion behavior.
7. One controlled interaction or motion moment.
8. Supporting polish.

Avoid proposing only cosmetic substitutions such as changing the font, removing
the badge, adding texture, or making the screenshot larger. State how the pieces
combine into one direction.

Do not copy the surface style of a reference image. Extract the relevant
principle—such as asymmetric balance, editorial typography, dominant imagery, or
controlled tension—and reinterpret it through the actual product.

## Output format

Use this structure for audit-only requests:

### Diagnosis

One concise paragraph describing the current perception.

### Preserve

List the strongest existing decisions that should remain.

### Generic signals

For each detected cluster, provide:

- Observed evidence.
- Why it feels interchangeable or AI-coded.
- Severity: high, medium, or low.

### Missing authorship

Describe the product-specific visual idea that the page has not yet expressed.

### Proposed direction

Describe one coherent direction, including:

- Composition.
- Reading order.
- Typography.
- Product evidence.
- Brand behavior.
- CTA.
- Motion or interaction.

### Priorities

Separate:

- Structural changes.
- Supporting refinements.
- Optional experiments.

### Required inputs

List only missing assets or commercial decisions that materially affect the
proposal.

End by stating that no files were modified.

## Acceptance checks

- The diagnosis cites visible evidence rather than personal taste alone.
- Genericity is attributed to a pattern cluster, not one common component.
- The proposal includes an idea specific to the product.
- The direction changes composition, not only styling.
- At least one existing strength is preserved.
- Controlled imperfection remains functional and accessible.
- Recommendations are prioritized and implementable.
- No files are modified during an audit-only request.
