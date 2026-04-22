# Guide des Compétences

> 🇬🇧 [English version](SKILLS-GUIDE.en.md)

Ce guide explique les compétences de copywriting disponibles dans ce projet, comment les utiliser, et comment les modifier ou en créer de nouvelles.

### Qu'est-ce qu'une « skill » (compétence) ?

Une skill est un ensemble d'instructions spécialisées qui indique à Claude comment accomplir une tâche spécifique. Par exemple, la skill "SEO Web Copy" sait comment structurer une page Web pour le référencement.

Vous n'avez pas besoin de connaître les détails techniques — il suffit de demander à Claude ce que vous voulez et il utilise automatiquement la bonne skill.

---

## Les compétences de copywriting

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

## Comment voir comment fonctionne une skill

Tapez dans le chat :
```
Lis la skill seo-web-copy.md et explique-moi comment elle structure une page Web.
```

Claude lira la skill et vous l'expliquera en langage simple.

---

## Comment éditer une skill existante

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

## Comment créer une nouvelle skill

**Option 1 — Utiliser le Skill Creator (recommandé)**

1. Tapez `/anthropic-skills:skill-creator`
2. Dites que vous voulez créer une nouvelle skill
3. Décrivez ce qu'elle doit faire. Par exemple :
```
Je veux une skill qui écrit des descriptions de produits pour un magasin de mode. 
Elle doit inclure : nom du produit, description courte, caractéristiques, avantages, prix.
```

**Option 2 — Demander à Claude directement**

```
Crée une nouvelle skill pour écrire des pages À propos pour les cabinets d'avocats. 
Elle doit couvrir : la mission du cabinet, les domaines de pratique, les avantages clients, et un appel à l'action.
Mets-la dans .claude/skills/legal-about-page.md
```

---

## Conseils

- **Les skills fonctionnent automatiquement** — vous n'avez pas besoin de les appeler par leur nom.
- **Plus vous donnez de contexte, mieux c'est** — incluez le public cible, le ton, le format, etc.
- **Vous pouvez créer autant de skills que vous le souhaitez** — si vous faites souvent la même chose, créez une skill pour l'automatiser.
- **Testez une skill avant de l'utiliser en production** — demandez-lui de générer un exemple, puis vérifiez-le.
