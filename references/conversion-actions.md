# Conversion actions

## Objective

Make every call to action complete a real, testable next step. Never ship a
button that exists only visually.

## Select the conversion path

Inspect the project and user-provided context before choosing CTA behavior. Use
the first verified option that matches the commercial objective:

1. Existing booking, contact, signup, or demo route.
2. Existing form and submission service.
3. A minimal lead form connected to an available backend or verified service.
4. A verified WhatsApp, phone, email, or calendar destination.
5. A concise question to the user when no real destination can be discovered.

Do not invent a phone number, email address, booking URL, API endpoint, database
table, or message recipient. Do not use `href="#"`, empty click handlers, or fake
success messages as substitutes.

## Demo request behavior

When “Request a demo” is the primary CTA, choose one complete behavior:

### Accessible modal or inline form

- Request only information needed for the next contact, normally name and one
  verified contact method.
- Add company or role only when it affects qualification.
- Use visible labels, clear validation, and actionable error messages.
- Define disabled, loading, success, retry, and server-error states.
- Move focus into an opened dialog and restore it when the dialog closes.
- Support Escape and an explicit close control.
- State what happens after submission.
- Submit to a real endpoint, database action, email service, or automation.

If no submission destination exists, ask for it before implementing the form.
Do not collect information that is discarded.

### WhatsApp

- Use only a confirmed business number in international digits-only format.
- Build a `https://wa.me/<number>?text=<encoded-message>` URL.
- Prefill a short message that names the product and visitor intent.
- Open external navigation safely and keep the CTA understandable without the
  WhatsApp icon.
- Verify the generated link on mobile and desktop.

### Phone, email, calendar, or internal route

- Use `tel:` and `mailto:` only with confirmed destinations.
- Use an existing booking URL rather than fabricating availability.
- Verify that internal routes exist and render without authentication when the
  landing visitor must access them.

## CTA hierarchy

- Use one primary conversion goal throughout the page.
- Keep CTA wording consistent unless a later label describes a more specific
  step.
- Give secondary actions a distinct purpose, such as viewing the product or
  contacting sales through another verified channel.
- Do not place two visually equal actions together without a clear priority.
- Repeat the primary CTA only at meaningful decision points.

## Forms and trust

- Keep required fields minimal.
- Explain why sensitive or unusual information is required.
- Do not add consent text, response-time promises, or privacy claims that cannot
  be supported.
- Preserve entered values after recoverable submission errors.
- Prevent accidental duplicate submissions.
- Never show success until the destination confirms acceptance.

## Acceptance checks

- Activate every CTA and verify its destination or resulting state.
- Complete form validation, successful submission, and failure recovery.
- Test external links and encoded messages.
- Test keyboard and mobile interaction.
- Confirm that lead data reaches the intended verified destination.
- Treat any dead button or simulated success as a blocking defect.
