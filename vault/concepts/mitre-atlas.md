---
type: concept
name: "MITRE ATLAS"
aliases: ["ATLAS", "Adversarial Threat Landscape for AI Systems"]
description: "MITRE's knowledge base of adversarial machine-learning tactics and techniques observed against real AI systems, modeled on the structure of MITRE ATT&CK — cited by AISVS as a threat-pattern source behind several of its requirements."
related_to: ["[[aisvs-standard]]", "[[data-poisoning]]", "[[adversarial-example]]", "[[model-extraction]]", "[[genai-top10-framework-mappings]]"]
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
graphify_node_ids: ["aisvs_mitre_atlas", "genai_top10_mitre_atlas_ref"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# MITRE ATLAS

> MITRE's knowledge base of adversarial machine-learning tactics and techniques actually observed against AI systems, structured like MITRE ATT&CK but for AI/ML-specific threats.

## Description

Captured here as a lightweight reference stub because [[aisvs-standard|AISVS]] cites ATLAS as source material behind several of its requirements — particularly around [[data-poisoning|data poisoning]], [[adversarial-example|adversarial examples]], and [[model-extraction|model extraction]], all of which correspond to named ATLAS technique categories. This entry should be expanded if a future source in this vault ingests ATLAS directly.

## Where it Applies

- [[aisvs-standard]] — cited as a threat-pattern source for several core control categories

The [[genai-top10-framework-mappings|OWASP GenAI LLM Top 10 (2026)]] also cites ATLAS, mapping it as a primary reference against all ten of its risks — the broadest cross-reference of any framework in that standard's coverage matrix.

## Related Concepts

- [[data-poisoning]]
- [[adversarial-example]]
- [[model-extraction]]
- [[genai-top10-framework-mappings]] — maps ATLAS against all ten OWASP LLM Top 10 risks
