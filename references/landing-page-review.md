# Landing page review

## Purpose

Use this checklist after each meaningful implementation stage and before the
landing page is considered complete.

For a diagnosis-only request, first apply
`authorship-and-art-direction-audit.md` and do not implement corrections until
the user approves a direction.

## Product and message

- Identify the buyer, user, problem, and primary action from the first screen.
- Confirm that the page describes business outcomes rather than CRUD features.
- Verify that each important claim is supported by real product evidence.
- Remove invented customers, testimonials, metrics, integrations, or outcomes.
- Check that terminology matches the product and its users.

## Narrative

- Give every section a distinct purpose.
- Remove sections that repeat an earlier claim.
- Confirm the section order builds a coherent argument.
- Show the product before the first major scroll when suitable evidence exists.
- Make the primary conversion action clear and consistent.

## Visual design

- Identify generic AI-generated patterns using `anti-ai-patterns.md`.
- Evaluate authorship, product specificity, controlled asymmetry, and the first
  viewport using `authorship-and-art-direction-audit.md`.
- Apply `brand-hierarchy-and-composition.md` to logo placement, color balance,
  metric scale, reading order, process continuity, plans, and final CTA.
- Check hierarchy, rhythm, alignment, density, and readable line lengths.
- Look for excessive cards, pills, gradients, containers, and decorations.
- Verify that repeated components contain genuinely comparable information.
- Check that no section number, commission, price, badge, or decorative label
  overwhelms the brand message without a deliberate reason.
- Check that compact logo placements use an asset that remains recognizable.
- Recommend removals before additions.

## Interaction and accessibility

- Apply `interaction-and-motion.md` to review borders, hover states, filters,
  scroll effects, and product demonstrations.
- Test keyboard navigation and visible focus.
- Verify semantic headings, landmarks, labels, and alternative text.
- Confirm sufficient contrast and non-color state indicators.
- Respect reduced-motion preferences.
- Check interactive states: hover, focus, active, disabled, loading, and error.
- Confirm scroll effects support the narrative, release cleanly, and never trap
  or hijack normal scrolling.

## Conversion path

- Apply `conversion-actions.md` to every primary and secondary CTA.
- Reject buttons with empty handlers, placeholder links, or destinations that do
  not exist.
- Verify forms have a real submission destination and complete loading, success,
  validation, and error states.
- Verify WhatsApp, phone, email, calendar, and internal links use real confirmed
  destinations.
- Complete the primary conversion flow on mobile and desktop.

## Responsive behavior

Review at minimum around these viewport widths:

- 375px: narrow mobile.
- 768px: tablet or compact layout.
- 1440px: wide desktop.

Check for overflow, awkward wrapping, hidden actions, oversized headings,
overlapping sticky elements, and loss of reading order.

## Quality and delivery

- Verify links, forms, analytics hooks when present, and the complete conversion
  path.
- Check loading performance and unnecessary asset weight.
- Review page title, description, social metadata, and heading structure.
- Confirm there are no console errors or broken assets.
- Record reusable findings in the global library only when they apply across
  multiple products.
