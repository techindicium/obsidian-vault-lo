---
type: concept
name: "Unbounded Consumption"
aliases: ["LLM06:2026", "Resource Exhaustion (AI)"]
description: "A risk where an AI application allows uncontrolled resource consumption — excessive inference calls, uncapped context/token usage, or unbounded agentic action loops — leading to denial of service or runaway cost."
related_to: ["[[genai-top10-standard]]", "[[excessive-agency]]", "[[ai-supply-chain-risk]]"]
sources:
  - url: "https://github.com/GenAI-Security-Project/GenAI-LLM-Top10"
    type: "github-repo"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
graphify_node_ids: ["genai_top10_llm06_unbounded_consumption"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Unbounded Consumption

> Uncontrolled resource consumption by an AI application — excessive inference calls, uncapped context/token usage, or an agent looping without a resource ceiling — leading to denial of service or runaway operating cost.

## Description

This risk shares its root cause with [[excessive-agency|Excessive Agency]] (an under-bounded agent can consume resources without limit, not just take unauthorized actions) and with third-party/infrastructure dependencies covered by [[ai-supply-chain-risk|Supply Chain]] (rate limits and quotas on upstream model providers are part of the mitigation surface). Left unmitigated, this is both a reliability risk (denial of service) and a financial risk (uncontrolled inference cost).

## Key Characteristics

- Manifests as denial of service, runaway cost, or both.
- Root cause shared with excessive agency: absence of a hard ceiling on resource use, not just action scope.
- Mitigations include rate limiting, token/cost budgets per request or session, and agent loop/step limits.

## Where it Applies

- [[genai-top10-standard]] — ranked #6 in the 2026 OWASP LLM Top 10

## Related Concepts

- [[excessive-agency]] — shares the "missing bound on autonomous behavior" root cause
- [[ai-supply-chain-risk]] — infrastructure-level rate limiting is part of the mitigation surface
