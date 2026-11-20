# Newsjacking V0 · AI Disclosure Statement

Inventaire initial du 18 novembre 2026.

## Modèles déclarés dans le workflow

| Modèle | Fournisseur du modèle | Offre utilisée et rôle |
| --- | --- | --- |
| GPT-OSS 120B · `openai/gpt-oss-120b` | OpenAI | API **GroqCloud** via Groq Chat Model dans n8n. Structure le contexte de l’entreprise, sélectionne les sujets et propose des angles, puis rédige le brouillon. Trois nœuds utilisent ce même modèle. L’abonnement GroqCloud exact n’est pas consigné dans l’export. |
| FLUX.1 [schnell] · `@cf/black-forest-labs/flux-1-schnell` | Black Forest Labs | API **Cloudflare Workers AI**, appelée pour le format post LinkedIn avec image. La recette de référence portait sur la newsletter et le doublon. L’abonnement Cloudflare exact n’est pas consigné dans l’export. |

Documentation des offres et modèles · [GPT-OSS 120B sur GroqCloud](https://console.groq.com/docs/model/openai/gpt-oss-120b) · [FLUX.1 [schnell] sur Workers AI](https://developers.cloudflare.com/workers-ai/models/flux-1-schnell/)

## Services utilisés pendant l’exécution

| Service | Contribution |
| --- | --- |
| Tavily Search et Extract | Recherche d’actualités et extraction de texte de pages publiques. Appels API direct avec l’identifiant n8n. Aucun modèle sous-jacent n’est sélectionné dans l’export. |
| Jina AI Reader | Lecture de pages publiques pour obtenir du texte exploitable. Aucun modèle sous-jacent n’est sélectionné dans l’export. |

## Outils d’IA employés pour la construction

| Outil et fournisseur | Offre et contribution |
| --- | --- |
| ChatGPT / Codex · OpenAI | Session de travail ChatGPT avec Codex. A aidé à concevoir et à implémenter le workflow n8n, rédiger les instructions des modèles, ajuster les écrans, corriger les erreurs observées et construire les tests et les livrables. L’historique de construction ne consigne pas le modèle exact pour chacune des contributions. |

L’agent produit des brouillons et des propositions de sources. La validation humaine porte sur l’angle, le texte final et les passages qui justifient les affirmations. Lors de l’essai SprechenEasy, une mention de partenariat a été corrigée avant validation car les sources ne l’établissaient pas.
