---
type: concept
name: "Model Extraction"
aliases: ["Model Stealing"]
description: "An attack that reconstructs or steals a proprietary model's parameters, behavior, or training data by systematically querying it and analyzing the responses."
related_to: ["[[aisvs-standard]]", "[[aisvs-core-categories]]", "[[data-poisoning]]", "[[adversarial-example]]"]
sources:
  - url: "https://github.com/OWASP/AISVS"
    type: "github-repo"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
graphify_node_ids: ["aisvs_model_extraction"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Model Extraction

> Reconstructing or stealing a model's behavior, parameters, or the training data it was built on, by systematically querying it and analyzing the pattern of responses — without ever accessing the model's internals directly.

## Description

Model extraction is a confidentiality and IP-theft risk distinct from [[data-poisoning|data poisoning]] (which corrupts a model) or [[jailbreak|jailbreaking]] (which manipulates a model's output policy) — it targets stealing the model itself, or the sensitive data it was trained on, through black-box interaction alone. Rate limiting, output obfuscation, and monitoring for extraction-pattern query behavior are the AISVS-recognized mitigations, sitting primarily under Access Control/Identity and Monitoring/Logging.

## Key Characteristics

- A black-box attack — the attacker never needs direct access to model weights or training pipeline.
- Targets confidentiality (of the model or its training data), not availability or integrity directly.
- Distinct from [[data-poisoning|data poisoning]] (which corrupts what a model knows) — extraction steals what it knows.

## Where it Applies

- [[aisvs-core-categories]] — Access Control & Identity (C05) and Monitoring/Logging (C12) address rate-limiting and detecting extraction-pattern query behavior

## Related Concepts

- [[data-poisoning]] — a related but distinct attack that corrupts rather than steals model knowledge
- [[adversarial-example]] — extraction attacks often use carefully crafted queries similar in spirit to adversarial examples
