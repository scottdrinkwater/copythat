# Assistant de rédaction IA

> 🇬🇧 [English version](README.en.md)

Votre espace de travail Claude Code pour la rédaction web, le SEO et l'optimisation LLM.

## Installation

**Option 1 — Téléchargement direct (recommandé)**

1. Téléchargez le fichier ZIP depuis la [dernière version](https://github.com/scottdrinkwater/copythat/releases/latest) (cliquez sur « Source code (zip) »)
2. Décompressez le dossier
3. Ouvrez [Claude Code](https://claude.com/claude-code), puis ouvrez ce dossier

Tous les skills sont prêts à l'emploi — aucune configuration supplémentaire nécessaire.

**Option 2 — Via Git (utilisateurs techniques)**

```bash
git clone git@github.com:scottdrinkwater/copythat.git
cd copythat
```

## Ce que Claude peut faire

- Rédiger des pages de service, accueil, à propos, pages locales
- Optimiser les textes pour le SEO — mots-clés, balises titre, méta descriptions, FAQ
- Optimiser les pages pour être citées par les IA (ChatGPT, Perplexity, Google AI Overviews)
- Auditer les textes existants : clarté, SEO, lisibilité IA, conversion
- Rédiger des landing pages, séquences d'emails et publicités
- Extraire ou appliquer la voix de marque d'un client
- Lire des PDF, Word, tableaux Excel et présentations PowerPoint

Voir [docs/agents.md](docs/agents.md) pour la liste complète des compétences.

## Comment parler à Claude

Décrivez simplement ce que vous voulez. Plus vous donnez de contexte, meilleur est le résultat.

**Bons exemples :**
- « Rédige une page de service pour une agence de copywriting B2B ciblant "copywriter Paris". Ton : direct et professionnel. »
- « Lis brief.pdf et propose une structure de page avec H1, H2 et messages clés. »
- « Audite ce texte de page d'accueil pour l'optimisation IA. Donne-moi les 3 points prioritaires. »
- « Réécris ce premier paragraphe pour qu'il réponde directement à la requête de recherche. »

**Moins utile :**
- « Écris quelque chose de bien » — trop vague
- « Corrige ça » — collez le texte et précisez ce qui ne va pas

## Gérer les clients

Chaque client a un dossier dans `clients/` avec deux fichiers :

- `brief.md` — présentation de l'entreprise, audience, objectifs, mots-clés cibles
- `brand-voice.md` — règles de ton, préférences de style, mots à éviter

Pour ajouter un client : copiez un dossier existant, renommez-le et remplissez les fichiers. Mentionnez le client par son nom et Claude lira ses fichiers automatiquement.

**Exemple :** « Rédige une page d'accueil pour Apex Group. Lis d'abord leur brief et leur voix de marque. »

Les brouillons peuvent aussi être enregistrés dans le dossier client — ex. `clients/apex-group/accueil-v1.md`.

## Conseils

- Collez directement votre texte dans le chat — Claude travaille avec ce que vous lui donnez
- Indiquez le mot-clé cible, l'audience et le ton dès le départ
- Si le résultat ne convient pas : « plus court », « plus direct », « essaie un autre angle »
- Utilisez « Souviens-toi que [client] préfère... » pour sauvegarder des préférences
