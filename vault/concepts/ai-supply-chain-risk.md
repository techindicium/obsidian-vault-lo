---
type: concept
name: "AI Supply Chain Risk"
aliases: ["LLM04:2026 Supply Chain"]
description: "Risk introduced by third-party components an AI system depends on — pretrained models, datasets, fine-tuning adapters, plugins, or MCP tool packages — whose integrity and provenance may not be verifiable."
related_to: ["[[genai-top10-standard]]", "[[data-poisoning]]", "[[model-context-protocol]]", "[[aisvs-core-categories]]"]
sources:
  - url: "https://github.com/GenAI-Security-Project/GenAI-LLM-Top10"
    type: "github-repo"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
graphify_node_ids: ["genai_top10_llm04_supply_chain"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# AI Supply Chain Risk

> Risk introduced by any third-party component an AI system depends on — a pretrained model, a dataset, a fine-tuning adapter, a plugin, or a tool package invoked over [[model-context-protocol|MCP]] — whose provenance and integrity the consuming system can't fully verify.

## Description

This risk overlaps directly with [[data-poisoning|Data and Model Poisoning]] (LLM05): a poisoned upstream dataset or model is itself a supply-chain compromise, but the 2026 OWASP list treats supply chain as the broader "what third-party pieces am I trusting, and how do I verify them" question, while data/model poisoning focuses specifically on the corruption mechanism. Compromised tool packages invoked by an agent over MCP are called out as a specific 2026 concern connecting this risk to [[excessive-agency|Excessive Agency]] — a compromised tool can be misused by an over-privileged agent.

## Key Characteristics

- Covers models, datasets, fine-tuning adapters, plugins, and MCP tool packages as distinct supply-chain components.
- Overlaps with, but is broader than, [[data-poisoning|data/model poisoning]] — poisoning is one mechanism of supply-chain compromise.
- Mitigation emphasis: signing and provenance verification for models/datasets/packages, similar in spirit to software supply-chain security (SBOM-style tracking).

## Where it Applies

- [[genai-top10-standard]] — ranked #4 in the 2026 OWASP LLM Top 10
- [[aisvs-core-categories]] — AISVS's Supply Chain Security for Models (C06) addresses the same risk from a verification-requirements angle

## Related Concepts

- [[data-poisoning]] — a specific corruption mechanism within the broader supply chain risk
- [[model-context-protocol]] — MCP tool packages are a named supply-chain component in the 2026 list
