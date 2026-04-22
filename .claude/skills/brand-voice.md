# Skill: Brand Voice Extractor & Applier

Use this skill when the user wants to define, document, or apply a brand's tone of voice.

## Trigger phrases
- "brand voice", "tone of voice", "TOV"
- "sound more like", "write in the style of"
- "match this brand", "apply our tone"
- "extract the tone from", "analyse this copy"
- "voix de marque", "ton de marque", "tonalité"
- "écrire dans le style de", "appliquer notre ton"
- "extraire le ton", "analyser ce texte", "guide de style"
- "comment on écrit", "notre façon d'écrire"

## Two modes

### Mode A: Extract voice from examples
When the user provides existing copy (from a website, doc, or paste), analyse it and produce a **Brand Voice Card**.

**Brand Voice Card format:**

```
BRAND VOICE: [Brand name]

IN THREE WORDS: [adjective] · [adjective] · [adjective]

WE SOUND LIKE: [one vivid analogy — e.g. "a smart friend at the pub, not a consultant at a boardroom"]

WHAT WE DO:
- [specific sentence-level behaviour — e.g. "Use short sentences. One idea per line."]
- [punctuation/formatting rule]
- [vocabulary choice — e.g. "Say 'you' not 'our customers'"]
- [structural pattern — e.g. "Lead with the outcome, not the process"]

WHAT WE NEVER DO:
- [specific thing to avoid — e.g. "Never use exclamation marks"]
- [jargon or phrases to ban]
- [tone to avoid — e.g. "Never sound apologetic or hedge with 'perhaps'"]

SAMPLE SENTENCE IN VOICE:
[Write one example sentence that perfectly captures the voice]
```

### Mode B: Apply existing voice to new copy
When the user provides both a voice guide AND copy to rewrite, apply the voice rules faithfully. After rewriting:
- Show the before and after
- Note which voice rules you applied

## Output format
- For Mode A: Produce the Brand Voice Card in a code block so it's easy to copy
- For Mode B: Show original, then rewritten version, then a brief note on changes

## Inputs to ask for (if not provided)
- Sample copy to analyse (Mode A) — more examples = better analysis
- Or: the existing voice guide + copy to rewrite (Mode B)
- Brand name and industry (for context)
