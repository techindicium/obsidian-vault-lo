---
type: concept
name: "OWASP Top 10 for LLM Applications and Generative AI (2026)"
aliases: ["OWASP GenAI LLM Top 10", "OWASP LLM Top 10 2026"]
description: "OWASP's community-driven, evidence-weighted ranking of the ten most critical security risks in LLM and generative-AI applications, published by the OWASP GenAI Security Project."
related_to: ["[[prompt-injection]]", "[[excessive-agency]]", "[[data-poisoning]]", "[[sensitive-information-disclosure]]", "[[ai-supply-chain-risk]]", "[[unbounded-consumption]]", "[[misinformation]]", "[[hidden-context-exposure]]", "[[vector-and-embedding-weaknesses]]", "[[improper-output-handling]]", "[[genai-top10-framework-mappings]]", "[[aisvs-standard]]"]
sources:
  - url: "https://github.com/GenAI-Security-Project/GenAI-LLM-Top10"
    type: "github-repo"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
graphify_node_ids: ["genai_top10_document", "genai_top10_methodology_2026_update"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# OWASP Top 10 for LLM Applications and Generative AI (2026)

> OWASP's ranked, evidence-weighted list of the ten most critical security risks facing LLM and generative-AI applications, maintained by the OWASP GenAI Security Project (30,000+ member community).

## Description

Published August 2026, this is the successor to the 2025 edition, re-ranked using an evidence-weighted methodology rather than purely subjective community voting — risks with more documented real-world incidents and stronger community consensus moved up or down accordingly. The ten 2026 risks are:

1. [[prompt-injection|LLM01: Prompt Injection]]
2. [[sensitive-information-disclosure|LLM02: Sensitive Information Disclosure]]
3. [[excessive-agency|LLM03: Excessive Agency]]
4. [[ai-supply-chain-risk|LLM04: Supply Chain]]
5. [[data-poisoning|LLM05: Data and Model Poisoning]]
6. [[unbounded-consumption|LLM06: Unbounded Consumption]]
7. [[misinformation|LLM07: Misinformation]]
8. [[hidden-context-exposure|LLM08: Hidden Context Exposure]]
9. [[vector-and-embedding-weaknesses|LLM09: Vector and Embedding Weaknesses]]
10. [[improper-output-handling|LLM10: Improper Output Handling]]

[[genai-top10-framework-mappings|Two appendices]] cross-reference these ten risks against external frameworks — including [[aisvs-standard|OWASP AISVS]], [[nist-ai-risk-management-framework|NIST AI RMF]], and [[mitre-atlas|MITRE ATLAS]] — so teams already following one of those frameworks can locate the corresponding LLM Top 10 coverage.

## 2026 Methodology Update

The 2026 edition introduced evidence-weighted reranking: risks are prioritized using documented incident evidence and severity data alongside community input, rather than community sentiment alone. This produced several rank migrations from 2025 — notably several risks tied to agentic behavior and supply chain moved up as agentic AI adoption grew, and [[hidden-context-exposure|Hidden Context Exposure]] is a new 2026 entry that wasn't in the 2025 list.

## Where it Applies

- [[aisvs-standard]] — cross-mapped via [[genai-top10-framework-mappings]]
- [[nist-ai-risk-management-framework]] — cross-mapped via [[genai-top10-framework-mappings]]

## Related Concepts

- [[genai-top10-framework-mappings]] — the appendices mapping these ten risks to external frameworks
