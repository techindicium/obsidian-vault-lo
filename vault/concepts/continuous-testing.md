---
type: concept
name: "Continuous Testing"
aliases: ["Continuous Test Execution"]
description: "Executing the tests created across all stages of development continuously, giving constant feedback as code changes land — made practical for later-stage functional tests via service virtualization."
related_to: ["[[service-virtualization]]", "[[shift-left-testing]]"]
sources:
  - url: "https://www.stickyminds.com/article/shift-left-approach-software-testing"
    type: "remote-binary"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
graphify_node_ids: ["shift_left_approach_software_testing_continuous_testing"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Continuous Testing

> Taking the tests created at every stage of development and running them continuously, so agile teams get constant feedback as code changes.

## Description

Continuous testing is critical for teams adopting agile development practices — it provides ongoing feedback throughout the development process rather than feedback concentrated at the end of a cycle. Unit tests are easy to run continuously on their own, but later-stage functional tests are often blocked by external system dependencies; [[service-virtualization|service virtualization]] removes that blocker by simulating those dependencies, letting continuous testing extend further left.

## Key Characteristics

- Applies to tests from every development stage, not just unit tests.
- The main obstacle for later-stage functional tests is external system dependencies — solved via [[service-virtualization|service virtualization]].
- Supports the constant-feedback loop that agile/DevOps delivery depends on.

## Where it Applies

- [[service-virtualization]] — the mechanism that unblocks continuous execution of later-stage functional tests

## Related Concepts

- [[shift-left-testing]] — continuous testing is part of the "leveraging service virtualization" lever of shift-left
