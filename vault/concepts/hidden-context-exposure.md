---
type: concept
name: "Hidden Context Exposure"
aliases: ["LLM08:2026"]
description: "A new-for-2026 risk where hidden context an LLM relies on internally — system prompts, tool definitions, retrieved-but-unshown content, chain-of-thought — leaks to a user or attacker, or amplifies other risks by giving an attacker more to work with."
related_to: ["[[genai-top10-standard]]", "[[prompt-injection]]", "[[sensitive-information-disclosure]]", "[[excessive-agency]]", "[[improper-output-handling]]"]
sources:
  - url: "https://github.com/GenAI-Security-Project/GenAI-LLM-Top10"
    type: "github-repo"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
graphify_node_ids: ["genai_top10_llm08_hidden_context_exposure"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Hidden Context Exposure

> A new 2026 entry: hidden context an LLM relies on internally — system prompts, tool/function definitions, unshown retrieved content, or chain-of-thought reasoning — leaking to a user or attacker.

## Description

This risk didn't appear in the 2025 list — it was added as agentic and RAG-based systems made "hidden" context (content the model sees but isn't meant to reveal) a bigger and more consequential attack surface. The 2026 text explicitly calls out that hidden context exposure amplifies four other risks: it can leak the specifics an attacker needs for [[prompt-injection|prompt injection]], directly constitute [[sensitive-information-disclosure|sensitive information disclosure]], reveal tool definitions an attacker can exploit for [[excessive-agency|excessive agency]], or surface unvalidated content that becomes an [[improper-output-handling|improper output handling]] problem downstream.

## Key Characteristics

- New in the 2026 edition — not present in 2025's list.
- A cross-cutting amplifier: its main significance is making four other risks easier to exploit, not just a standalone leak.
- Covers system prompts, tool/function schemas, retrieved-but-unshown content, and chain-of-thought reasoning as distinct hidden-context categories.

## Where it Applies

- [[genai-top10-standard]] — ranked #8 in the 2026 OWASP LLM Top 10 (new entry)

## Related Concepts

- [[prompt-injection]] — hidden context exposure can supply an attacker what they need to craft an injection
- [[sensitive-information-disclosure]] — hidden context leakage is itself a disclosure
- [[excessive-agency]] — exposed tool definitions/schemas aid excessive-agency exploitation
- [[improper-output-handling]] — unvalidated hidden content reaching output is a handling failure
