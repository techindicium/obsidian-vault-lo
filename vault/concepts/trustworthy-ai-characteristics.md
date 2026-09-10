---
type: concept
name: "Trustworthy AI Characteristics"
aliases: ["Trustworthy AI", "AI Trustworthiness"]
description: "The seven characteristics NIST's AI RMF uses to define trustworthy AI: valid & reliable, safe, secure & resilient, accountable & transparent, explainable & interpretable, privacy-enhanced, and fair with harmful bias managed."
related_to: ["[[nist-ai-risk-management-framework]]", "[[ai-rmf-core-functions]]"]
sources:
  - url: "https://www.nist.gov/itl/ai-risk-management-framework"
    type: "remote-binary"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
graphify_node_ids: ["nist_ai_100_1_trustworthy_ai", "nist_ai_100_1_valid_and_reliable", "nist_ai_100_1_safe", "nist_ai_100_1_secure_and_resilient", "nist_ai_100_1_accountable_and_transparent", "nist_ai_100_1_explainable_and_interpretable", "nist_ai_100_1_privacy_enhanced", "nist_ai_100_1_fair_with_harmful_bias_managed"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Trustworthy AI Characteristics

> The seven characteristics the [[nist-ai-risk-management-framework|NIST AI RMF]] uses to define what makes an AI system trustworthy, each requiring trade-offs against the others depending on context.

## Description

No single characteristic guarantees trustworthiness on its own, and improving one can trade off against another (e.g., stronger privacy protection can reduce explainability). The AI RMF treats these seven as jointly necessary and context-dependent, to be balanced through the [[ai-rmf-core-functions|GOVERN, MAP, MEASURE, and MANAGE functions]].

## The Seven Characteristics

- **Valid and Reliable** — the system performs as intended, and its outputs can be confirmed accurate under expected conditions.
- **Safe** — the system does not endanger human life, health, property, or the environment under normal or foreseeable misuse conditions.
- **Secure and Resilient** — the system withstands and recovers from adverse events, attacks, and unauthorized access.
- **Accountable and Transparent** — the organization deploying the system can be held responsible for its impacts, and there is visibility into how it operates.
- **Explainable and Interpretable** — humans can understand and reason about how the system reaches its outputs.
- **Privacy-Enhanced** — the system safeguards human autonomy and reduces risks to privacy from data collection, use, and inference.
- **Fair — with Harmful Bias Managed** — the system avoids reinforcing unjust discrimination or unfair outcomes across groups.

## Where it Applies

- [[nist-ai-risk-management-framework]] — trustworthiness is the outcome the entire framework is organized to promote
- [[ai-rmf-core-functions]] — the four functions operationalize the trade-offs between these characteristics

## Related Concepts

- [[ai-rmf-risk-framing-challenges]] — measuring and prioritizing risk requires weighing these characteristics against each other
