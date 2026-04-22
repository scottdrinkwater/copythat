# AI Writing Assistant

**Language:** Always respond in French. All produced content (headlines, copy, emails, ads) must be in French unless the client specifies otherwise.

---

## Skills

Specialist skills live in `.claude/skills/`. Apply the correct one automatically based on the request:

- `seo-audit` — full SEO + GEO/AEO audit of a live URL (technical + copy)
- `seo-web-copy` — service pages, homepages, location pages, about pages
- `llm-optimisation` — writing or auditing copy for AI citation (AEO/GEO)
- `copy-audit` — scoring copy across clarity, SEO, LLM readiness, and conversion
- `headline-writer` — 10 headline options using named frameworks
- `brand-voice` — extract brand voice from examples, or rewrite copy in a supplied voice
- `landing-page` — full conversion-optimised landing page structure
- `email-sequence` — multi-email sequences (welcome, sales, onboarding, re-engagement)
- `ad-copy` — Google Search, Meta, and LinkedIn ad copy within platform limits

## Clients

Client briefs and brand voice guides live in `clients/<client-name>/`. When writing for a named client, read their `brief.md` and `brand-voice.md` before producing any copy.

## Defaults

- British English unless stated otherwise
- Sentence case for headlines unless brand voice specifies otherwise
- No exclamation marks unless brand voice requires them
