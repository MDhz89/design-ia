# Lovable Design Library

Reusable Markdown guidelines for creating intentional, product-led landing
pages in Lovable and other AI-assisted development tools.

This repository is the source of truth for stable design principles and
repeatable landing-page workflows. It intentionally does not contain product
folders yet. Product-specific context should be added only when work begins on
the first real landing page.

## Structure

```text
lovable-design-library/
├── global/
│   ├── design-principles.md
│   ├── anti-ai-patterns.md
│   └── accessibility.md
└── workflows/
    ├── landing-page-process.md
    └── landing-page-review.md
```

## How to use it

1. Keep stable, cross-project decisions in `global/`.
2. Use the documents in `workflows/` when planning or reviewing a landing page.
3. Copy only the relevant guidance into Lovable Workspace Knowledge, Project
   Knowledge, or the current prompt.
4. Update these documents when a lesson applies to more than one product.

Avoid loading the entire repository into every prompt. Use only the documents
that are relevant to the current task.
