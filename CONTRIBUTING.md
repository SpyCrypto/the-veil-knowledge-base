# Contributing to the-veil-knowledge-base

Thanks for your interest in contributing — we welcome improvements, research,
and community resources. This document explains the quickest path to a
successful contribution.

Where to start
- Read this README and [STRUCTURE.md](STRUCTURE.md) to understand repository
  layout and where content should live.
- Check open issues and discussions to find active work and avoid duplication.

Onboarding checklist
- [ ] Read README.md and [STRUCTURE.md](STRUCTURE.md).
- [ ] Browse existing issues and discussions to find active work.
- [ ] Introduce yourself in Discussions (optional) and state your interest area.
- [ ] Make a small contribution (typo fix, doc improvement) to get familiar with
  the flow.
- [ ] Open a PR and request a reviewer.

How to contribute
1. Fork the repository and create a topic branch for your change.
2. Add or edit files in the appropriate folder under `the-veil/` (see
   STRUCTURE.md for details).
3. Use clear file names and include front-matter metadata if the content type
   uses it (title, authors, date, tags).
4. Commit with a descriptive message and open a Pull Request that explains the
   motivation and scope of the change.

Pull request checklist
- [ ] I read [STRUCTURE.md](STRUCTURE.md) and placed files in the correct
  folder.
- [ ] I added or updated documentation where relevant.
- [ ] I validated that no sensitive information is included.
- [ ] I provided a clear PR description and linked any related issues.

Formatting and front-matter example

For research notes and documents we recommend a simple YAML front-matter at the
top of Markdown files. Example:

---
title: "Understanding X"
author: "Name"
date: 2026-06-19
tags: [research, privacy]
---

Contribution examples
- Add a research note: `the-veil/research/<topic>/YYYY-MM-DD-title.md` with
  front-matter and a descriptive filename.
- Propose a framework: `the-veil/frameworks/<framework-name>/README.md` plus
  examples or diagrams in the same folder.
- Media assets: `the-veil/media/<type>/` (logos, diagrams) and reference them in
  the relevant docs.

If you're unsure where something belongs, open an issue or start a discussion
— maintainers will help you find the right place.
