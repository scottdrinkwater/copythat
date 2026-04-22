# Compétences & Agents

> 🇬🇧 [English version](agents.en.md)

Ces outils spécialisés sont intégrés à Claude Code. Chacun gère un type de travail de copywriting précis — décrivez ce que vous voulez et Claude utilisera automatiquement le bon outil.

## Compétences de rédaction

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

## Lire des fichiers

Déposez n'importe quel fichier client dans ce dossier et demandez à Claude de le lire.

- **PDF** — briefs, guides de marque, rapports de recherche, contrats. Ex : « Lis brief.pdf et extrais les messages clés et l'audience cible. »
- **Word (.docx)** — textes clients, retours, anciens brouillons. Ex : « Lis feedback.docx et dis-moi quels changements le client veut. »
- **Tableur (.xlsx)** — listes de mots-clés, matrices de contenu, trackers. Ex : « Lis keywords.xlsx et suggère lesquels cibler sur la page d'accueil. »
- **Présentation (.pptx)** — chartes graphiques, briefs créatifs, études concurrentielles. Ex : « Lis brand-guidelines.pptx et extrais les règles de ton. »

## Organisation & mémoire

- `/anthropic-skills:consolidate-memory` — sauvegarde tout ce que Claude a appris sur vos préférences et clients pour les sessions futures.
- `/anthropic-skills:schedule` — programme une tâche récurrente. Ex : « Chaque vendredi, rappelle-moi de mettre à jour mon suivi de projet. »

## Gérer les clients

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
