# Accessibility

## Baseline

Treat accessibility as a design and implementation requirement from the start,
not as a final cleanup task.

## Structure and semantics

- Use semantic HTML landmarks and native elements whenever possible.
- Provide one descriptive `h1` and maintain a logical heading hierarchy.
- Keep reading order consistent with the visual order.
- Give links and buttons descriptive, distinct labels.
- Associate every form control with a visible label.
- Provide useful alternative text for informative images.
- Mark purely decorative images so assistive technology can ignore them.

## Keyboard and focus

- Make every interactive element reachable and operable with a keyboard.
- Preserve a clearly visible focus indicator.
- Keep focus order predictable.
- Do not create keyboard traps.
- Move or restore focus deliberately when dialogs and menus open or close.

## Color and typography

- Maintain sufficient text and interface contrast.
- Never use color as the only way to communicate meaning or state.
- Keep body text comfortably readable across viewport sizes.
- Allow text zoom and reflow without hiding content or controls.
- Do not place essential text inside images.

## Motion and media

- Respect the `prefers-reduced-motion` setting.
- Avoid flashes and continuous decorative motion.
- Do not autoplay media with sound.
- Provide captions or transcripts when the content requires them.

## Responsive behavior

- Verify content at narrow, medium, and wide viewports.
- Keep touch targets comfortably sized and separated.
- Avoid horizontal scrolling for normal page content.
- Ensure sticky elements do not obscure content or keyboard focus.

## Final checks

- Navigate the entire page using only a keyboard.
- Check headings, landmarks, names, roles, and states.
- Test zoom, text resizing, reduced motion, and high-contrast conditions.
- Run automated checks, then verify important flows manually.
