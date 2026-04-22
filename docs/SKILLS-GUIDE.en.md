# Skills Guide

> 🇫🇷 [Version française](SKILLS-GUIDE.md)

This guide explains the copywriting skills available in this project, how to use them, and how to modify or create new ones.

### What is a "Skill"?

A skill is a set of specialized instructions that tells Claude how to accomplish a specific task. For example, the "SEO Web Copy" skill knows how to structure a web page for search rankings.

You don't need to know technical details — just ask Claude what you want and it automatically uses the right skill.

---

## The Copywriting Skills

### 1. **SEO Web Copy** — Write pages that rank

**What it does:** Writes content for service pages, homepages, about pages, location pages. Includes title tags, meta descriptions, and SEO-optimized FAQ sections.

**How to use:**
```
Write a service page targeting 'copywriting agency London'. Audience: B2B tech agencies.
```

**Skill file:** `.claude/skills/seo-web-copy.md`

---

### 2. **LLM Optimisation (AEO/GEO)** — Optimize for ChatGPT, Perplexity, Google AI

**What it does:** Rewrites content so it gets cited and surfaced by AI tools (ChatGPT, Perplexity, Google AI Overviews). Uses techniques like answer-first writing, definition blocks, and entity clarity.

**How to use:**
```
Optimise this service page so it's more likely to be recommended by AI tools.
```

**Skill file:** `.claude/skills/llm-optimisation.md`

---

### 3. **Copy Audit** — Complete content audit

**What it does:** Reviews content across 7 dimensions: clarity, structure, tone, SEO, AI readiness, conversion, and accuracy. Produces a scored report with top priorities.

**How to use:**
```
Audit this homepage copy. Tell me what to fix for SEO and AI optimisation.
```

**Skill file:** `.claude/skills/copy-audit.md`

---

### 4. **Headline Writer** — Generate 10 headline options

**What it does:** Creates 10 different headlines using proven frameworks (PAS, AIDA, curiosity gap, benefit-led, specificity, contrarian, social proof, urgency). Each is labeled so you see the approach.

**How to use:**
```
Give me 10 headline ideas for a landing page selling CRM software to estate agents.
```

**Skill file:** `.claude/skills/headline-writer.md`

---

### 5. **Brand Voice** — Extract or apply a brand voice

**What it does:** Two modes —
- **(A) Extract** a brand voice from content examples and create a Brand Voice Card
- **(B) Rewrite** content in a supplied brand voice. Shows before/after.

**How to use:**
```
Extract the tone of voice from these three web pages.
```
or
```
Rewrite this in the Bloom Studio brand voice.
```

**Skill file:** `.claude/skills/brand-voice.md`

---

### 6. **Landing Page** — Write a complete landing page

**What it does:** Structures and writes a full landing page — hero, problem, solution, features/benefits, social proof, FAQ, pricing, and CTA — using a proven conversion sequence.

**How to use:**
```
Write a landing page for a website audit service targeting marketing managers.
```

**Skill file:** `.claude/skills/landing-page.md`

---

### 7. **Email Sequence** — Write multi-email campaigns

**What it does:** Writes email sequences — welcome, onboarding, sales/launch, or re-engagement. Each email includes subject line, preview text, body, and CTA.

**How to use:**
```
Write a 5-email welcome sequence for a B2B copywriting course.
```

**Skill file:** `.claude/skills/email-sequence.md`

---

### 8. **Ad Copy** — Write paid ads

**What it does:** Writes ad copy for Google Search, Meta (Facebook/Instagram), or LinkedIn. Respects platform character limits and formats. Produces multiple headline and description variations.

**How to use:**
```
Write Google search ads for this landing page. Primary keyword: 'SEO copywriter UK'.
```

**Skill file:** `.claude/skills/ad-copy.md`

---

## How to see how a skill works

Type in the chat:
```
Read the seo-web-copy.md skill and explain how it structures a web page.
```

Claude will read the skill and explain it in plain language.

---

## How to edit an existing skill

1. In Claude Code, type:
```
/anthropic-skills:skill-creator
```

2. Claude will ask you:
   - Create a new skill or modify an existing one?
   - Which one?
   - What do you want to change?

3. Follow the instructions and Claude will update the skill for you.

---

## How to create a new skill

**Option 1 — Use the Skill Creator (recommended)**

1. Type `/anthropic-skills:skill-creator`
2. Tell it you want to create a new skill
3. Describe what it should do. For example:
```
I want a skill that writes product descriptions for a fashion store. 
It should include: product name, short description, features, benefits, price.
```

**Option 2 — Ask Claude directly**

```
Create a new skill for writing About pages for law firms. 
It should cover: firm mission, practice areas, client benefits, and a CTA.
Save it to .claude/skills/legal-about-page.md
```

---

## Tips

- **Skills work automatically** — you don't need to call them by name.
- **More context = better results** — include the target audience, tone, format, etc.
- **You can create as many skills as you want** — if you do the same thing often, create a skill to automate it.
- **Test a skill before using it in production** — ask it to generate an example, then check it.
