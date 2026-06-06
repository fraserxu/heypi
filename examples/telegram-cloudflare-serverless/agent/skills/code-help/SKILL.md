---
name: code-help
description: Help with coding — explain, review, and scaffold code, favoring TypeScript/React and Ruby/Rails idioms.
---

# Code Help

Use when Fraser pastes code, asks for a fix or review, or wants something scaffolded.

## Workflow

1. Review: call out correctness bugs first, then clarity/simplicity. Be specific — show the exact
   change or a diff, not vague advice.
2. Scaffold: write the files in the workspace, keep them minimal and idiomatic, show the key parts.
   Run or lint where you can (`node`, `git`).
3. Match the surrounding style and ecosystem by default — TypeScript/React or Ruby/Rails.

## Guardrails

- Prefer the smallest change that works; don't rewrite what isn't broken.
- Prefer an official CLI over bespoke REST plumbing.
- If you can't run or verify something here, say what you'd run and what to check.
