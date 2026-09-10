---
type: concept
name: "Misinformation"
aliases: ["LLM07:2026", "AI-Generated Misinformation"]
description: "A risk where an AI application produces or amplifies false or misleading information that is consumed and acted upon as if it were accurate — the applied, downstream-harm-focused counterpart to hallucination."
related_to: ["[[genai-top10-standard]]", "[[hallucination]]", "[[improper-output-handling]]"]
sources:
  - url: "https://github.com/GenAI-Security-Project/GenAI-LLM-Top10"
    type: "github-repo"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
graphify_node_ids: ["genai_top10_llm07_misinformation"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Misinformation

> An AI application producing or amplifying false or misleading content that a user or downstream system acts on as if it were accurate — the real-world-harm framing of what [[hallucination|hallucination]] describes as a model behavior.

## Description

Misinformation is closely related to [[hallucination|hallucination]] but frames the risk from the consequence side: it doesn't matter whether false output came from the model confabulating or from it faithfully repeating false content it was fed — either way, a user or a downstream automated system ([[improper-output-handling|if output is passed on unhandled]]) can act on it as fact. This risk is why hallucination is treated as a security-relevant, testable requirement rather than only a UX quality issue.

## Key Characteristics

- Consequence-focused: the harm is downstream action taken on false information, regardless of its internal cause.
- Overlaps heavily with [[hallucination|hallucination]] but isn't limited to model-fabricated content — it also covers faithfully repeated false input.
- Compounded when output flows downstream without validation (see [[improper-output-handling]]).

## Where it Applies

- [[genai-top10-standard]] — ranked #7 in the 2026 OWASP LLM Top 10

## Related Concepts

- [[hallucination]] — the model-behavior mechanism most often behind this risk
- [[improper-output-handling]] — determines whether misinformation propagates downstream unchecked
