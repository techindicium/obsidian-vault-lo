---
type: concept
name: "Service Virtualization"
aliases: ["Service Virtualisation"]
description: "Simulating dependent systems (mainframes, third-party services, not-yet-ready components) so functional, performance, and security testing can run earlier and without a full test lab."
related_to: ["[[continuous-testing]]", "[[performance-testing]]", "[[security-testing]]", "[[shift-left-testing]]"]
sources:
  - url: "https://www.stickyminds.com/article/shift-left-approach-software-testing"
    type: "remote-binary"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
graphify_node_ids: ["shift_left_approach_software_testing_service_virtualization"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Service Virtualization

> Simulating dependent systems that have limited availability — mainframes, third-party services, or components that just aren't ready yet — so testing can run without the full system in place.

## Description

Service virtualization is the enabling mechanism that lets [[shift-left-testing|shift-left testing]] extend past unit tests into functional, performance, and security testing, all the way to the developer's desktop. By simulating dependencies, teams can run [[continuous-testing|continuous testing]] without needing the full system available, run what-if scenarios (e.g. a fast app server paired with a slow database), and inject failure conditions (500 errors, malformed data, flood conditions) that would be hard to reproduce against real systems.

## Key Characteristics

- Simulates systems with limited availability: mainframes, third-party APIs, not-yet-built components.
- Enables [[performance-testing|performance testing]] under adverse what-if scenarios without a full lab.
- Enables earlier, deeper [[security-testing|security testing]] by making simulated systems behave "evil" (malformed data, flood conditions, DDoS-like behavior) — going beyond what a production or lab system safely allows.

## Where it Applies

- [[continuous-testing]] — service virtualization is what makes later-stage functional tests executable continuously
- [[performance-testing]] — enables load/adverse-condition testing before the full system exists
- [[security-testing]] — enables adversarial/attack-behavior simulation earlier and more deeply

## Related Concepts

- [[shift-left-testing]] — service virtualization is the second major lever (alongside coding standards/static analysis) of a shift-left strategy
