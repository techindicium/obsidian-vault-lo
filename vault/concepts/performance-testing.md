---
type: concept
name: "Performance Testing"
aliases: ["Performance Test", "Load Testing"]
description: "Testing system behavior under load and adverse what-if conditions (slow dependencies, error injection), made possible earlier in the lifecycle via service virtualization."
related_to: ["[[service-virtualization]]", "[[security-testing]]"]
sources:
  - url: "https://www.stickyminds.com/article/shift-left-approach-software-testing"
    type: "remote-binary"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
graphify_node_ids: ["shift_left_approach_software_testing_performance_testing"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Performance Testing

> Testing how a system behaves under load and adverse conditions — sped up and made possible earlier by simulating dependencies instead of waiting for a full production-like lab.

## Description

[[service-virtualization|Service virtualization]] lets performance testing start before everything is ready and without a complete lab of every system component. It also enables what-if scenarios that are hard to reproduce in the real world — e.g., a fast app server paired with a slow database, or a dependency that suddenly starts returning 500 errors — letting teams push the system's limits as early and as hard as they want.

## Key Characteristics

- Runs before the full system/lab exists, via [[service-virtualization|service virtualization]].
- Supports deliberate what-if fault injection (slow dependencies, error responses) difficult to stage against real systems.
- Shares its enabling mechanism with [[security-testing|security testing]] — both push adverse-condition testing left via virtualized dependencies.

## Where it Applies

- [[service-virtualization]] — the mechanism that enables performance testing before the full system is available

## Related Concepts

- [[security-testing]] — sibling practice enabled by the same virtualization mechanism
