# Skill: SEO Audit

Use this skill when given a URL to perform a comprehensive SEO and content audit — combining technical SEO, GEO/AEO readiness, and a full copy quality review.

## Trigger phrases
- "audit this URL", "audit this page", "audit this site"
- "SEO audit", "full audit", "technical audit"
- "what's wrong with this page", "check this URL for SEO"
- "run an audit on", "analyse this page", "review this URL"
- "auditer cette URL", "audit SEO", "audit technique"
- "analyser cette page", "vérifier cette URL", "faire un audit de"

## What this skill does

Given a URL, this skill:
1. Fetches the page and inspects all available technical and on-page signals
2. Runs a full technical SEO audit against current best practices
3. Audits GEO/AEO readiness (AI citation signals)
4. Applies the **Copy Audit** skill to the page content
5. Delivers a single consolidated report with prioritised actions

---

## Step 1: Fetch the page

Use WebFetch (or equivalent) to retrieve the full HTML of the URL. Extract:
- Page title and meta description
- All heading tags (H1–H6) and their text
- Opening paragraph (first ~150 words of body copy)
- All body copy text
- Any visible structured data / JSON-LD blocks
- Internal and external links
- Image alt attributes
- Canonical tag value
- Robots meta tag
- Open Graph / Twitter card tags

If the page cannot be fetched, report the error and stop.

---

## Step 2: Technical SEO audit

Check each item below. Mark as **Pass**, **Flag**, or **Fail**.

### 2a. Crawlability & indexability
- [ ] Page returns HTTP 200 (not 3xx redirect chain, 4xx, or 5xx)
- [ ] Robots meta tag does not block indexing (`noindex` = Fail)
- [ ] Canonical tag present and self-referencing (or correctly pointing elsewhere)
- [ ] Page is not blocked by known redirect issues (multiple hops = Flag)

### 2b. Title tag
- [ ] Present and unique
- [ ] 40–60 characters (under 40 = Flag, over 60 = Flag)
- [ ] Primary keyword appears near the start
- [ ] Not duplicated as H1 verbatim

### 2c. Meta description
- [ ] Present
- [ ] 120–155 characters (missing = Fail, over 155 = Flag)
- [ ] Includes primary keyword naturally
- [ ] Has a clear value proposition or call to action

### 2d. Heading structure
- [ ] Single H1 present (zero or multiple = Fail)
- [ ] H1 contains or is closely related to the primary keyword
- [ ] Logical H1 → H2 → H3 hierarchy (no skipped levels)
- [ ] Headings are descriptive, not generic ("Introduction", "Section 1" = Flag)

### 2e. URL
- [ ] URL is clean and readable (no session IDs, excessive parameters)
- [ ] Contains keyword or topic signal
- [ ] Under 75 characters where possible

### 2f. Images
- [ ] All images have non-empty alt attributes
- [ ] Alt text is descriptive (not "image1.jpg", not keyword-stuffed)

### 2g. Internal linking
- [ ] At least 2–3 internal links to relevant related pages
- [ ] Links use descriptive anchor text (not "click here" or "read more")

### 2h. Mobile & performance signals
- [ ] Page content appears responsive (check viewport meta tag: `<meta name="viewport"...>`)
- [ ] No obvious render-blocking or heavy asset indicators in the HTML

### 2i. HTTPS
- [ ] URL begins with `https://` (http:// = Fail)

### 2j. Structured data (Schema.org)
- [ ] JSON-LD or microdata present (absence is a Flag for most pages)
- [ ] Schema type is appropriate for the page (Article, LocalBusiness, FAQPage, Product, etc.)
- [ ] FAQ schema present if the page has FAQ content
- [ ] Author or organisation entity named in schema

---

## Step 3: GEO / AEO audit (AI citation readiness)

Apply the LLM Optimisation checklist:

- [ ] Page opens with a clear, direct statement of what it is and who it's for
- [ ] Primary question answered in the first 100 words
- [ ] Definition block present ("X is Y that does Z for [audience]")
- [ ] FAQ section written the way someone would ask an AI tool
- [ ] Each FAQ answer is self-contained (no "as mentioned above")
- [ ] Business/person/brand named consistently throughout
- [ ] Specific claims, numbers, or named examples present
- [ ] Headings reflect real questions, not just keyword phrases
- [ ] Topic covered completely (what it is, who it's for, how it works, why it matters)
- [ ] Any snippet from this page would make sense out of context

---

## Step 4: Copy audit

Apply the **Copy Audit** skill to the extracted body copy, assessing all seven dimensions:

1. Clarity
2. Structure
3. Tone & voice
4. SEO performance
5. LLM readiness
6. Conversion
7. Accuracy & consistency

---

## Output format

```
SEO AUDIT: [page title or URL]
Audited: [date]
URL: [full URL]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
OVERALL SCORE: [Strong / Good / Needs Work / Significant Issues]
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

── SECTION 1: TECHNICAL SEO ────────────────────────────

Crawlability & indexability — [Pass / Flag / Fail]
  [Observation]

Title tag — [Pass / Flag / Fail]
  Current: "[title tag text]" ([X]/60 chars)
  [Observation]

Meta description — [Pass / Flag / Fail]
  Current: "[meta description text]" ([X]/155 chars)
  [Observation]

Heading structure — [Pass / Flag / Fail]
  H1: "[h1 text]"
  [Observation]

URL — [Pass / Flag / Fail]
  [Observation]

Images — [Pass / Flag / Fail]
  [Observation]

Internal linking — [Pass / Flag / Fail]
  [Observation]

Mobile & performance — [Pass / Flag / Fail]
  [Observation]

HTTPS — [Pass / Flag / Fail]
  [Observation]

Structured data — [Pass / Flag / Fail]
  [Schema types found or missing]

── SECTION 2: GEO / AEO READINESS ──────────────────────

GEO SCORE: [Strong / Good / Needs Work / Not Optimised]

  [✓ / ✗] Answer-first opening
  [✓ / ✗] Definition block
  [✓ / ✗] FAQ section (AI-phrased questions)
  [✓ / ✗] Self-contained FAQ answers
  [✓ / ✗] Entity clarity (named consistently)
  [✓ / ✗] Specific claims or data points
  [✓ / ✗] Complete topic coverage

  Key gaps: [list the most impactful missing items]

── SECTION 3: COPY AUDIT ────────────────────────────────

[Full Copy Audit output per the copy-audit skill format]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
TOP 5 PRIORITIES (across all sections)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

1. [Most impactful fix — specific and actionable]
2. [Second priority]
3. [Third priority]
4. [Fourth priority]
5. [Fifth priority]

QUICK WINS (can implement in under 30 minutes):
- [Specific small change]
- [Specific small change]
- [Specific small change]
```

After the audit, offer: "Want me to rewrite any flagged sections, draft updated meta tags, or add missing structured data?"

---

## Inputs to ask for (if not provided)
- The URL to audit (required)
- Primary target keyword (if known — helps assess SEO targeting)
- Business name and what they do (helps assess entity clarity)
- Page type (homepage, service page, landing page, blog post — helps calibrate expectations)
- Conversion goal (what action should the page drive?)
