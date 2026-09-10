---
type: concept
name: "Vector and Embedding Weaknesses"
aliases: ["LLM09:2026"]
description: "Security weaknesses in the vector-store/embedding layer that RAG systems depend on — unauthorized retrieval, embedding inversion, and poisoning of the retrieval index."
related_to: ["[[genai-top10-standard]]", "[[retrieval-augmented-generation]]", "[[data-poisoning]]", "[[ai-supply-chain-risk]]", "[[sensitive-information-disclosure]]"]
sources:
  - url: "https://github.com/GenAI-Security-Project/GenAI-LLM-Top10"
    type: "github-repo"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
graphify_node_ids: ["genai_top10_llm09_vector_and_embedding_weaknesses"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Vector and Embedding Weaknesses

> Security weaknesses in the vector-store/embedding layer underlying [[retrieval-augmented-generation|RAG]] systems: unauthorized retrieval, embedding inversion, and poisoning of the retrieval index itself.

## Description

Where [[data-poisoning|Data and Model Poisoning]] (LLM05) focuses on corrupting what goes into a retrieval store, this risk covers the retrieval layer's own security weaknesses more broadly — including access control on the vector store (who can query or read from it) and embedding inversion, where an attacker reconstructs sensitive source content from its embedding representation (overlapping with [[sensitive-information-disclosure|Sensitive Information Disclosure]]). It's also treated as part of the broader third-party/dependency surface covered by [[ai-supply-chain-risk|Supply Chain]] when the vector database itself is an externally managed component.

## Key Characteristics

- Distinct from but related to poisoning: this risk also covers access control and embedding-inversion weaknesses, not just data corruption.
- Embedding inversion can reconstruct sensitive source content from vectors alone — a disclosure vector in its own right.
- The vector database is itself a supply-chain/infrastructure dependency worth securing as such.

## Where it Applies

- [[genai-top10-standard]] — ranked #9 in the 2026 OWASP LLM Top 10
- [[retrieval-augmented-generation]] — this risk targets RAG's retrieval layer specifically

## Related Concepts

- [[data-poisoning]] — the corruption mechanism against the same retrieval layer
- [[sensitive-information-disclosure]] — embedding inversion is a specific disclosure technique
- [[ai-supply-chain-risk]] — the vector store as a third-party/infrastructure dependency
