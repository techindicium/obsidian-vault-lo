---
type: concept
name: "Retrieval-Augmented Generation (RAG)"
aliases: ["RAG"]
description: "An architecture that grounds an LLM's output by retrieving relevant content from an external knowledge source (often a vector database) and injecting it into the model's context before generation."
related_to: ["[[aisvs-standard]]", "[[aisvs-core-categories]]", "[[hallucination]]", "[[data-poisoning]]"]
sources:
  - url: "https://github.com/OWASP/AISVS"
    type: "github-repo"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
graphify_node_ids: ["aisvs_rag"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Retrieval-Augmented Generation (RAG)

> Grounding an LLM's output in retrieved external content — typically from a vector database of embeddings — instead of relying solely on what the model learned during training.

## Description

RAG is a widely used [[hallucination|hallucination]] mitigation: by injecting retrieved, sourced content into the model's context, output can be grounded in verifiable material rather than the model's parametric memory alone. But the retrieval layer becomes a new attack surface in its own right — if the underlying vector database or embedding pipeline is compromised via [[data-poisoning|data poisoning]], the model can be made to confidently ground its answer in fabricated or malicious retrieved content. AISVS treats memory/embeddings/vector-database security as its own control category precisely because of this dependency.

## Key Characteristics

- Retrieves relevant content at generation time rather than relying only on training-time knowledge.
- Reduces but does not eliminate [[hallucination|hallucination]] risk — grounding in compromised or poisoned retrieved content produces confidently wrong output too.
- Its security depends on the integrity of the retrieval/vector-database layer, not just the model.

## Where it Applies

- [[aisvs-core-categories]] — Memory, Embeddings & Vector Database Security (C08) covers RAG's retrieval-layer security specifically

## Related Concepts

- [[hallucination]] — the primary problem RAG is designed to mitigate
- [[data-poisoning]] — the attack vector against RAG's retrieval layer
