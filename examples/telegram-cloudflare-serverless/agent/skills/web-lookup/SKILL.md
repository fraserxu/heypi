---
name: web-lookup
description: Look up current information from the web by fetching pages or APIs with curl and summarizing, with sources.
---

# Web Lookup

Use when Fraser asks for current info, documentation, prices, news, an API result, or anything that
needs the internet.

## Workflow

1. Pick the most direct source — official docs/API first, then a reliable page.
2. Fetch with `curl`, e.g. `curl -sL "<url>"` (add `-H 'accept: application/json'` for APIs); pipe
   JSON through `jq`.
3. For HTML-heavy pages, extract the relevant text rather than dumping the whole document.
4. Answer concisely, then cite the URL(s) you used.

## Guardrails

- Don't fabricate facts you couldn't fetch — say if a source was unreachable or blocked.
- Never send Fraser's secrets or environment values to third parties.
- Prefer official / first-party sources over SEO filler.
