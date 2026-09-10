---
type: concept
name: "AI Lifecycle Dimensions"
aliases: ["AI System Lifecycle"]
description: "The stages an AI system moves through — from design through decommissioning — that the AI RMF's functions and actor tasks are mapped onto, so risk management applies continuously rather than only at deployment."
related_to: ["[[nist-ai-risk-management-framework]]", "[[ai-rmf-core-functions]]", "[[ai-actor-taxonomy]]"]
sources:
  - url: "https://www.nist.gov/itl/ai-risk-management-framework"
    type: "remote-binary"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
graphify_node_ids: ["nist_ai_100_1_ai_lifecycle"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# AI Lifecycle Dimensions

> The stages an AI system passes through over its life — the axis the AI RMF uses to show that risk management must be continuous, not a one-time pre-deployment check.

## Description

The AI RMF explicitly rejects a "test once at the end" model of AI risk management. Instead, its [[ai-rmf-core-functions|four core functions]] and its [[ai-actor-taxonomy|actor task categories]] (AI Design, Development, Deployment, Operation and Monitoring, TEVV) are all mapped onto lifecycle stages, so that governance, mapping, measurement, and management activities recur at every stage as the system, its data, and its context of use evolve.

## Key Characteristics

- Spans from initial design through operation/monitoring, not just "build then ship."
- The same actor task categories recur at different lifecycle points with different responsibilities.
- Risk isn't a fixed, one-time property of a system — it changes as the system moves through its lifecycle (new data, new use contexts, model drift).

## Where it Applies

- [[ai-rmf-core-functions]] — the four functions are applied continuously across every lifecycle stage
- [[ai-actor-taxonomy]] — actor task categories are defined relative to lifecycle stages

## Related Concepts

- [[nist-ai-risk-management-framework]]
