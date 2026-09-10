---
type: concept
name: "Capers Jones Cost-of-Defect Graph"
aliases: ["Cost of Defect Curve", "Cost-of-Defect Model"]
description: "A widely cited model, attributed to Capers Jones, showing that the cost to fix a software defect increases dramatically the later it is found in the development lifecycle."
related_to: ["[[shift-left-testing]]"]
sources:
  - url: "https://www.stickyminds.com/article/shift-left-approach-software-testing"
    type: "remote-binary"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
graphify_node_ids: ["shift_left_approach_software_testing_defect_cost_graph"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Capers Jones Cost-of-Defect Graph

> A model showing that most bugs are introduced during coding but are almost never found there — and that the cost to fix them escalates sharply the later they are caught.

## Description

The graph, attributed to researcher Capers Jones, overlays three curves across the SDLC phases: when defects are *introduced* (mostly during coding), when they are *found* (mostly during testing — roughly the inverse of the introduction curve), and the *cost* to fix them at each phase. The cost curve rises steeply: letting a bug slip through to system testing costs roughly forty times more than catching it during coding, and about ten times more than catching it during unit testing — with deployment-stage costs higher still. This model is the empirical foundation for the [[shift-left-testing|shift-left testing]] strategy.

## Key Characteristics

- Three overlaid curves: defect introduction, defect detection, and cost-to-fix, by SDLC phase.
- Cost-to-fix at system testing ≈ 40x the cost at coding time; ≈10x the cost at unit-testing time.
- Cost escalation drivers: harder root-cause tracing in complex late-cycle test cases, harder reproduction once dependent systems (databases, third-party APIs) are involved, and larger blast radius when the fix is systemic (wrong framework, unscalable design, unsecurable code).

## Where it Applies

- [[shift-left-testing]] — the primary strategy motivated directly by this cost curve

## Related Concepts

- [[shift-left-testing]]
