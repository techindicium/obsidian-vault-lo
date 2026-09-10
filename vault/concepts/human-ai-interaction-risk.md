---
type: concept
name: "AI Risk Management and Human-AI Interaction"
aliases: ["Human-AI Interaction Risk"]
description: "The AI RMF's treatment (Appendix C) of risks arising specifically from how humans interact with, rely on, oversee, or are affected by AI systems — over-reliance, automation bias, and the need for meaningful human oversight."
related_to: ["[[nist-ai-risk-management-framework]]", "[[ai-actor-taxonomy]]"]
sources:
  - url: "https://www.nist.gov/itl/ai-risk-management-framework"
    type: "remote-binary"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
graphify_node_ids: ["nist_ai_100_1_human_ai_interaction"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# AI Risk Management and Human-AI Interaction

> The AI RMF's Appendix C treatment of risks that arise specifically at the interface between people and AI systems — not risks in the model itself, but in how humans use, trust, and are affected by it.

## Description

Many AI risks materialize only through human interaction with the system: users over-relying on outputs they should scrutinize (automation bias), operators lacking the context or authority to meaningfully override the system, or affected individuals having no effective way to contest or seek recourse for a harmful outcome. This dimension cuts across the [[ai-actor-taxonomy|actor taxonomy]] — end users, human-factors specialists, and affected individuals/communities each carry distinct interaction risks the AI RMF asks organizations to account for.

## Key Characteristics

- Risk can arise from correct model behavior interacting badly with human trust/oversight patterns, not only from model error.
- Automation bias — the tendency to over-trust AI outputs — is a named concern.
- Meaningful human oversight and contestability for affected individuals are treated as risk-management requirements, not afterthoughts.

## Where it Applies

- [[ai-actor-taxonomy]] — end users, human factors, and affected individuals/communities are the actor categories most directly implicated

## Related Concepts

- [[nist-ai-risk-management-framework]]
