---
type: concept
name: "Jailbreak"
aliases: ["LLM Jailbreaking"]
description: "A technique that manipulates an AI model into bypassing its own safety training or usage policies, causing it to produce output it was designed to refuse."
related_to: ["[[aisvs-standard]]", "[[aisvs-core-categories]]", "[[prompt-injection]]", "[[guardrails]]", "[[adversarial-example]]"]
sources:
  - url: "https://github.com/OWASP/AISVS"
    type: "github-repo"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
graphify_node_ids: ["aisvs_jailbreak"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Jailbreak

> Manipulating a model into ignoring its own safety training or usage policy, so it produces output it was designed to refuse.

## Description

Jailbreaks target the model's own alignment/safety behavior directly — through role-play framing, hypothetical scenarios, encoding tricks, or multi-turn manipulation — rather than smuggling instructions in via external content, which is what distinguishes it from [[prompt-injection|prompt injection]]. A model can be jailbroken through a direct conversation with no external content involved at all. Defenses include [[guardrails|guardrails]], adversarial training, and runtime detection of known jailbreak patterns.

## Key Characteristics

- Targets the model's own safety/alignment behavior, not just its instruction-following.
- Can occur purely through conversational manipulation, without any external/indirect content.
- Runtime detection ([[aisvs-core-categories|AISVS C12]]) and pre-deployment hardening ([[aisvs-core-categories|AISVS C11]]) are the two AISVS-recognized mitigation stages.

## Where it Applies

- [[aisvs-core-categories]] — Adversarial Robustness (C11) and Monitoring/Logging (C12) both address jailbreak resistance and detection

## Related Concepts

- [[prompt-injection]] — a related but distinct manipulation technique that smuggles instructions via content rather than direct conversation
- [[guardrails]] — a primary defensive mechanism against jailbreaks
- [[adversarial-example]] — a broader category of deliberately crafted input jailbreaks are one instance of
