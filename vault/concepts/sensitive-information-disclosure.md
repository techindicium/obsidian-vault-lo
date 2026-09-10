---
type: concept
name: "Sensitive Information Disclosure"
aliases: ["LLM02:2026", "AI Data Leakage"]
description: "A risk where an LLM application reveals sensitive data — PII, credentials, proprietary information, or training-data fragments — in its output, either directly or inferable from responses."
related_to: ["[[genai-top10-standard]]", "[[model-extraction]]", "[[vector-and-embedding-weaknesses]]"]
sources:
  - url: "https://github.com/GenAI-Security-Project/GenAI-LLM-Top10"
    type: "github-repo"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
graphify_node_ids: ["genai_top10_llm02_sensitive_information_disclosure"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Sensitive Information Disclosure

> An LLM application leaking sensitive data — personal information, credentials, proprietary business data, or fragments memorized from training data — through its normal output.

## Description

Disclosure can happen directly (the model states sensitive data verbatim) or through inference (an attacker reconstructs sensitive data by combining multiple responses) — the latter overlapping with [[model-extraction|model extraction]] techniques and embedding-inversion attacks against [[vector-and-embedding-weaknesses|vector/embedding stores]]. Excessive permissions granted to an agent (see [[excessive-agency|Excessive Agency]]) can also expose sensitive data the agent shouldn't have surfaced in the first place.

## Key Characteristics

- Direct leakage (verbatim sensitive output) vs. inferential leakage (reconstructed across multiple interactions).
- Overlaps with embedding-inversion risk in RAG/vector-store architectures.
- Amplified when an agent holds broader data access than its task requires.

## Where it Applies

- [[genai-top10-standard]] — ranked #2 in the 2026 OWASP LLM Top 10

## Related Concepts

- [[model-extraction]] — shares the black-box, inference-based extraction technique
- [[vector-and-embedding-weaknesses]] — embedding inversion is a specific disclosure vector
