# Compétences & Agents / Skills & Agents

---

## 🇫🇷 En français

Ces outils spécialisés sont intégrés à Claude Code. Chacun gère un type de travail de copywriting précis — décrivez ce que vous voulez et Claude utilisera automatiquement le bon outil.

### Compétences de rédaction

Ces compétences se déclenchent automatiquement quand vous demandez à Claude d'écrire ou d'optimiser quelque chose. Inutile de les appeler par leur nom.

**Audit SEO**
Ce que ça fait : audit complet d'une URL — SEO technique, préparation GEO/AEO (citation IA) et audit du texte. Inspecte balise titre, méta description, structure des titres, données structurées, liens internes et signaux de performance. Produit un rapport noté avec un top 5 des priorités et des actions rapides.
Comment l'utiliser : « Audite cette URL pour le SEO et l'optimisation IA : [url] »

**Texte web SEO**
Ce que ça fait : rédige du contenu web optimisé pour le référencement — pages de service, pages locales, accueil, à propos. Inclut balise titre, méta description, H1, corps de texte et FAQ. Suit la hiérarchie des mots-clés et les principes E-E-A-T.
Comment l'utiliser : « Rédige une page de service ciblant "copywriter freelance Manchester". Audience : entreprises tech B2B. »

**Optimisation LLM (AEO / GEO)**
Ce que ça fait : rédige ou réécrit des textes pour qu'ils soient cités par les outils IA — ChatGPT, Perplexity, Google AI Overviews, Claude. Utilise l'écriture answer-first, les blocs de définition, les FAQ autonomes et la clarté des entités.
Comment l'utiliser : « Optimise cette page de service pour qu'elle soit recommandée par les outils IA. »

**Audit de texte**
Ce que ça fait : évalue les textes existants selon 7 dimensions : clarté, structure, ton, SEO, lisibilité IA, conversion et exactitude. Produit un rapport noté avec priorités et améliorations rapides.
Comment l'utiliser : « Audite ce texte de page d'accueil. Dis-moi quoi corriger pour le SEO et l'optimisation IA. »

**Rédacteur de titres**
Ce que ça fait : génère 10 options de titres selon des frameworks éprouvés — PAS, AIDA, curiosity gap, bénéfice-led, précision, angle contrarian, preuve sociale, urgence. Chaque titre est étiqueté avec son approche.
Comment l'utiliser : « Donne-moi 10 idées de titres pour une landing page vendant un CRM à des agences immobilières. »

**Voix de marque**
Ce que ça fait : deux modes — (A) extrait une voix de marque à partir d'exemples de textes et produit une Brand Voice Card, ou (B) réécrit un texte dans une voix de marque fournie. Montre avant/après en cas de réécriture.
Comment l'utiliser : « Extrais le ton de ces trois pages web. » ou « Réécris ce texte dans la voix de marque de Bloom Studio. »

**Landing page**
Ce que ça fait : structure et rédige une landing page complète — hero, problème, solution, fonctionnalités/bénéfices, preuve sociale, FAQ, tarifs et CTA — selon une séquence de conversion éprouvée.
Comment l'utiliser : « Rédige une landing page pour un service d'audit de site web ciblant des directeurs marketing. »

**Séquence d'emails**
Ce que ça fait : rédige des séquences multi-emails — bienvenue, onboarding, vente/lancement ou réengagement. Chaque email inclut objet, texte de prévisualisation, corps et CTA.
Comment l'utiliser : « Rédige une séquence de bienvenue en 5 emails pour une formation en copywriting B2B. »

**Publicités**
Ce que ça fait : rédige des publicités payantes pour Google Search, Meta (Facebook/Instagram) ou LinkedIn. Respecte les limites de caractères et les formats de chaque plateforme. Produit plusieurs variantes de titres et descriptions.
Comment l'utiliser : « Rédige des annonces Google Search pour cette landing page. Mot-clé principal : "copywriter SEO France". »

### Lire des fichiers

Déposez n'importe quel fichier client dans ce dossier et demandez à Claude de le lire.

- **PDF** — briefs, guides de marque, rapports de recherche, contrats. Ex : « Lis brief.pdf et extrais les messages clés et l'audience cible. »
- **Word (.docx)** — textes clients, retours, anciens brouillons. Ex : « Lis feedback.docx et dis-moi quels changements le client veut. »
- **Tableur (.xlsx)** — listes de mots-clés, matrices de contenu, trackers. Ex : « Lis keywords.xlsx et suggère lesquels cibler sur la page d'accueil. »
- **Présentation (.pptx)** — chartes graphiques, briefs créatifs, études concurrentielles. Ex : « Lis brand-guidelines.pptx et extrais les règles de ton. »

### Organisation & mémoire

- `/anthropic-skills:consolidate-memory` — sauvegarde tout ce que Claude a appris sur vos préférences et clients pour les sessions futures.
- `/anthropic-skills:schedule` — programme une tâche récurrente. Ex : « Chaque vendredi, rappelle-moi de mettre à jour mon suivi de projet. »

### Gérer les clients

Chaque client a un dossier dans `clients/` avec deux fichiers :

- `brief.md` — présentation de l'entreprise, audience, objectifs, mots-clés cibles
- `brand-voice.md` — règles de ton, préférences de style, mots à éviter

**Ajouter un client :** copiez un dossier existant (ex. `clients/apex-group/`), renommez-le et remplissez les deux fichiers.

**Écrire pour un client :** mentionnez-le par son nom et Claude lira ses fichiers automatiquement.
> « Rédige une page de service pour Bloom Studio. Lis d'abord leur brief et leur voix de marque. »

**Sauvegarder des brouillons :** ajoutez-les directement dans le dossier client.
> ex. `clients/bloom-studio/accueil-v1.md`, `clients/apex-group/services.md`

**Mettre à jour la mémoire de Claude en cours de session :** dites-le simplement.
> « Souviens-toi qu'Apex Group n'utilise jamais la voix passive. »

---

## 🇬🇧 In English

These are specialist tools built into Claude Code. Each one handles a specific copywriting job — just describe what you want and Claude will use the right one automatically.

### Writing Skills

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

### Reading Files

Drop any client file into this folder and ask Claude to read it.

- **PDF** — briefs, brand guides, research reports, contracts. e.g. "Read brief.pdf and pull out the key messages and target audience."
- **Word (.docx)** — client copy, feedback docs, previous drafts. e.g. "Read feedback.docx and tell me what changes the client wants."
- **Spreadsheet (.xlsx)** — keyword lists, content matrices, copy trackers. e.g. "Read keywords.xlsx and suggest which ones to target on the homepage."
- **Presentation (.pptx)** — brand decks, creative briefs, competitor research. e.g. "Read brand-guidelines.pptx and extract the tone of voice rules."

### Organisation & Memory

- `/anthropic-skills:consolidate-memory` — saves everything Claude has learned about your preferences and clients for future sessions.
- `/anthropic-skills:schedule` — set up a recurring task. e.g. "Every Friday, remind me to update my project tracker."

### Managing Clients

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
