---
type: concept
name: "Software Testing Pyramid"
aliases: ["Test Pyramid", "Testing Pyramid"]
description: "A testing-mix model where unit tests form a large base, functional/API tests a smaller middle layer, and manual/UI tests only a thin top layer that proves — rather than discovers — functionality."
related_to: ["[[unit-testing]]", "[[shift-left-testing]]"]
sources:
  - url: "https://www.stickyminds.com/article/shift-left-approach-software-testing"
    type: "remote-binary"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
graphify_node_ids: ["shift_left_approach_software_testing_software_testing_pyramid"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Software Testing Pyramid

> A model for how much of each test type a mature team should have: mostly [[unit-testing|unit tests]] at the base, a smaller layer of functional/API tests, and just enough manual/UI tests at the top to confirm things work.

## Description

The testing pyramid is the structural backbone of an effective [[shift-left-testing|shift-left testing]] strategy. Developers create unit tests that cover the code reasonably well; functional and API testers do as much as they can at that layer; and late-cycle manual/UI tests exist only to prove functionality is working — not to serve as the primary bug-finding mechanism. This inverts the common anti-pattern of relying mainly on late, expensive, manual system testing to catch defects.

## Key Characteristics

- Large base of cheap, fast [[unit-testing|unit tests]].
- Middle layer of functional/API tests.
- Thin top layer of manual/UI tests used to confirm functionality, not to discover bugs.

## Where it Applies

- [[shift-left-testing]] — the pyramid is the test-mix foundation that makes shifting left practical

## Related Concepts

- [[unit-testing]] — the pyramid's base layer
