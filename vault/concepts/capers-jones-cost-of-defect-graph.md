---
type: concept
name: "Capers Jones Cost-of-Defect Graph"
aliases: ["Cost of Defect Curve", "Cost-of-Defect Model"]
description: "A widely cited model, attributed to Capers Jones, showing that the cost to fix a software defect increases dramatically the later it is found in the development lifecycle."
related_to: ["[[shift-left-testing]]", "[[static-code-analysis]]", "[[coding-standards]]"]
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

The graph, attributed to researcher Capers Jones, overlays three curves across five SDLC phases — Coding, Unit Test, Functional Test, System Test, and Release: when defects are *introduced* (a "% defect injection" curve peaking during coding), when they are *found* (a "% defects found" curve, roughly inverse-shaped, peaking during unit/functional test), and the *cost to repair* each defect, which rises steeply phase over phase — from 1X at coding to a striking **640X at release**. This model is the empirical foundation for the [[shift-left-testing|shift-left testing]] strategy.

## Key Characteristics

- Three overlaid curves across five SDLC phases: % defect injection, % defects found, and cost-to-repair-defect.
- **Cost-to-repair-defect multiplier by phase:** Coding = 1X, Unit Test = 4X, Functional Test = 10X, System Test = 40X, Release = **640X**.
- Defect injection peaks at 85% during Coding — most bugs are introduced right at the start, even though they are rarely caught there.
- Cost escalation drivers: harder root-cause tracing in complex late-cycle test cases, harder reproduction once dependent systems (databases, third-party APIs) are involved, and larger blast radius when the fix is systemic (wrong framework, unscalable design, unsecurable code).

## How Shift-Left Bends the Curve

The source article overlays a second version of this same graph to show the effect of applying [[shift-left-testing|shift-left testing]] practices:

- The **% defect injection peak is reduced** — fewer bugs introduced in the first place, the direct effect of upstream practices like [[static-code-analysis|static code analysis]] and [[coding-standards|coding standards]].
- The **% defects found curve shifts left** — the same defects get caught earlier, during Unit Test/Functional Test, instead of at System Test or Release, where the cost is 40x–640x higher.

This is the two-sided mechanism behind the "reduce, don't just find" framing of shift-left: fewer defects are introduced, and the ones that are introduced get caught before they reach the expensive tail of the curve.

## Where it Applies

- [[shift-left-testing]] — the primary strategy motivated directly by this cost curve

## Related Concepts

- [[shift-left-testing]]

## Source

Chart originally published in: Jones, Capers. *Applied Software Measurement: Global Analysis of Productivity and Quality.* Reproduced in the ingested article (see `sources` in frontmatter).
