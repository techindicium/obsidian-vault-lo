---
type: concept
name: "Coding Standards"
aliases: ["Engineering Standards", "Code Standards"]
description: "Engineering rules and conventions, enforced through static code analysis, that reduce the volume of bugs introduced and let teams build secure-by-design software instead of testing security in afterward."
related_to: ["[[static-code-analysis]]", "[[gdpr]]", "[[security-testing]]", "[[shift-left-testing]]"]
sources:
  - url: "https://www.stickyminds.com/article/shift-left-approach-software-testing"
    type: "remote-binary"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
graphify_node_ids: ["shift_left_approach_software_testing_coding_standards"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Coding Standards

> The software equivalent of engineering standards: rules enforced through static code analysis that reduce bug volume and help build security into code from the start.

## Description

Coding standards are key to getting the most value out of a [[shift-left-testing|shift-left]] initiative — they reduce the volume of bugs introduced (not just find them earlier) via [[static-code-analysis|static code analysis]]. They are especially important for software security: the goal is to build security into the code from the beginning ("secure by design") rather than testing it in after the fact. This is both good practice and, in regulated contexts, a requirement — e.g. under [[gdpr|GDPR]].

## Key Characteristics

- Enforced mechanically through [[static-code-analysis|static code analysis]], not manual review alone.
- Reduces the number of bugs introduced, complementing the goal of finding bugs earlier.
- Central to "secure by design": hardening software by construction rather than through later [[security-testing|security testing]] alone.

## Where it Applies

- [[static-code-analysis]] — the enforcement mechanism for coding standards
- [[gdpr]] — a regulatory driver requiring secure-by-design coding practices
- [[security-testing]] — coding standards reduce what security testing needs to catch after the fact

## Related Concepts

- [[static-code-analysis]]
- [[shift-left-testing]] — coding standards are one of the two main levers of shifting left
