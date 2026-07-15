# Lovable Landing Kit

Reusable Markdown guidance for discovering an existing product and creating an
intentional, product-led landing page in Lovable or another AI-assisted tool.

`landing-generator.md` is the master entry point. It discovers product context
from the current application, so this repository does not require a folder or
brief for every product. The two supporting directories keep stable rules and
repeatable workflows modular and maintainable.

## Structure

```text
lovable-landing-kit/
├── landing-generator.md
├── global/
│   ├── design-principles.md
│   ├── anti-ai-patterns.md
│   └── accessibility.md
└── workflows/
    ├── landing-page-process.md
    └── landing-page-review.md
```

## Responsibilities

- `landing-generator.md` discovers the product, classifies confidence, and
  orchestrates planning, implementation, and verification.
- `global/` contains stable constraints shared by every landing page.
- `workflows/` contains the detailed build sequence and final review checklist.

The master file references the supporting documents; they are not additional
inputs that must be recreated for each product.

## How to use it

Import the repository as a reusable skill or make its Markdown files available
to the current Lovable project. Then invoke the same instruction in each app:

```text
Use landing-generator.md to inspect this project and create its public landing
page. Do not create product documentation. Present the concise discovery summary
before implementation, then implement and review the result.
```

If the environment accepts only one document, use `landing-generator.md` by
itself. It contains a compact fallback for the essential design and review rules.

Only add a product-specific file later when important commercial context cannot
be discovered from the application and is reused often enough to justify it.
