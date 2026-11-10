# Agent Extension

Catalogue des skills, serveurs MCP et outils que l’on peut ajouter à un environnement d’agents selon les besoins d’un projet.

**Dernière revue documentaire** · 10 novembre 2026. Les dépôts et leurs README ont été consultés. Les prérequis et compatibilités indiqués viennent des mainteneurs. La colonne « Vérifié le » date cette lecture. Les essais locaux sont à consigner séparément.

- **Skill** · instructions et ressources de travail, généralement regroupées autour d’un fichier `SKILL.md`. Un pack en rassemble plusieurs. [Spécification Agent Skills](https://agentskills.io/)
- **MCP** · serveur qui expose des outils ou des ressources à un agent compatible. [Documentation MCP](https://modelcontextprotocol.io/)
- **Outil** · application, CLI, bibliothèque ou collection de code qu’un agent peut utiliser dans un workflow.

## Sources de veille

- **Dumble, 9 novembre 2026** · 20 projets autour de la vidéo, du design, de la 3D, de l’animation et des jeux. [Post sur X](https://x.com/Y0urDumble/status/2119793194435027220) · [Texte via FxTwitter](https://api.fxtwitter.com/Y0urDumble/status/2119793194435027220)
- **@abir35627, 10 octobre 2026** · 10 outils pour l’IA locale, les médias, le design et l’autohébergement. [Post sur X](https://x.com/abir35627/status/2108713572566180087) · [Texte via FxTwitter](https://api.fxtwitter.com/abir35627/status/2108713572566180087)
- **Dumble** · Sélections sur les Shorts, la capture de mouvement, le storyboard et les effets. [Pipeline Shorts](https://teapawt.org/Y0urDumble/status/2114798387249717600) · [Studio 2.5D](https://teapawt.org/Y0urDumble/status/2117030430507401326) · [Skills vidéo et VFX](https://xitter.cf/Y0urDumble/status/2119456820758524021)
- **ErikCH** · Sélection de serveurs MCP pour le navigateur, le code et les données. [Publication sur DEV](https://dev.to/erikch/10-mcp-servers-worth-adding-to-your-ai-coding-workflow-in-2026-1j1m)
- **r/claudeskills** · Discussion sur les packs de skills et les workflows de spécification. [Discussion sur Reddit](https://www.reddit.com/r/claudeskills/comments/1wwqyom/matt_pocock_superpowers_openspec_do_you_pick_one/)
- **Anmol Baranwal et Vultr** · Sélection d’outils pour construire des agents et guide de déploiement d’une base vectorielle. [Panorama sur DEV](https://dev.to/anmolbaranwal/open-source-toolkit-for-building-ai-agents-in-2026-55h1) · [Guide Qdrant](https://dev.to/vultr/deploying-qdrant-open-source-vector-database-for-ai-applications-on-ubuntu-2404-5235)
- **Microsoft, 4 novembre 2026** · Annonce des skills officiels pour développer avec Agent Framework en .NET et Python. [Annonce Microsoft](https://devblogs.microsoft.com/agent-framework/give-your-coding-agent-a-head-start-with-microsoft-agent-framework-skills-for-net-and-python/)
- **Notes de version MCP** · Évolutions des outils de développement, de test et de diagnostic. [FastMCP](https://github.com/PrefectHQ/fastmcp/blob/main/docs/updates.mdx) · [MCP Inspector](https://github.com/modelcontextprotocol/inspector/releases) · [Sentry Toolkit](https://github.com/getsentry/toolkit/releases)
- **SkillsLLM et iart-ai** · Sélection de quatre packs d’animation. Au 10 novembre 2026, GitHub affiche environ 1 300 étoiles pour la collection et 217 pour Motion Design Skills. Les trois autres packs ont surtout été retenus pour leurs usages distincts et leurs commits de septembre ou octobre 2026. [Fiche SkillsLLM](https://skillsllm.com/skill/motion-skills) · [Collection officielle](https://github.com/iart-ai/motion-skills)
- **AgenticSkills et SkillMD** · Repérage des skills de motion d’interface, de transitions React et d’animation 3D sur le Web. [Animate sur AgenticSkills](https://agenticskills.io/skills/animate) · [Animation & Graphics sur SkillMD](https://skillmd.com/category/animation-graphics)

Les publications servent à repérer des projets. Chaque fiche renvoie au dépôt du mainteneur et, le cas échéant, à la documentation de la fonctionnalité ou de la licence.

## Premiers essais à retenir

1. **HyperFrames** pour produire un Short vertical de 15 secondes à partir d’un extrait existant, avec sous-titres et carton de fin.
2. **Herk Edit Kit** pour comparer les coupes proposées sur une minute de dialogue à un montage manuel, en écoutant les raccords.
3. **Blender MCP** pour créer et rendre un plan 2.5D simple dans un fichier Blender de test.

Pour le design web, `impeccable` et `frontend-design` figurent déjà parmi les skills disponibles dans cet environnement. Comparer leur couverture avant d’ajouter Hallmark ou d’importer le pack Anthropic.

## Vidéo

| Nom | Type | Usage et prérequis | Vérifié le | Source |
| --- | --- | --- | --- | --- |
| HyperFrames | CLI + skills | Compose et rend des vidéos depuis HTML, CSS et JavaScript. Node.js 22+ et FFmpeg. | 2026-11-10 | [HeyGen](https://github.com/heygen-com/hyperframes) |
| OpenMontage | Suite d’outils + skills | Chaînes de production vidéo du script au rendu. Python, Node.js et FFmpeg. Les fournisseurs de génération dépendent du workflow choisi. | 2026-11-10 | [OpenMontage](https://github.com/OpenMontageInc/OpenMontage) |
| Video Shotcraft | Skill + modèles | Clips promotionnels éditables avec des recettes de plans, une synchronisation musicale et un rendu Remotion. Node.js et FFmpeg. | 2026-11-10 | [Video Shotcraft](https://github.com/Vincentwei1021/video-shotcraft) |
| Remotion Skills | Pack de skills | Composer des vidéos en React, avec des guides pour l’animation et le rendu. Le moteur Remotion a ses propres conditions d’usage. | 2026-11-10 | [Remotion Skills](https://github.com/remotion-dev/skills) · [Licence du moteur](https://www.remotion.dev/docs/license/pricing) |
| yt-dlp | CLI | Récupère des médias et des sous-titres depuis les sites pris en charge pour des sources qu’on est autorisé à traiter. FFmpeg sert notamment à fusionner les pistes audio et vidéo. | 2026-11-10 | [yt-dlp](https://github.com/yt-dlp/yt-dlp) |
| FFmpeg | CLI + bibliothèques | Découpe, assemble, convertit et encode des médias. `ffprobe` permet d’inspecter les pistes et métadonnées avant un export automatisé. | 2026-11-10 | [FFmpeg](https://github.com/FFmpeg/FFmpeg) |
| Drama Skills | Pack de skills + scripts | Adapte une histoire en scénario, prépare les fiches personnages et les storyboards, puis structure la revue des plans générés. Documentation principalement en chinois. Scripts Python 3.9+ et FFmpeg pour l’assemblage. | 2026-11-10 | [Drama Skills](https://github.com/zenstory-ai/drama-skills) |

## Design

| Nom | Type | Usage et prérequis | Vérifié le | Source |
| --- | --- | --- | --- | --- |
| Anthropic Skills | Pack de skills | Exemples pour le design d’interface, l’art algorithmique, les documents et les tests web. Sélectionner les dossiers utiles et vérifier leurs dépendances. | 2026-11-10 | [Anthropic](https://github.com/anthropics/skills) |
| Impeccable | Skill + plugin | Concevoir et auditer des interfaces, puis travailler la hiérarchie, la typographie et la finition. Déjà disponible dans cet environnement. | 2026-11-10 | [Impeccable](https://github.com/pbakaus/impeccable) |
| OpenDesign | Application + CLI + extensions | Espace de travail pour prototypes, sites, présentations et vidéos. Peut s’appuyer sur une CLI d’agent existante et expose aussi un MCP. | 2026-11-10 | [OpenDesign](https://github.com/nexu-io/open-design) |
| Hallmark | Skill | Direction visuelle pour sites et pages de présentation, avec des ressources photo et typographiques. Installation Codex documentée. | 2026-11-10 | [Hallmark](https://github.com/Nutlope/hallmark) |
| Penpot | Application web + MCP | Maquettes, prototypes et systèmes de design. Son MCP officiel permet de lire et de modifier la page ouverte, par exemple pour extraire les tokens d’un design system ou créer des variantes. | 2026-11-10 | [Penpot](https://github.com/penpot/penpot) · [Documentation MCP](https://help.penpot.app/mcp/) |

## 3D et éditeurs

| Nom | Type | Usage et prérequis | Vérifié le | Source |
| --- | --- | --- | --- | --- |
| Blender MCP | MCP + extension Blender | Piloter scènes, matériaux et objets depuis un agent. Blender et son extension doivent tourner. Le serveur expose aussi l’exécution de Python dans Blender. | 2026-11-10 | [MCP for Blender](https://github.com/ahujasid/mcp-for-blender) |
| Anatomy | Skill | Illustrations isométriques et vues éclatées interactives en SVG, avec des effets WebGL en option. | 2026-11-10 | [Anatomy](https://github.com/wheresryan22/anatomy) |
| Unity MCP | MCP + package Unity | Manipuler scènes et assets et modifier des scripts dans l’éditeur. Unity 2021.3 LTS à 6.x et Python 3.10+ via `uv` selon le README. | 2026-11-10 | [CoplayDev](https://github.com/CoplayDev/unity-mcp) |
| Blender Skills | Pack de skills | Guides de production, du blocage des volumes à l’export vers un moteur. Le workflow d’exécution documenté s’appuie sur Blender MCP. | 2026-11-10 | [Blender Skills](https://github.com/arjun988/blender-skills) |
| MPFB 2 | Extension Blender | Crée des personnages humains paramétrables pour préparer un rig ou peupler une scène. Blender 4.2+ selon le dépôt. | 2026-11-10 | [MakeHuman Community](https://github.com/makehumancommunity/mpfb2) |
| FreeMoCap | Application de capture | Enregistre des mouvements sans marqueurs avec une ou plusieurs caméras et exporte un squelette animé vers Blender. La reconstruction multi-vues demande une calibration. | 2026-11-10 | [FreeMoCap](https://github.com/freemocap/freemocap) · [Documentation](https://docs.freemocap.org/) |
| Three.js Skills | Pack de skills | Anime des modèles glTF, mélange des clips, pilote des squelettes et des morph targets, puis ajoute des effets de post-traitement. Le pack cible Three.js r186 et couvre WebGL et WebGPU avec TSL. | 2026-11-10 | [CloudAI-X](https://github.com/CloudAI-X/threejs-skills) |

## Animation et montage

| Nom | Type | Usage et prérequis | Vérifié le | Source |
| --- | --- | --- | --- | --- |
| GSAP Skills | Pack de skills | Guides officiels pour les courbes d’accélération, les timelines, le défilement et les plugins GSAP. | 2026-11-10 | [GSAP](https://github.com/greensock/gsap-skills) |
| Emil Kowalski Skills | Pack de skills | `animate` aide à décider quand et comment animer une interface, puis implémente la transition avec gestion des interruptions et du mouvement réduit. Le même dépôt propose `review-animations` et `animation-performance` pour la revue et le diagnostic. | 2026-11-10 | [Emil Kowalski](https://github.com/emilkowalski/skills) · [Skill Animate](https://github.com/emilkowalski/skills/tree/main/skills/animate) |
| Vercel React View Transitions | Skill | Guide officiel pour les transitions de navigation et les éléments partagés avec `<ViewTransition>`. React 19.3+ hors Next.js, avec une procédure dédiée à l’App Router. Licence de redistribution à confirmer. | 2026-11-10 | [Vercel](https://github.com/vercel-labs/agent-skills/tree/main/skills/react-view-transitions) · [Documentation React](https://react.dev/reference/react/ViewTransition) |
| Transitions.dev | Skill + bibliothèque CSS | Fournit des snippets de transition prêts à intégrer pour les menus, les onglets et les compteurs. Les exemples CSS sont indépendants du framework et incluent `prefers-reduced-motion`. La licence autorise l’usage commercial et encadre la redistribution de la bibliothèque. | 2026-11-10 | [Transitions.dev](https://github.com/Jakubantalik/transitions.dev) · [Licence](https://github.com/Jakubantalik/transitions.dev/blob/main/LICENSE) |
| Pretext Creative Demos | Skill | Skill optionnel de Hermes Agent pour faire circuler du texte autour de formes animées et manipuler des glyphes dans Canvas. Les démos utilisent la bibliothèque `@chenglou/pretext` et les exemples du skill la chargent depuis un CDN. | 2026-11-10 | [Skill dans Hermes Agent](https://github.com/NousResearch/hermes-agent/blob/main/optional-skills/creative/pretext/SKILL.md) · [Bibliothèque Pretext](https://github.com/chenglou/pretext) |
| Anything2Explainer | Skill + modèle Remotion | Produit un explicatif animé avec narration et sous-titres. Les workflows documentés couvrent l’anglais et le chinois. Le dépôt indique une licence PolyForm Noncommercial. | 2026-11-10 | [Anything2Explainer](https://github.com/Vincentwei1021/anything2explainer) |
| Oil Motion | Skill + scripts | Transforme des séquences d’images en animations web pilotées par le défilement, la souris ou le tactile. Traitement local via Python et FFmpeg. Génération IA via ZenMux par défaut. | 2026-11-10 | [Oil Motion](https://github.com/oil-oil/oil-motion) |
| Herk Edit Kit | Pack de skills + scripts | Prépare des coupes à partir d’une transcription et habille des Shorts avec HyperFrames. Node.js 22+, Git, FFmpeg et Chrome ou Chromium. | 2026-11-10 | [Herk Edit Kit](https://github.com/nateherkai/herk-edit-kit) |
| Shader Skills | Pack de skills + scripts | Écrit et vérifie des shaders procéduraux pour Shadertoy et WebGL2, par exemple pour l’eau, les nuages ou les effets de matière. | 2026-11-10 | [Shader Skills](https://github.com/gokayfem/shader-skills) |
| Motion Design Skills | Pack de skills | Guides de direction artistique, de rythme, de composition et d’animation de logos. Le skill After Effects couvre les expressions, les rigs et les réglages d’export. | 2026-11-10 | [iart-ai](https://github.com/iart-ai/motion-design-skills) |
| JavaScript Animation Skills | Pack de skills + scripts | Dessine chaque image en Canvas 2D sans fichiers d’illustration et peut synthétiser la bande-son en code. Le rendu MP4 s’appuie sur Node.js 18+, Playwright, Chrome ou Chromium et FFmpeg. | 2026-11-10 | [iart-ai](https://github.com/iart-ai/javascript-animation-skills) |
| Lower Thirds Skills | Skill + scripts | Crée des bandeaux animés transparents et vérifie le canal alpha après encodage. Exporte en WebM VP9 pour OBS ou en ProRes 4444 pour Resolve et Premiere. Requiert Node.js 18+, Playwright, Chrome ou Chromium et FFmpeg. | 2026-11-10 | [iart-ai](https://github.com/iart-ai/lower-thirds-skills) |
| B-roll Skills | Skill + scripts | Ajoute à une vidéo face caméra des graphiques animés calés sur les mots, avec export séparé sur fond transparent. Requiert Node.js 18+, Playwright, Chrome ou Chromium et FFmpeg. Transcription via whisper.cpp en local ou via l’API ElevenLabs. | 2026-11-10 | [iart-ai](https://github.com/iart-ai/b-roll-skills) |

## Jeux et assets

| Nom | Type | Usage et prérequis | Vérifié le | Source |
| --- | --- | --- | --- | --- |
| Universal Modder | Plugin + skills + MCP | Accompagne l’analyse et le modding de jeux PC. La méthode dépend du jeu et de son moteur. La génération d’assets peut passer par fal. | 2026-11-10 | [Universal Modder](https://github.com/rehan-remade/universal-modder) |
| Gamedev Agent Skills | Pack de skills | Sélection de workflows par moteur, dont Godot, Unity, Unreal, Phaser et Three.js. | 2026-11-10 | [Gamedev Agent Skills](https://github.com/gamedev-skills/awesome-gamedev-agent-skills) |
| PixelFX | Bibliothèque d’effets + skill | Exemples d’effets pixel art en code et skill pour en créer de nouveaux. Le dépôt documente le skill pour Claude Code. | 2026-11-10 | [PixelFX](https://github.com/patch-gg/pixelfx) |
| Sprite Gen | Skill + CLI Python | Produit des planches de sprites et des atlas d’animation. Python 3.11+ et fournisseur d’images selon le mode choisi. | 2026-11-10 | [Sprite Gen](https://github.com/aldegad/sprite-gen) |

## IA locale et génération d’images

| Nom | Type | Usage et prérequis | Vérifié le | Source |
| --- | --- | --- | --- | --- |
| Ollama | CLI + API | Exécute des modèles de langage en local avec une API utilisable par un agent. La mémoire nécessaire dépend du modèle et du contexte. Les fonctions cloud peuvent être désactivées. | 2026-11-10 | [Ollama](https://github.com/ollama/ollama) · [Mode local](https://docs.ollama.com/faq#how-do-i-disable-ollama-s-cloud-features) |
| Fooocus | Application | Génération d’images locale avec Stable Diffusion XL. Le projet est en maintenance limitée aux correctifs. Consulter la matrice GPU du dépôt avant installation. | 2026-11-10 | [Fooocus](https://github.com/lllyasviel/Fooocus) |
| ComfyUI | Application + API | Construit et exécute des graphes réutilisables de génération d’images ou de vidéo. Les modèles, les nœuds additionnels et la mémoire nécessaire varient selon le workflow. | 2026-11-10 | [ComfyUI](https://github.com/Comfy-Org/ComfyUI) |

## Voix et transcription

| Nom | Type | Usage et prérequis | Vérifié le | Source |
| --- | --- | --- | --- | --- |
| Whisper | CLI + bibliothèque | Transcription multilingue locale avec Python et FFmpeg. Pour obtenir des horodatages affinés au mot, voir WhisperX ci-dessous. | 2026-11-10 | [Whisper](https://github.com/openai/whisper) |
| WhisperX | CLI + bibliothèque | Transcription horodatée au mot pour sous-titres et coupes. La séparation des locuteurs est optionnelle et utilise un modèle soumis à des conditions d’accès. | 2026-11-10 | [WhisperX](https://github.com/m-bain/whisperX) |
| Kokoro | Modèle + bibliothèque Python | Synthèse vocale locale avec des voix prédéfinies. La v1.0 propose notamment la voix française `ff_siwis`, avec `espeak-ng` pour la prononciation. | 2026-11-10 | [Kokoro](https://github.com/hexgrad/kokoro) · [Voix disponibles](https://huggingface.co/hexgrad/Kokoro-82M/blob/main/VOICES.md) |
| ElevenLabs Skills | Pack de skills | Guides officiels pour intégrer la synthèse, le doublage, les bruitages et la musique d’ElevenLabs. Une clé API du service est requise. | 2026-11-10 | [ElevenLabs](https://github.com/elevenlabs/skills) |
| Fish S2 Skill | Skill + scripts | Pilote Fish Audio S2 Pro en local pour la narration expressive et les dialogues avec pistes séparées. Requiert ComfyUI, le pack de nœuds `ComfyUI-FishAudioS2` et FFmpeg. Le skill est sous MIT. Le modèle demande une licence distincte pour un usage commercial. | 2026-11-10 | [Fish S2 Skill](https://github.com/ruashots/fish-s2-skill) · [Licence du modèle](https://huggingface.co/fishaudio/s2-pro#license) |

## Automatisation et services autohébergeables

| Nom | Type | Usage et prérequis | Vérifié le | Source |
| --- | --- | --- | --- | --- |
| n8n | Plateforme + MCP | Automatise des workflows entre applications. Son MCP intégré peut déclencher les workflows exposés et, selon la version, les créer ou les modifier. La Sustainable Use License encadre notamment l’usage commercial. | 2026-11-10 | [n8n](https://github.com/n8n-io/n8n) · [Documentation MCP](https://docs.n8n.io/connect/connect-to-n8n-mcp-server) · [Licence](https://github.com/n8n-io/n8n/blob/master/LICENSE.md) |
| Plausible | Application web | Mesure l’audience d’un site. La Community Edition est distribuée sous AGPL et fournit une configuration Docker Compose pour l’autohébergement. | 2026-11-10 | [Plausible](https://github.com/plausible/analytics) · [Community Edition](https://github.com/plausible/community-edition) |
| AppFlowy | Application + serveur | Wiki, documents et suivi de projets collaboratifs. Pour partager un espace en autohébergement, le mainteneur documente le déploiement d’AppFlowy Cloud. | 2026-11-10 | [AppFlowy](https://github.com/AppFlowy-IO/AppFlowy) |
| Cal.diy | Application web | Prise de rendez-vous autohébergée, sous licence MIT. Le lien GitHub `calcom/cal.com` cité dans le post redirige vers `calcom/cal.diy`. PostgreSQL est requis. | 2026-11-10 | [Cal.diy](https://github.com/calcom/cal.diy) |
| Bitwarden | Serveur + CLI distincte | Coffre-fort de mots de passe autohébergeable. Pour les secrets d’un workflow, Bitwarden documente une CLI dédiée dans Secrets Manager. | 2026-11-10 | [Bitwarden Server](https://github.com/bitwarden/server) · [Secrets Manager CLI](https://bitwarden.com/help/secrets-manager-cli/) |

## Développement et tests web

| Nom | Type | Usage et prérequis | Vérifié le | Source |
| --- | --- | --- | --- | --- |
| Playwright MCP | MCP | Piloter un navigateur pour reproduire un parcours web. Node.js 18+ selon le README. | 2026-11-10 | [Microsoft](https://github.com/microsoft/playwright-mcp) |
| Chrome DevTools | MCP + CLI | Diagnostique un problème dans Chrome à partir des traces de performance, des requêtes réseau ou des erreurs de console. Chrome stable et Node.js LTS selon le dépôt. | 2026-11-10 | [Chrome DevTools](https://github.com/ChromeDevTools/chrome-devtools-mcp) |
| Context7 | MCP + CLI | Récupère de la documentation et des exemples pour une version de bibliothèque. Service distant, avec clé recommandée pour des quotas plus élevés. | 2026-11-10 | [Upstash](https://github.com/upstash/context7) |
| Serena | MCP | Navigue dans les définitions et les références et permet des modifications par symbole. S’appuie sur un serveur de langage ou sur son intégration JetBrains selon la configuration. | 2026-11-10 | [Serena](https://github.com/oraios/serena) |
| GitHub MCP Server | MCP | Consulte dépôts, issues, pull requests et résultats de CI. Le serveur officiel permet de choisir les groupes d’outils et propose un mode lecture seule. | 2026-11-10 | [GitHub](https://github.com/github/github-mcp-server) |
| Supabase MCP | MCP | Inspecte les schémas et les tables d’un projet Supabase. La connexion peut être limitée à un projet et aux outils en lecture seule. | 2026-11-10 | [Supabase](https://github.com/supabase/mcp) |
| Matt Pocock Skills | Pack de skills | `grill-with-docs` aide à clarifier un besoin et consigner les décisions. `tdd` guide les boucles de développement pilotées par les tests. Le dépôt documente un plugin Codex. | 2026-11-10 | [Matt Pocock](https://github.com/mattpocock/skills) |
| OpenSpec | CLI + workflows | Conserve dans le dépôt des propositions, des exigences et des tâches que l’agent peut relire pendant l’implémentation. L’installation via npm demande Node.js 22.12+. | 2026-11-10 | [OpenSpec](https://github.com/Fission-AI/OpenSpec) |
| Microsoft Agent Framework Builder Skills | Pack de skills | Guides officiels .NET et Python pour concevoir des agents, leurs outils, leurs sessions et leurs workflows. Le projet applicatif utilise le SDK correspondant et les accès de son fournisseur de modèles. | 2026-11-10 | [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) · [Documentation des skills](https://devblogs.microsoft.com/agent-framework/give-your-coding-agent-a-head-start-with-microsoft-agent-framework-skills-for-net-and-python/) |
| FastMCP | Bibliothèque Python + CLI | Construit des serveurs et des clients MCP, notamment pour exposer des fonctions Python comme outils. Python 3.11+ et licence Apache-2.0 selon le dépôt. | 2026-11-10 | [FastMCP](https://github.com/PrefectHQ/fastmcp) · [Documentation](https://gofastmcp.com/docs/getting-started/installation) |
| MCP Inspector | Application web + CLI + TUI | Inspecte les outils et ressources d’un serveur MCP et permet de tester les appels, y compris depuis une CI. La version 2 requiert une version compatible de Node.js. Les paramètres de connexion peuvent inclure des secrets. | 2026-11-10 | [MCP Inspector](https://github.com/modelcontextprotocol/inspector) · [Documentation MCP](https://modelcontextprotocol.io/docs/tools/inspector) |

## Recherche et observabilité des agents

| Nom | Type | Usage et prérequis | Vérifié le | Source |
| --- | --- | --- | --- | --- |
| Exa MCP | MCP + skills | Recherche sur le Web et récupère le contenu des pages pour une veille. Le serveur hébergé accepte des requêtes anonymes avec quotas. Les fonctions Exa Agent demandent une authentification. | 2026-11-10 | [Exa](https://github.com/exa-labs/exa-mcp-server) |
| Qdrant | Base vectorielle + API | Indexe des embeddings pour retrouver des passages ou objets par similarité, avec filtres sur les métadonnées. Déploiement local ou hébergé. | 2026-11-10 | [Qdrant](https://github.com/qdrant/qdrant) |
| Langfuse | Plateforme + SDK | Trace les appels aux modèles et aux outils, mesure l’usage et évalue des workflows d’agents. Les SDK envoient les traces vers une instance hébergée ou autohébergée. | 2026-11-10 | [Langfuse](https://github.com/langfuse/langfuse) |
| Sentry Toolkit | MCP + CLI | Recherche les erreurs et les traces d’une application dans Sentry et aide à trier les incidents. Le MCP distant prend en charge OAuth et peut être limité à un projet. L’ancien dépôt `getsentry/sentry-mcp` redirige vers le Toolkit. | 2026-11-10 | [Sentry Toolkit](https://github.com/getsentry/toolkit) · [Documentation MCP](https://mcp.sentry.dev/) |

## Tenir le catalogue à jour

1. **Repérer.** Consulter les nouvelles sources partagées, les releases des dépôts déjà suivis et les annuaires. [skills.sh](https://skills.sh/) · [Registre officiel MCP](https://registry.modelcontextprotocol.io/)
2. **Vérifier.** Ouvrir la source officielle, le README, la licence et, selon le type, `SKILL.md` ou le manifeste MCP. Relever le client compatible, les dépendances, les services et clés requis, les permissions et les coûts documentés qui changent la décision d’adoption.
3. **Mettre à jour.** Dédupliquer par URL canonique et comparer les usages des projets similaires. Regrouper les composants d’un même projet sur une fiche si le choix se fait ensemble. Ajouter ou corriger la ligne dans sa catégorie et dater uniquement les entrées relues. Signaler un lien rompu ou un dépôt archivé, avec son successeur si le mainteneur en indique un.
4. **Après un essai.** Ajouter sous l’entrée le client, le système, la version testée, la date, le scénario et le résultat. Avant un nouvel essai, relire la documentation si la dernière vérification date de plus de trois mois.

Demande réutilisable à donner à un agent.

> Mets à jour `agent-extension/README.md` à partir des nouvelles sources que je te donne. Vérifie chaque ajout dans la documentation du mainteneur, repère les doublons, note les prérequis qui changent la décision d’essai et date les lignes relues. Limite le travail à la mise à jour du catalogue.
