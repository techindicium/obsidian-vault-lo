---
type: concept
name: "AI RMF Risk-Framing Challenges"
aliases: ["Risk Tolerance", "Risk Prioritization", "Risk Measurement"]
description: "Three interlocking challenges the AI RMF names for framing AI risk: risk measurement (AI risks are often hard to quantify), risk tolerance (how much risk is acceptable, and to whom), and risk prioritization (which risks to address first given constrained resources)."
related_to: ["[[nist-ai-risk-management-framework]]", "[[ai-rmf-core-functions]]", "[[trustworthy-ai-characteristics]]"]
sources:
  - url: "https://www.nist.gov/itl/ai-risk-management-framework"
    type: "remote-binary"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
graphify_node_ids: ["nist_ai_100_1_risk_tolerance", "nist_ai_100_1_risk_prioritization", "nist_ai_100_1_risk_measurement"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# AI RMF Risk-Framing Challenges

> Three interlocking problems the AI RMF names as harder for AI than for traditional systems: measuring risk, setting risk tolerance, and prioritizing which risks to act on.

## Description

Before an organization can act (via the [[ai-rmf-core-functions|MEASURE and MANAGE functions]]), it has to resolve these three framing questions, each complicated by the nature of AI systems and the trade-offs between [[trustworthy-ai-characteristics|trustworthiness characteristics]]:

## The Three Challenges

### Risk Measurement
AI risks are frequently difficult to reliably measure due to factors such as inadequate metrics for emergent properties, contextual dependence of harms, and the fact that some impacts (e.g., societal, reputational) resist clean quantification the way traditional software defect rates do.

### Risk Tolerance
How much risk an organization — or society — is willing to accept is not fixed; it varies by sector, use case, regulatory context, and stakeholder, and the AI RMF deliberately does not prescribe a single tolerance level, leaving that judgment to the adopting organization within its own risk appetite.

### Risk Prioritization
Given finite resources, organizations must decide which risks to address first. This requires weighing severity, likelihood, and the trade-offs between different [[trustworthy-ai-characteristics|trustworthiness characteristics]] (e.g., a fix that improves fairness might reduce explainability), not just ranking risks on a single axis.

## Where it Applies

- [[ai-rmf-core-functions]] — MEASURE and MANAGE directly operationalize responses to these challenges
- [[trustworthy-ai-characteristics]] — prioritization requires weighing these characteristics against each other

## Related Concepts

- [[nist-ai-risk-management-framework]]
