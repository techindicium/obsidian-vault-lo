---
type: concept
name: "Security Testing"
aliases: ["Security Test"]
description: "Testing aimed at finding vulnerabilities and exploit paths, pushed earlier and deeper via service virtualization simulating attacker behavior."
related_to: ["[[service-virtualization]]", "[[coding-standards]]", "[[performance-testing]]", "[[samm-verification]]"]
sources:
  - url: "https://owaspsamm.org/model/verification/security-testing/"
    type: "remote-binary"
    synced_at: "2026-09-10"
  - url: "https://www.stickyminds.com/article/shift-left-approach-software-testing"
    type: "remote-binary"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
graphify_node_ids: ["shift_left_approach_software_testing_security_testing"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Security Testing

> Testing aimed at surfacing security vulnerabilities — made earlier and deeper by decoupling from physical systems via service virtualization.

## Description

Security testing benefits doubly from a shift-left strategy: [[coding-standards|coding standards]] build security in from the start ("secure by design", reducing what needs to be caught later), while [[service-virtualization|service virtualization]] lets teams simulate systems behaving maliciously — flooding with packets, sending malformed data, or running other exploits attackers commonly use — earlier in the lifecycle and more aggressively than would be safe or possible against a real test lab or production system.

## Key Characteristics

- Strengthened upstream by [[coding-standards|coding standards]] and secure-by-design practices.
- Enabled to run earlier and more aggressively via [[service-virtualization|service virtualization]] simulating attacker behavior (malformed data, flood/DDoS-like conditions).
- Complements [[performance-testing|performance testing]] — both rely on virtualized dependencies to push adverse-condition testing left.

## Where it Applies

- [[coding-standards]] — reduces the security debt security testing has to catch
- [[service-virtualization]] — the mechanism enabling earlier and deeper adversarial testing

## Related Concepts

- [[performance-testing]] — sibling practice enabled by the same service-virtualization mechanism
- [[samm-verification]] — OWASP SAMM's "Security Testing" practice formalizes this concept into a maturity-leveled process (scalable automated baseline + deep manual understanding streams)
