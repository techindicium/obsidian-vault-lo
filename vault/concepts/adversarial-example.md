---
type: concept
name: "Adversarial Example"
aliases: ["Adversarial Input"]
description: "An input deliberately crafted, often with small/imperceptible perturbations, to cause an AI model to misclassify or misbehave in a way the attacker chose."
related_to: ["[[aisvs-standard]]", "[[aisvs-core-categories]]", "[[jailbreak]]", "[[model-extraction]]"]
sources:
  - url: "https://github.com/OWASP/AISVS"
    type: "github-repo"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
graphify_node_ids: ["aisvs_adversarial_example"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Adversarial Example

> Input deliberately crafted — often via small, human-imperceptible perturbations — to make an AI model produce a specific wrong or attacker-chosen output.

## Description

Adversarial examples are the broader technical category that [[jailbreak|jailbreak]] prompts and some [[model-extraction|model-extraction]] query strategies are specific instances of: all exploit a model's sensitivity to carefully chosen input to elicit behavior it wasn't designed to produce. AISVS groups defense against adversarial examples under Adversarial Robustness (C11), alongside jailbreak resistance, since the underlying hardening techniques (adversarial training, input sanitization, robustness testing) overlap heavily.

## Key Characteristics

- Exploits model sensitivity to carefully chosen — often subtle — input perturbations.
- A broader category that jailbreak prompts are one specific instance of.
- Mitigated primarily through adversarial training and robustness testing, tested under AISVS's Adversarial Robustness category.

## Where it Applies

- [[aisvs-core-categories]] — Adversarial Robustness (C11) is dedicated to hardening against adversarial examples

## Related Concepts

- [[jailbreak]] — a specific instance of adversarial-example crafting targeted at safety behavior
- [[model-extraction]] — some extraction strategies use adversarial-example-like query crafting
