# AI Writing Assistant

> 🇫🇷 [Version française](README.md)

Your Claude Code workspace for website copywriting, SEO, and LLM optimisation.

## Installation

**Option 1 — Direct download (recommended)**

1. Download the ZIP from the [latest release](https://github.com/scottdrinkwater/copythat/releases/latest) (click "Source code (zip)")
2. Unzip the folder
3. Open [Claude Code](https://claude.com/claude-code), then open that folder

All skills are ready to use immediately — no additional setup needed.

**Option 2 — Via Git (technical users)**

```bash
git clone git@github.com:scottdrinkwater/copythat.git
cd copythat
```

## What Claude can help with

- Write service pages, homepages, about pages, location pages
- Write and optimise copy for SEO — keywords, title tags, meta descriptions, FAQs
- Optimise pages to be cited by AI tools (ChatGPT, Perplexity, Google AI Overviews)
- Audit existing copy for clarity, SEO, LLM readiness, and conversion
- Write landing pages, email sequences, and ad copy
- Extract or apply a client's brand voice
- Read PDFs, Word docs, spreadsheets, and presentations

See [docs/agents.en.md](docs/agents.en.md) for the full list of skills and how to trigger them.

## How to talk to Claude

Just describe what you want. The more context you give, the better the output.

**Good prompts:**
- "Write a service page for a B2B copywriting agency targeting 'website copywriter for tech companies'. Tone: confident and direct."
- "Read brief.pdf and suggest a page structure with H1, H2s, and key messages."
- "Audit this homepage copy for LLM readiness. Tell me the top 3 things to fix."
- "Rewrite this opening paragraph so it answers the search query directly."

**Less useful:**
- "Write something good" — too vague
- "Fix this" — paste the copy and say what's wrong

## Managing clients

Each client has a folder in `clients/` with two files:

- `brief.md` — business overview, audience, goals, target keywords
- `brand-voice.md` — tone rules, style preferences, words to avoid

To add a new client, copy an existing folder, rename it, and fill in the files. Mention the client by name and Claude will read their files automatically.

**Example:** "Write a homepage for Apex Group. Read their brief and brand voice first."

Copy drafts can live in the client folder too — e.g. `clients/apex-group/homepage-v1.md`.

## Tips

- Paste copy directly into the chat — Claude will work with whatever you give it
- Tell Claude the target keyword, the audience, and the tone upfront
- If you don't like the output: "make it shorter", "more direct", "try a different angle"
- Use "Remember that [client] prefers..." to save preferences for future sessions
