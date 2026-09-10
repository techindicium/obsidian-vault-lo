---
type: concept
name: "Static Code Analysis"
aliases: ["Static Analysis", "SAST"]
description: "Analyzing source code without executing it to detect bugs, insecure patterns, and coding-standard violations during the coding phase itself."
related_to: ["[[shift-left-testing]]", "[[coding-standards]]", "[[unit-testing]]"]
sources:
  - url: "https://www.stickyminds.com/article/shift-left-approach-software-testing"
    type: "remote-binary"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
graphify_node_ids: ["shift_left_approach_software_testing_static_code_analysis"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Static Code Analysis

> Finding bugs during the actual coding phase, before any test is run, by analyzing source code itself rather than its runtime behavior.

## Description

Static code analysis is the practice that lets teams find defects at the cheapest possible point in the SDLC: while the code is still being written. It underpins [[coding-standards|coding standards]] enforcement — helping developers avoid bad, dangerous, or insecure code — and is the furthest-left practice in a [[shift-left-testing|shift-left testing]] strategy, since it needs no running system or test infrastructure to operate.

## Key Characteristics

- Requires no test execution or environment — operates directly on source code.
- Enables detection of insecure/dangerous patterns tied to coding standards (e.g., regulatory requirements like [[gdpr|GDPR]]).
- Complements, but does not replace, [[unit-testing|unit tests]] — the two form the base of an effective [[software-testing-pyramid|testing pyramid]].

## Where it Applies

- [[shift-left-testing]] — the practice that pushes bug-finding into the coding phase
- [[coding-standards]] — static analysis is the mechanism that enforces coding standards

## Related Concepts

- [[unit-testing]] — the other foundational, developer-owned testing practice
- [[coding-standards]] — engineering rules enforced through static analysis
