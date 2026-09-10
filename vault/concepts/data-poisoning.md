---
type: concept
name: "Data Poisoning"
aliases: ["Training Data Poisoning"]
description: "An attack that corrupts an AI system by injecting malicious or manipulated data into its training set, fine-tuning data, or retrieval/embedding store, so the system learns or retrieves compromised information."
related_to: ["[[aisvs-standard]]", "[[aisvs-core-categories]]", "[[retrieval-augmented-generation]]", "[[model-extraction]]", "[[genai-top10-standard]]", "[[ai-supply-chain-risk]]", "[[vector-and-embedding-weaknesses]]"]
sources:
  - url: "https://github.com/GenAI-Security-Project/GenAI-LLM-Top10"
    type: "github-repo"
    synced_at: "2026-09-10"
  - url: "https://github.com/OWASP/AISVS"
    type: "github-repo"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
graphify_node_ids: ["aisvs_data_poisoning", "genai_top10_llm05_data_model_poisoning"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Data Poisoning

> Corrupting an AI system's behavior by injecting manipulated data into what it learns from or retrieves at inference time — training data, fine-tuning data, or a RAG vector store.

## Description

Data poisoning can target training-time data (corrupting what the model learns during training or fine-tuning) or inference-time retrieval data (corrupting what a [[retrieval-augmented-generation|RAG]] system retrieves and grounds its answers in). Both variants exploit the same underlying weakness: the system trusts data it should be validating and tracking provenance for. AISVS addresses training-time poisoning primarily under Training Data Integrity & Traceability, and retrieval-time poisoning under Memory, Embeddings & Vector Database Security.

## Key Characteristics

- Two attack surfaces: training/fine-tuning data, and RAG retrieval/embedding stores.
- Exploits missing data provenance and validation, not a flaw in the model architecture itself.
- Distinct from but related to [[model-extraction|model extraction]] — poisoning corrupts what a model knows; extraction steals what it knows.

## Where it Applies

- [[aisvs-core-categories]] — Training Data Integrity & Traceability (C01) and Memory/Embeddings/Vector Database Security (C08) both address data poisoning, at different lifecycle stages

## Ranking (OWASP GenAI LLM Top 10 2026)

Listed as **LLM05: Data and Model Poisoning** in the [[genai-top10-standard|OWASP Top 10 for LLM Applications and Generative AI (2026)]], ranked #5. The 2026 list treats it as overlapping with, but narrower than, [[ai-supply-chain-risk|Supply Chain]] (LLM04) — poisoning is one specific corruption mechanism within the broader third-party-trust problem supply chain risk covers — and as closely linked to [[vector-and-embedding-weaknesses|Vector and Embedding Weaknesses]] (LLM09), which covers the retrieval layer's security more broadly beyond just poisoning.

## Related Concepts

- [[retrieval-augmented-generation]] — the primary inference-time target of retrieval-store poisoning
- [[model-extraction]] — a related but distinct attack that steals rather than corrupts model knowledge
- [[genai-top10-standard]] — ranked #5 (LLM05) in the 2026 OWASP LLM Top 10
