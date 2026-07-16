# Interaction and motion

## Contents

- Define interaction states
- Minimal interaction language
- Filters, tabs, and selectors
- Scroll-triggered reveals
- Narrative scroll moments
- Technical constraints
- Acceptance checks

Make the landing feel deliberately crafted through restrained interaction
detail and a small number of narrative motion moments. Never add effects only
to make the page look busier.

## Define interaction states

Before considering an interactive element complete, define the states relevant
to it:

- Default.
- Hover for pointer devices.
- Visible keyboard focus.
- Active or pressed.
- Selected or current.
- Disabled when appropriate.
- Loading, success, and error when an asynchronous action exists.

Do not make hover the only signal or the only way to reveal essential content.

## Minimal interaction language

Use a consistent combination of two or three signals across the page:

- Quiet one-pixel borders that gain contrast on hover or focus.
- Small background or text-color changes derived from existing tokens.
- Underline offset, arrow movement, or icon movement for text links.
- Subtle elevation or a one-to-two-pixel translation for actionable surfaces.
- Short opacity or transform transitions for state changes.

Avoid stacking scale, shadow, glow, rotation, color, and movement on the same
element. Avoid hover scaling that causes layout movement. A card should behave as
a clickable surface only when the entire card performs a real action.

Use glow as a restrained emphasis treatment, not as a default decoration. A
subtle brand-colored halo or border may distinguish one selected plan or CTA when
a fully inverted high-contrast surface would feel visually heavy.

## Filters, tabs, and selectors

- Implement filters and tabs only when they change real visible content.
- Make the selected state unmistakable without relying only on color.
- Preserve keyboard navigation and appropriate semantic state.
- Animate content replacement subtly; do not replay an entrance animation on
  every small interaction.
- Keep labels specific to the product rather than using generic categories.

## Scroll-triggered reveals

- Trigger once as content enters the viewport.
- Prefer opacity with a short 12–24px translation.
- Use restrained staggering only for genuinely related items.
- Keep content readable when JavaScript is unavailable.
- Disable or simplify the effect for reduced-motion preferences.

Do not animate every heading, paragraph, icon, and card independently.

## Narrative scroll moments

Reserve the strongest motion for one or two moments that explain value, such as:

- Revealing the real interface after stating the problem.
- Advancing through consecutive steps of the product workflow.
- Comparing the manual process with the controlled product state.
- Emphasizing product evidence immediately before the primary CTA.

For a scroll-linked zoom moment:

- Anchor the effect to meaningful product media or verified evidence.
- Start close to the final size; an approximately 8–12% scale change is enough.
- Use transforms instead of changing layout dimensions.
- Keep surrounding copy stable and readable.
- Define clear start and end points, then release normal page scrolling.
- Replace the effect with a static final state on small screens when necessary.

For sticky storytelling:

- Keep one stable visual while short steps update beside it.
- Synchronize the active step with a real interface state or product concept.
- Ensure the sticky section has a clear exit and does not obscure later content.
- Avoid long pinned sequences that make visitors feel trapped.

Never hijack scroll speed, replace native scrolling, or require precision
scrolling to access content.

## Technical constraints

- Reuse the animation tools already present in the project.
- Prefer CSS transitions and Intersection Observer for simple effects.
- Add a motion library only when the approved interaction cannot be implemented
  reliably with the existing stack.
- Animate transform and opacity where possible.
- Verify performance on mobile and prevent cumulative layout shift.
- Respect `prefers-reduced-motion` for every non-essential effect.

## Acceptance checks

- Interactions communicate action, hierarchy, selection, or progression.
- Pointer, keyboard, touch, and reduced-motion experiences remain complete.
- The page contains at least one considered interaction detail when appropriate,
  but no section depends on decoration to be understandable.
- The strongest motion moment reinforces a specific claim or conversion step.
