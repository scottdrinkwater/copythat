# Assistant de rédaction IA / AI Writing Assistant

---

## 🇫🇷 En français

Votre espace de travail Claude Code pour la rédaction web, le SEO et l'optimisation LLM.

### Installation

Clonez le dépôt et ouvrez-le dans Claude Code :

```bash
git clone git@github.com:scottdrinkwater/copythat.git
cd copythat
```

Ouvrez ensuite ce dossier dans [Claude Code](https://claude.com/claude-code). Tous les skills sont prêts à l'emploi — aucune configuration supplémentaire nécessaire.

### Ce que Claude peut faire

- Rédiger des pages de service, accueil, à propos, pages locales
- Optimiser les textes pour le SEO — mots-clés, balises titre, méta descriptions, FAQ
- Optimiser les pages pour être citées par les IA (ChatGPT, Perplexity, Google AI Overviews)
- Auditer les textes existants : clarté, SEO, lisibilité IA, conversion
- Rédiger des landing pages, séquences d'emails et publicités
- Extraire ou appliquer la voix de marque d'un client
- Lire des PDF, Word, tableaux Excel et présentations PowerPoint

Voir [docs/agents.md](docs/agents.md) pour la liste complète des compétences.

### Comment parler à Claude

Décrivez simplement ce que vous voulez. Plus vous donnez de contexte, meilleur est le résultat.

**Bons exemples :**
- « Rédige une page de service pour une agence de copywriting B2B ciblant "copywriter Paris". Ton : direct et professionnel. »
- « Lis brief.pdf et propose une structure de page avec H1, H2 et messages clés. »
- « Audite ce texte de page d'accueil pour l'optimisation IA. Donne-moi les 3 points prioritaires. »
- « Réécris ce premier paragraphe pour qu'il réponde directement à la requête de recherche. »

**Moins utile :**
- « Écris quelque chose de bien » — trop vague
- « Corrige ça » — collez le texte et précisez ce qui ne va pas

### Gérer les clients

Chaque client a un dossier dans `clients/` avec deux fichiers :

- `brief.md` — présentation de l'entreprise, audience, objectifs, mots-clés cibles
- `brand-voice.md` — règles de ton, préférences de style, mots à éviter

Pour ajouter un client : copiez un dossier existant, renommez-le et remplissez les fichiers. Mentionnez le client par son nom et Claude lira ses fichiers automatiquement.

**Exemple :** « Rédige une page d'accueil pour Apex Group. Lis d'abord leur brief et leur voix de marque. »

Les brouillons peuvent aussi être enregistrés dans le dossier client — ex. `clients/apex-group/accueil-v1.md`.

### Conseils

- Collez directement votre texte dans le chat — Claude travaille avec ce que vous lui donnez
- Indiquez le mot-clé cible, l'audience et le ton dès le départ
- Si le résultat ne convient pas : « plus court », « plus direct », « essaie un autre angle »
- Utilisez « Souviens-toi que [client] préfère... » pour sauvegarder des préférences

---

## 🇬🇧 In English

Your Claude Code workspace for website copywriting, SEO, and LLM optimisation.

### Installation

Clone the repository and open it in Claude Code:

```bash
git clone git@github.com:scottdrinkwater/copythat.git
cd copythat
```

Then open this folder in [Claude Code](https://claude.com/claude-code). All skills are ready to use immediately — no additional setup needed.

### What Claude can help with

- Write service pages, homepages, about pages, location pages
- Write and optimise copy for SEO — keywords, title tags, meta descriptions, FAQs
- Optimise pages to be cited by AI tools (ChatGPT, Perplexity, Google AI Overviews)
- Audit existing copy for clarity, SEO, LLM readiness, and conversion
- Write landing pages, email sequences, and ad copy
- Extract or apply a client's brand voice
- Read PDFs, Word docs, spreadsheets, and presentations

See [docs/agents.md](docs/agents.md) for the full list of skills and how to trigger them.

### How to talk to Claude

Just describe what you want. The more context you give, the better the output.

**Good prompts:**
- "Write a service page for a B2B copywriting agency targeting 'website copywriter for tech companies'. Tone: confident and direct."
- "Read brief.pdf and suggest a page structure with H1, H2s, and key messages."
- "Audit this homepage copy for LLM readiness. Tell me the top 3 things to fix."
- "Rewrite this opening paragraph so it answers the search query directly."

**Less useful:**
- "Write something good" — too vague
- "Fix this" — paste the copy and say what's wrong

### Managing clients

Each client has a folder in `clients/` with two files:

- `brief.md` — business overview, audience, goals, target keywords
- `brand-voice.md` — tone rules, style preferences, words to avoid

To add a new client, copy an existing folder, rename it, and fill in the files. Mention the client by name and Claude will read their files automatically.

**Example:** "Write a homepage for Apex Group. Read their brief and brand voice first."

Copy drafts can live in the client folder too — e.g. `clients/apex-group/homepage-v1.md`.

### Tips

- Paste copy directly into the chat — Claude will work with whatever you give it
- Tell Claude the target keyword, the audience, and the tone upfront
- If you don't like the output: "make it shorter", "more direct", "try a different angle"
- Use "Remember that [client] prefers..." to save preferences for future sessions
