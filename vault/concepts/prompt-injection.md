---
type: concept
name: "Prompt Injection"
aliases: ["Indirect Prompt Injection"]
description: "An attack that manipulates an LLM's behavior by embedding malicious instructions in its input — either directly in user input, or indirectly via content the model retrieves or is exposed to (a document, webpage, tool output)."
related_to: ["[[aisvs-standard]]", "[[aisvs-core-categories]]", "[[jailbreak]]", "[[guardrails]]", "[[trust-boundary]]", "[[genai-top10-standard]]", "[[hidden-context-exposure]]"]
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
graphify_node_ids: ["aisvs_prompt_injection", "aisvs_indirect_prompt_injection", "genai_top10_llm01_prompt_injection"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Prompt Injection

> Manipulating an LLM's behavior by embedding malicious or unintended instructions inside its input, causing it to ignore its original instructions or take unintended action.

## Description

**Direct prompt injection** happens when an attacker crafts adversarial input directly in the conversation with the model. **Indirect prompt injection** is the more insidious variant: the malicious instructions are embedded in content the model consumes as data — a webpage it browses, a document it summarizes, a tool response it receives — rather than in the user's own message. Because the model can't always distinguish "instructions from my operator" from "text I'm supposed to just process," indirect injection is especially dangerous for agentic systems that call tools and consume external content on the user's behalf, crossing multiple [[trust-boundary|trust boundaries]] where injected content can hide.

## Key Characteristics

- Direct variant: attacker-controlled input in the conversation itself.
- Indirect variant: attacker-controlled content in something the model retrieves or is fed (documents, web pages, tool/API responses) — the injection point is not the conversation the user sees.
- Distinct from but related to [[jailbreak|jailbreaking]]: injection smuggles instructions in via content; jailbreaking manipulates the model's own safety behavior directly.
- Mitigated by input/output validation ([[aisvs-core-categories|AISVS C02]]), [[guardrails|guardrails]], and treating all retrieved/tool content as untrusted data rather than instructions.

## Where it Applies

- [[aisvs-core-categories]] — Input Validation (C02) and Monitoring/Logging (C12) categories address detecting and mitigating prompt injection
- [[trust-boundary]] — indirect injection specifically exploits content crossing a trust boundary without re-validation

## Ranking (OWASP GenAI LLM Top 10 2026)

Ranked **#1** in the [[genai-top10-standard|OWASP Top 10 for LLM Applications and Generative AI (2026)]] — the highest-ranked risk in the evidence-weighted 2026 methodology. The 2026 list notes explicit overlap with [[excessive-agency|Excessive Agency]] (an injected instruction is far more dangerous when the agent already holds broad permissions) and with [[ai-supply-chain-risk|Supply Chain]] (shared signing/provenance mitigations, different root causes). [[hidden-context-exposure|Hidden Context Exposure]] (a new 2026 risk) can supply an attacker the specifics needed to craft an effective injection.

## Related Concepts

- [[jailbreak]] — a related but distinct manipulation technique targeting the model's safety behavior directly
- [[guardrails]] — a primary defensive mechanism against injection
- [[genai-top10-standard]] — ranked #1 in the 2026 OWASP LLM Top 10
