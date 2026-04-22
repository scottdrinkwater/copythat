# Skills & Agents

> 🇫🇷 [Version française](agents.md)

These are specialist tools built into Claude Code. Each one handles a specific copywriting job — just describe what you want and Claude will use the right one automatically.

## Writing Skills

These load automatically when you ask Claude to write or optimise something. You don't need to call them by name.

**SEO Audit**
What it does: full audit of a live URL — technical SEO, GEO/AEO readiness (AI citation signals), and a complete copy review. Checks title tag, meta description, heading structure, structured data, internal links, and performance signals. Produces a scored report with a top 5 priority list and quick wins.
How to use: "Audit this URL for SEO and AI optimisation: [url]"

**SEO Web Copy**
What it does: writes website copy that ranks — service pages, location pages, homepages, about pages. Includes title tag, meta description, H1, body copy, and FAQ section. Follows keyword hierarchy and E-E-A-T principles.
How to use: "Write a service page targeting 'freelance copywriter Manchester'. Audience: B2B tech companies."

**LLM Optimisation (AEO / GEO)**
What it does: writes or rewrites copy so it gets surfaced and cited by AI tools — ChatGPT, Perplexity, Google AI Overviews, Claude. Uses answer-first writing, definition blocks, self-contained FAQ answers, and entity clarity techniques.
How to use: "Optimise this service page so it's more likely to be recommended by AI tools."

**Copy Audit**
What it does: reviews existing copy across 7 dimensions: clarity, structure, tone, SEO, LLM readiness, conversion, and accuracy. Produces a scored report with top priorities and quick wins.
How to use: "Audit this homepage copy. Tell me what to fix for SEO and AI optimisation."

**Headline Writer**
What it does: generates 10 headline options using proven frameworks — PAS, AIDA, curiosity gap, benefit-led, specificity, contrarian, social proof, urgency. Labels each so you can see the approach.
How to use: "Give me 10 headline ideas for a landing page selling CRM software to estate agents."

**Brand Voice**
What it does: two modes — (A) extracts a brand voice from copy examples and produces a Brand Voice Card, or (B) rewrites copy in a supplied brand voice. Shows before/after when rewriting.
How to use: "Extract the tone of voice from these three web pages." or "Rewrite this in the Bloom Studio brand voice."

**Landing Page**
What it does: structures and writes a full landing page — hero, problem, solution, features/benefits, social proof, FAQ, pricing, and CTA — using a proven conversion sequence.
How to use: "Write a landing page for a website audit service targeting marketing managers."

**Email Sequence**
What it does: writes multi-email sequences — welcome, onboarding, sales/launch, or re-engagement. Each email includes subject line, preview text, body, and CTA.
How to use: "Write a 5-email welcome sequence for a B2B copywriting course."

**Ad Copy**
What it does: writes paid ad copy for Google Search, Meta (Facebook/Instagram), or LinkedIn. Respects platform character limits and formats. Produces multiple headline and description variations.
How to use: "Write Google search ads for this landing page. Primary keyword: 'SEO copywriter UK'."

## Reading Files

Drop any client file into this folder and ask Claude to read it.

- **PDF** — briefs, brand guides, research reports, contracts. e.g. "Read brief.pdf and pull out the key messages and target audience."
- **Word (.docx)** — client copy, feedback docs, previous drafts. e.g. "Read feedback.docx and tell me what changes the client wants."
- **Spreadsheet (.xlsx)** — keyword lists, content matrices, copy trackers. e.g. "Read keywords.xlsx and suggest which ones to target on the homepage."
- **Presentation (.pptx)** — brand decks, creative briefs, competitor research. e.g. "Read brand-guidelines.pptx and extract the tone of voice rules."

## Organisation & Memory

- `/anthropic-skills:consolidate-memory` — saves everything Claude has learned about your preferences and clients for future sessions.
- `/anthropic-skills:schedule` — set up a recurring task. e.g. "Every Friday, remind me to update my project tracker."

## Managing Clients

Each client has a folder under `clients/` containing two files:

- `brief.md` — business overview, audience, goals, target keywords
- `brand-voice.md` — tone rules, style preferences, words to avoid

**To add a new client:** copy an existing folder (e.g. `clients/apex-group/`), rename it, and fill in the two files.

**To write for a client:** mention them by name and Claude will read their files automatically.
> "Write a service page for Bloom Studio. Read their brief and brand voice first."

**To save copy drafts:** add them directly to the client folder.
> e.g. `clients/bloom-studio/homepage-v1.md`, `clients/apex-group/services-page.md`

**To update Claude's memory of a client mid-session:** just say it.
> "Remember that Apex Group never uses passive voice."
