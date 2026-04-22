# Skills Guide / Guide des Compétences

---

## 🇫🇷 Guide pour les utilisateurs non-techniques

Ce guide explique les 8 compétences de copywriting disponibles dans ce projet, comment les utiliser, et comment les modifier ou en créer de nouvelles.

### Qu'est-ce qu'une « skill » (compétence) ?

Une skill est un ensemble d'instructions spécialisées qui indique à Claude comment accomplir une tâche spécifique. Par exemple, la skill "SEO Web Copy" sait comment structurer une page Web pour le référencement.

Vous n'avez pas besoin de connaître les détails techniques — il suffit de demander à Claude ce que vous voulez et il utilise automatiquement la bonne skill.

---

## 📚 Les 8 Compétences de Copywriting

### 1. **SEO Web Copy** — Écrire des pages qui se classent bien

**À quoi ça sert :** Écrit du contenu pour les pages de service, accueil, à propos, pages de localisation. Inclut les balises titre, les descriptions meta, et les sections FAQ optimisées pour le référencement.

**Comment l'utiliser :**
```
Écris une page de service pour une agence de copywriting ciblant « copywriter Paris ». 
Audience : agences numériques B2B.
```

**Fichier skill :** `.claude/skills/seo-web-copy.md`

---

### 2. **LLM Optimisation (AEO/GEO)** — Optimiser pour ChatGPT, Perplexity, Google AI

**À quoi ça sert :** Réécrit du contenu pour qu'il soit cité et surfacé par les outils IA (ChatGPT, Perplexity, Google AI Overviews). Utilise des techniques comme les réponses directes, les blocs de définition, et la clarté des entités.

**Comment l'utiliser :**
```
Optimise cette page de service pour qu'elle soit plus susceptible d'être recommandée par les outils IA.
```

**Fichier skill :** `.claude/skills/llm-optimisation.md`

---

### 3. **Copy Audit** — Audit complet du contenu existant

**À quoi ça sert :** Analyse du contenu sur 7 dimensions : clarté, structure, ton, SEO, compatibilité IA, conversion, et exactitude. Produit un rapport noté avec les priorités principales.

**Comment l'utiliser :**
```
Fais un audit de cette page d'accueil. Dis-moi quoi corriger pour le SEO et l'optimisation IA.
```

**Fichier skill :** `.claude/skills/copy-audit.md`

---

### 4. **Headline Writer** — Générer 10 options de titres

**À quoi ça sert :** Crée 10 titres différents en utilisant des cadres éprouvés (PAS, AIDA, curiosité, bénéfices, spécificité, contrarian, preuve sociale, urgence). Chacun est étiqueté pour que tu vois l'approche.

**Comment l'utiliser :**
```
Donne-moi 10 idées de titres pour une page de destination vendant un logiciel CRM à des agents immobiliers.
```

**Fichier skill :** `.claude/skills/headline-writer.md`

---

### 5. **Brand Voice** — Extraire ou appliquer une voix de marque

**À quoi ça sert :** Deux modes —
- **(A) Extraire** une voix de marque à partir d'exemples de contenu et créer une carte de ton de voix
- **(B) Réécrire** du contenu dans une voix de marque fournie. Affiche le avant/après.

**Comment l'utiliser :**
```
Extrais le ton de voix de ces trois pages Web.
```
ou
```
Réécris ça dans la voix de marque de l'agence Bloom Studio.
```

**Fichier skill :** `.claude/skills/brand-voice.md`

---

### 6. **Landing Page** — Écrire une page de destination complète

**À quoi ça sert :** Structure et écrit une page de destination complète — héros, problème, solution, caractéristiques/avantages, preuve sociale, FAQ, prix, et appel à l'action — en utilisant une séquence de conversion éprouvée.

**Comment l'utiliser :**
```
Écris une page de destination pour un service d'audit de site Web ciblant les responsables marketing.
```

**Fichier skill :** `.claude/skills/landing-page.md`

---

### 7. **Email Sequence** — Écrire une séquence multi-email

**À quoi ça sert :** Écrit des séquences d'emails — bienvenue, onboarding, vente/lancement, ou ré-engagement. Chaque email inclut la ligne d'objet, le texte d'aperçu, le corps et l'appel à l'action.

**Comment l'utiliser :**
```
Écris une séquence de 5 emails de bienvenue pour un cours de copywriting B2B.
```

**Fichier skill :** `.claude/skills/email-sequence.md`

---

### 8. **Ad Copy** — Écrire des annonces payantes

**À quoi ça sert :** Écrit du contenu d'annonce pour Google Search, Meta (Facebook/Instagram), ou LinkedIn. Respecte les limites de caractères de chaque plateforme et les formats. Produit plusieurs variations de titres et descriptions.

