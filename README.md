# AI isn't magic: try this Monday
# L'IA, ce n'est pas de la magie : à essayer lundi

DevFest Montréal 2026 · Stacy Véronneau

One thing to try for each part of the machine. Pick one; you don't need them all.
*Une chose à essayer pour chaque pièce de la machine. Choisissez-en une; pas besoin de tout faire.*

## 1. The engine · Le moteur

**Run your PyTorch code on TPUs, no JAX required.** TorchTPU is open source: debug in eager mode, then move to `torch.compile` for production.
*Faites rouler votre code PyTorch sur des TPU, sans JAX. TorchTPU est en code source ouvert.*
→ https://cloud.google.com/blog/topics/ai-infrastructure/torchtpu-is-now-open-source-run-native-pytorch-on-tpus

**Pick the smallest model that does the job, and pin it.** Defaults change: one Google tool switched its default model, and its price, in October.
*Choisissez le plus petit modèle qui fait le travail, et fixez-le dans votre code. Les valeurs par défaut changent.*

## 2. The track · La piste

**Stream your AI answers through a gateway** with the same auth, rate limits and monitoring as the rest of your APIs (Public Preview).
*Diffusez les réponses de votre IA en continu à travers une passerelle, avec la même authentification et les mêmes limites (aperçu public).*
→ https://docs.cloud.google.com/api-gateway/docs/streaming-configure

## 3. Fuel & telemetry · Carburant et télémétrie

**Give your agents one shared meaning for your data.** Knowledge Catalog's self-learning enrichment keeps definitions current, and each team can keep its own (Preview).
*Donnez à vos agents un seul sens commun pour vos données. L'enrichissement autoapprenant de Knowledge Catalog garde les définitions à jour (aperçu).*
→ https://cloud.google.com/blog/products/data-analytics/knowledge-catalog-self-learning-context-enrichment-for-ai-agents

**Chunk documents for retrieval (RAG) right in SQL**, with BigQuery's `AI.CHUNK_DOCUMENT`.
*Découpez vos documents pour la recherche augmentée (RAG) directement en SQL avec `AI.CHUNK_DOCUMENT` dans BigQuery.*
→ https://docs.cloud.google.com/bigquery/docs/reference/standard-sql/bigqueryml-syntax-ai-chunk-document

## 4. The barriers · Les barrières

**Put the helmet on:** screen prompts, responses and documents for prompt injection with Model Armor. It works in front of any model.
*Mettez le casque : filtrez requêtes, réponses et documents contre l'injection de requêtes avec Model Armor, devant n'importe quel modèle.*
→ https://docs.cloud.google.com/model-armor/overview

**Copy Google's own blueprint.** Its agentic reference architectures now include Agent Identity, Agent Gateway, Agent Registry and Model Armor.
*Copiez le plan de Google : ses architectures de référence pour agents intègrent maintenant Agent Identity, Agent Gateway, Agent Registry et Model Armor.*
→ https://docs.cloud.google.com/architecture/agentic-ai-orchestrate-security-ops-workflows

**Keep secrets out of your agent's context window:** out of prompts, tool results, logs and traces. See "Your Agent's Context Window Is Not a Vault" (featured in GCP Weekly #526).
*Gardez vos secrets hors de la fenêtre de contexte de vos agents : requêtes, résultats d'outils, journaux et traces.*

## 5. Paying for speed or heat? · La vitesse ou la chaleur?

**Set a budget kill switch** that disables billing when a project passes its budget. Google warns there's a delay in billing data, so set the cap below what you can actually afford to lose.
*Installez un coupe-circuit budgétaire qui désactive la facturation quand un projet dépasse son budget. Prévoyez une marge : les données de facturation arrivent avec un délai.*
→ https://docs.cloud.google.com/billing/docs/how-to/disable-billing-with-notifications

## 6. Swap the driver · Changez de pilote

**Build so you can swap models.** Google Cloud now offers Gemini, Claude and GPT (GPT in private preview), alongside 200+ other models.
*Concevez pour pouvoir changer de modèle. Google Cloud offre maintenant Gemini, Claude et GPT (GPT en aperçu privé), en plus de 200 autres modèles.*
→ https://cloud.google.com/blog/products/ai-machine-learning/google-cloud-brings-openai-models-to-customers

---

## Go deeper · Pour aller plus loin

- **ISO/IEC 27090:2026:** the first international standard on AI security threats (guidance, not a certification) · *la première norme internationale sur les menaces de sécurité de l'IA* → https://www.iso.org/standard/27090
- **OWASP Top 10 for LLM Applications (2026 edition):** data and model poisoning is #5 · *l'empoisonnement des données et des modèles est au 5e rang* → https://genai.owasp.org
- **MITRE ATT&CK v20:** indirect prompt injection is now its own technique · *l'injection indirecte de requêtes est maintenant une technique à part entière* → https://attack.mitre.org
- **The demo from the talk (pizza bot + Model Armor):** *pizza-demo.sh in this Repo*

*Questions? Find me on LinkedIn: Stacy Véronneau · GDG Cloud Montréal*
