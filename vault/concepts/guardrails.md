---
type: concept
name: "Guardrails"
aliases: ["AI Guardrails"]
description: "Enforcement mechanisms — input filters, output filters, policy checks — placed around an AI model to keep its behavior within intended, safe bounds."
related_to: ["[[aisvs-standard]]", "[[aisvs-core-categories]]", "[[prompt-injection]]", "[[jailbreak]]", "[[hallucination]]"]
sources:
  - url: "https://github.com/OWASP/AISVS"
    type: "github-repo"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
graphify_node_ids: ["aisvs_guardrails"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Guardrails

> Mechanisms placed around a model — filtering its inputs, its outputs, or both against policy — to keep its behavior within intended, safe bounds regardless of what it's asked to do internally.

## Description

Guardrails sit outside the model itself (as opposed to safety alignment baked into the model's own training) and act as an enforcement layer: rejecting or rewriting disallowed inputs, filtering outputs that violate policy, or blocking tool calls that fall outside an allowed set. They are the AISVS's primary recommended defense against both [[prompt-injection|prompt injection]] and [[jailbreak|jailbreak]] attempts, and can also catch [[hallucination|hallucinated]] output before it reaches a user or a downstream system.

## Key Characteristics

- External to the model — a separate enforcement layer, not reliant solely on the model's own training.
- Can operate on input (pre-filtering), output (post-filtering), or both.
- A single guardrail layer commonly defends against multiple risk types at once (injection, jailbreak, unsafe tool calls, policy-violating output).

## Where it Applies

- [[aisvs-core-categories]] — referenced across Input Validation (C02), Model Behavior (C07), and Monitoring/Logging (C12) as the primary enforcement mechanism

## Related Concepts

- [[prompt-injection]] — guardrails are a primary defense against this
- [[jailbreak]] — guardrails are a primary defense against this
- [[hallucination]] — output-side guardrails can catch some hallucinated content before delivery