**Comment l'utiliser :**
```
Écris des annonces Google Search pour cette page de destination. Mot-clé principal : « copywriter SEO Paris ».
```

**Fichier skill :** `.claude/skills/ad-copy.md`

---

## 🔍 Comment Voir Comment Fonctionne Une Skill

### **Méthode 1 : Demande à Claude de l'expliquer (plus facile)**

Tapez dans le chat :
```
Lis la skill seo-web-copy.md et explique-moi comment elle structure une page Web.
```

Claude lira la skill et vous l'expliquera en langage simple.

---

## ✏️ Comment Éditer une Skill Existante

### **Méthode 1 : Utiliser l'outil Skill Creator (recommandé)**

C'est la méthode la plus sûre pour les utilisateurs non-techniques.

1. Dans Claude Code, tapez :
```
/anthropic-skills:skill-creator
```

2. Claude vous posera des questions :
   - Créer une nouvelle skill ou modifier une existante ?
   - Laquelle ?
   - Qu'est-ce que tu veux changer ?

3. Suivez les instructions et Claude mettra à jour la skill pour vous.

---

## ➕ Comment Créer Une Nouvelle Skill

### **Méthode 1 : Utiliser l'outil Skill Creator (recommandé)**

1. Dans Claude Code, tapez :
```
/anthropic-skills:skill-creator
```

2. Dites que vous voulez créer une nouvelle skill

3. Décrivez ce que la nouvelle skill doit faire. Par exemple :
```
Je veux une skill qui écrit des descriptions de produits pour un magasin de mode. 
Elle doit inclure : nom du produit, description courte, caractéristiques, avantages, prix.
```

4. Claude créera la skill et la sauvegardiera pour vous.

### **Méthode 2 : Demander à Claude de la créer**

Vous pouvez aussi demander à Claude de créer une nouvelle skill sans utiliser l'outil :

```
Crée une nouvelle skill pour écrire des pages À propos pour les cabinets d'avocats. 
Elle doit couvrir : la mission du cabinet, les domaines de pratique, les avantages clients, et un appel à l'action.
Mets-la dans .claude/skills/legal-about-page.md
```

Claude créera le fichier pour vous.

---

## 📝 Conseils pour les Skills

- **Les skills fonctionnent automatiquement** — vous n'avez pas besoin de les appeler par leur nom. Juste demandez à Claude ce que vous voulez.
- **Plus vous donnez de contexte, mieux c'est** — incluez le public cible, le ton, le format, etc.
- **Vous pouvez créer autant de skills que vous le souhaitez** — si vous faites souvent la même chose, créez une skill pour l'automatiser.
- **Testez une skill avant de l'utiliser en production** — demandez-lui de générer un exemple, puis vérifiez-le.

---

---

## 🇬🇧 Guide for Non-Technical Users

This guide explains the 8 copywriting skills available in this project, how to use them, and how to modify or create new ones.

### What is a "Skill"?

A skill is a set of specialized instructions that tells Claude how to accomplish a specific task. For example, the "SEO Web Copy" skill knows how to structure a web page for search rankings.

You don't need to know technical details — just ask Claude what you want and it automatically uses the right skill.

---

## 📚 The 8 Copywriting Skills

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

## 🔍 How to See How a Skill Works

### **Method 1: Ask Claude to explain it (easiest)**

Type in the chat:
```
Read the seo-web-copy.md skill and explain how it structures a web page.
```

Claude will read the skill and explain it in plain language.

---

## ✏️ How to Edit an Existing Skill

### **Method 1: Use the Skill Creator tool (recommended)**

This is the safest method for non-technical users.

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

## ➕ How to Create a New Skill

### **Method 1: Use the Skill Creator tool (recommended)**

1. In Claude Code, type:
```
/anthropic-skills:skill-creator
```

2. Tell it you want to create a new skill

3. Describe what the new skill should do. For example:
```
I want a skill that writes product descriptions for a fashion store. 
It should include: product name, short description, features, benefits, price.
```

4. Claude will create the skill and save it for you.

### **Method 2: Ask Claude to create it**

You can also ask Claude to create a new skill directly:

```
Create a new skill for writing About pages for law firms. 
It should cover: firm mission, practice areas, client benefits, and a CTA.
Save it to .claude/skills/legal-about-page.md
```

Claude will create the file for you.

---

## 📝 Tips for Skills

- **Skills work automatically** — you don't need to call them by name. Just ask Claude what you want.
- **More context = better results** — include the target audience, tone, format, etc.
- **You can create as many skills as you want** — if you do the same thing often, create a skill to automate it.
- **Test a skill before using it in production** — ask it to generate an example, then check it.

