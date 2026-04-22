# Skill: Copy Audit

Use this skill when reviewing existing web copy for quality, clarity, SEO performance, or LLM readiness — before sending to a client or when asked to improve existing work.

## Trigger phrases
- "audit this copy", "review this page", "what's wrong with this"
- "improve this", "tighten this", "is this good enough"
- "check this for SEO", "check this for AI", "is this optimised"
- "give me feedback on", "critique this"
- "auditer ce texte", "analyser cette page", "qu'est-ce qui ne va pas"
- "améliorer ce texte", "vérifier ce texte", "est-ce suffisant"
- "vérifier le SEO", "vérifier pour l'IA", "est-ce optimisé"
- "donne-moi un retour sur", "critiquer ce texte", "passer en revue"

## Audit dimensions

Run through all relevant dimensions below. Skip any that don't apply to the brief.

---

### 1. CLARITY
Can a stranger understand what this page is about and who it's for in 5 seconds?
- Is the H1 immediately clear?
- Is the opening paragraph free of jargon?
- Does the copy assume too much prior knowledge?

**Flag:** Sentences over 25 words, unexplained acronyms, passive voice overuse.

---

### 2. STRUCTURE
Does the copy guide the reader forward logically?
- Is there a clear hierarchy (H1 → H2 → H3)?
- Do sections follow a logical order (problem → solution → proof → CTA)?
- Are paragraphs short and scannable?

**Flag:** Walls of text, missing subheadings, CTAs buried at the bottom only.

---

### 3. TONE & VOICE
Is the tone consistent and appropriate for the audience?
- Does it match the brand voice (if one was provided)?
- Is it too formal / too casual / inconsistent?
- Does it speak directly to the reader (uses "you")?

**Flag:** Sudden tone shifts, corporate-speak, passive or distancing language.

---

### 4. SEO PERFORMANCE
Is the copy optimised to rank?
- Is the primary keyword in the H1 and opening paragraph?
- Are secondary keywords used naturally in H2s and body?
- Is the meta description compelling and within 155 characters?
- Are there internal link opportunities?

**Flag:** Missing keyword in H1, keyword stuffing, no meta description, no FAQ section.

---

### 5. LLM READINESS (AEO / GEO)
Is this copy likely to be surfaced or cited by AI tools?
- Is the main question answered directly in the first 100 words?
- Are there definition blocks ("X is Y that does Z")?
- Are FAQ answers self-contained (work without context)?
- Is the entity (business/person) named clearly and consistently?

**Flag:** Vague opening, no FAQ, answers that rely on surrounding context, no specific claims or data.

---

### 6. CONVERSION
Does the copy move the reader toward the desired action?
- Is there a clear CTA?
- Is the benefit stated before the ask?
- Are objections addressed before the CTA?
- Is social proof present?

**Flag:** Weak or missing CTA, features listed without benefits, no trust signals.

---

### 7. ACCURACY & CONSISTENCY
Are claims credible and consistent throughout?
- Are there unsupported superlatives ("best", "leading", "world-class")?
- Are figures and facts referenced or attributed?
- Is terminology consistent (not switching between names for the same thing)?

**Flag:** Unverified claims, inconsistent naming, hollow adjectives.

---

## Output format

```
COPY AUDIT: [Page name or topic]
Audited: [date]

OVERALL SCORE: [Strong / Good / Needs Work / Significant Issues]

DIMENSION FINDINGS:

1. Clarity — [Pass / Flag / Fail]
   [Specific observation + example from the copy]

2. Structure — [Pass / Flag / Fail]
   [Specific observation]

3. Tone & Voice — [Pass / Flag / Fail]
   [Specific observation]

4. SEO — [Pass / Flag / Fail]
   [Specific observation]

5. LLM Readiness — [Pass / Flag / Fail]
   [Specific observation]

6. Conversion — [Pass / Flag / Fail]
   [Specific observation]

7. Accuracy — [Pass / Flag / Fail]
   [Specific observation]

TOP 3 PRIORITIES:
1. [Most important fix — specific and actionable]
2. [Second priority]
3. [Third priority]

QUICK WINS (can fix in under 5 mins):
- [Specific small change]
- [Specific small change]
```

After the audit, offer: "Want me to rewrite any of the flagged sections now?"

## Inputs to ask for (if not provided)
- The copy to audit (paste it in or provide a file)
- Page type (homepage, service page, landing page, etc.)
- Primary keyword (for SEO dimension)
- Brand voice guide (for tone dimension) — or skip that dimension
- Conversion goal (what action should the page drive?)
