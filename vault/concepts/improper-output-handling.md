---
type: concept
name: "Improper Output Handling"
aliases: ["LLM10:2026"]
description: "A risk where an LLM's output is passed downstream (to a browser, a shell, a database query, another system) without the same validation/sanitization that would be applied to any other untrusted input."
related_to: ["[[genai-top10-standard]]", "[[misinformation]]", "[[prompt-injection]]", "[[excessive-agency]]"]
sources:
  - url: "https://github.com/GenAI-Security-Project/GenAI-LLM-Top10"
    type: "github-repo"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
graphify_node_ids: ["genai_top10_llm10_improper_output_handling"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Improper Output Handling

> Passing an LLM's output downstream — into a browser (XSS), a shell command, a database query, or another system — without the validation/sanitization that untrusted input normally requires, on the mistaken assumption that model output is inherently safe.

## Description

This is the classic "never trust user input" principle applied to LLM output specifically: an LLM's response should be treated as untrusted data by anything that consumes it downstream, the same way user-supplied input is. Failing to do so turns [[misinformation|misinformation]] or attacker-influenced output (via [[prompt-injection|prompt injection]] or an over-permissioned [[excessive-agency|agent]]) into concrete downstream vulnerabilities — injection attacks, unauthorized commands, or corrupted data — rather than just a bad answer.

## Key Characteristics

- The failure mode: model output is trusted as safe by default, when it should be validated like any other untrusted input.
- Turns upstream risks (misinformation, prompt injection, excessive agency) into concrete downstream vulnerabilities when output reaches a browser, shell, or database unsanitized.
- Mitigated with standard output-encoding/sanitization practices, applied consistently to LLM output.

## Where it Applies

- [[genai-top10-standard]] — ranked #10 in the 2026 OWASP LLM Top 10

## Related Concepts

- [[misinformation]] — unhandled output is how misinformation propagates downstream
- [[prompt-injection]] — attacker-influenced output reaching an unsanitized sink is a common attack chain
