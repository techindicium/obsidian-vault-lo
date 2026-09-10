---
type: concept
name: "Hallucination"
aliases: ["AI Hallucination", "Model Hallucination"]
description: "An AI model producing output that is fabricated, factually incorrect, or unsupported by its training data or retrieved context, while presented with the same confidence as accurate output."
related_to: ["[[aisvs-standard]]", "[[aisvs-core-categories]]", "[[retrieval-augmented-generation]]", "[[guardrails]]"]
sources:
  - url: "https://github.com/OWASP/AISVS"
    type: "github-repo"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
graphify_node_ids: ["aisvs_hallucination"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Hallucination

> A model producing fabricated or factually wrong output with the same apparent confidence as correct output — a core reliability risk distinct from a security exploit, but treated by AISVS as a verifiable, testable requirement.

## Description

Hallucination is treated in AISVS as part of Model Behavior, Output Control & Safety Assurance — an assurance property to be tested and monitored, not just a known model limitation to shrug off. [[retrieval-augmented-generation|RAG]] is a common mitigation (grounding output in retrieved source content), but a poorly secured retrieval layer can itself introduce fabricated or poisoned context that produces confidently wrong output — so RAG reduces but does not eliminate hallucination risk, and both need to be verified together.

## Key Characteristics

- Output-confidence and factual-accuracy are decoupled — a hallucination can be delivered as fluently and confidently as a correct answer.
- Distinguishing it as a testable requirement (not just accepted behavior) is central to AISVS's Model Behavior category.
- [[retrieval-augmented-generation|RAG]] mitigates but doesn't eliminate hallucination risk — a compromised retrieval layer can produce confidently wrong grounded output too.
- Runtime monitoring (detecting hallucination patterns in production) is treated as a distinct, necessary layer alongside pre-deployment testing.

## Where it Applies

- [[aisvs-core-categories]] — addressed under Model Behavior (C07) and Monitoring/Logging (C12)

## Related Concepts

- [[retrieval-augmented-generation]] — a common mitigation, with its own security dependencies
- [[guardrails]] — output-side guardrails can catch some hallucinated content before delivery
