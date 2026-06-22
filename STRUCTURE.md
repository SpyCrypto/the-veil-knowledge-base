# Repository Structure & Contribution Guidelines

This document describes the canonical folder layout for The Veil Knowledge Base and guidance for organizing contributions.

## Directory Layout

```
the-veil-knowledge-base/
├── README.md                    # Main entry point
├── STRUCTURE.md                 # This file
├── SUMMARY.md                   # GitBook table of contents
├── book.json                    # GitBook configuration
├── CODE_OF_CONDUCT.md          # Community standards
├── CONTRIBUTING.md             # Contribution guidelines
├── LICENSE                      # Repository license
├── SECURITY.md                  # Security policy
├── the-veil/
│   ├── README.md               # Veil project overview
│   ├── manifesto/
│   │   ├── README.md
│   │   └── manifesto.md        # Core manifesto document
│   ├── research/
│   │   ├── README.md           # Research index
│   │   ├── topic-name/
│   │   │   ├── README.md       # Topic overview
│   │   │   └── study-name.md   # Individual research
│   │   └── ...
│   ├── frameworks/
│   │   ├── README.md           # Frameworks index
│   │   ├── framework-name/
│   │   │   ├── README.md       # Framework description
│   │   │   ├── architecture.md
│   │   │   ├── examples/
│   │   │   └── diagrams/
│   │   └── ...
│   ├── community/
│   │   ├── README.md
│   │   ├── case-studies/
│   │   └── resources/
│   ├── media/
│   │   ├── logos/
│   │   ├── diagrams/
│   │   └── images/
│   └── discussions/
│       └── README.md           # Links to GitHub Discussions
└── .github/
    └── workflows/              # CI/CD automation
```

## Content Guidelines

### Research Files
- **Location:** `the-veil/research/<topic>/`
- **Naming:** Use hyphens for spaces (e.g., `cryptographic-methods.md`)
- **Front-matter (optional):**
  ```yaml
  ---
  title: "Your Research Title"
  author: "Your Name"
  date: "YYYY-MM-DD"
  tags: ["tag1", "tag2"]
  ---
  ```
- **Structure:** H1 title, introduction, sections, references
- **Length:** 500–5000 words recommended

### Framework Files
- **Location:** `the-veil/frameworks/<framework-name>/`
- **Must include:**
  - `README.md` — overview and use cases
  - `architecture.md` — design and components
  - Examples or diagrams subdirectory
- **Front-matter:**
  ```yaml
  ---
  title: "Framework Name"
  version: "1.0"
  author: "Author Name"
  date: "YYYY-MM-DD"
  ---
  ```

### Media Assets
- **Location:** `the-veil/media/<category>/`
- **Categories:** `logos/`, `diagrams/`, `images/`, `videos/` (as needed)
- **Naming:** Descriptive, lowercase with hyphens (e.g., `veil-logo-dark.png`)
- **Format:** PNG, SVG, JPG preferred; PDFs for documents

## Contribution Workflow

1. **Fork the repository** and clone locally.
2. **Create a feature branch:** `git checkout -b add/your-contribution`
3. **Add your content** following structure guidelines above.
4. **Test locally** (see below).
5. **Commit with clear messages:** `git commit -m "Add research on [topic]"`
6. **Push and open a PR** with a description of changes.
7. **Wait for review** and address feedback.

## Local Testing

### Build GitBook Locally
```bash
# Install dependencies (if using Node.js)
npm install

# Serve locally (watch for changes)
gitbook serve

# Build static HTML
gitbook build
```

### View in Browser
- Open `http://localhost:4000` after running `gitbook serve`
- Changes auto-reload as you edit files

## Naming Conventions

- **Files:** lowercase, hyphens for spaces (e.g., `cryptographic-methods.md`)
- **Directories:** lowercase, hyphens for spaces (e.g., `case-studies/`)
- **Titles (in files):** Title Case
- **Tags:** lowercase, meaningful (e.g., `cryptography`, `frameworks`)

## Front-Matter Best Practices

Use front-matter (YAML) at the top of files to add metadata:

```yaml
---
title: "Document Title"
author: "Your Name"
date: "2026-06-22"
tags: ["research", "cryptography"]
status: "draft" # or "published"
---

# Document Title

Your content here...
```

Status field helps track work-in-progress vs. published content.

## Review Checklist

Before submitting a PR:
- [ ] Content follows naming conventions
- [ ] Front-matter is complete (if applicable)
- [ ] Markdown is valid (headers, links, lists)
- [ ] External links are active
- [ ] No sensitive information included
- [ ] Contribution follows Code of Conduct

## Questions?

- Open an **Issue** for structure questions or clarifications
- Use **Discussions** for brainstorming new sections
- Contact maintainers for governance questions

---

Thank you for contributing to The Veil Knowledge Base!
