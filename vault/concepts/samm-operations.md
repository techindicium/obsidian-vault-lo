---
type: concept
name: "SAMM Operations"
aliases: ["OWASP SAMM Operations Function"]
description: "OWASP SAMM's business function for maintaining security once software is running in production: incident management, environment management, and operational management."
related_to: ["[[samm-standard]]", "[[samm-verification]]"]
sources:
  - url: "https://owaspsamm.org/model/operations/incident-management/"
    type: "remote-binary"
    synced_at: "2026-09-10"
  - url: "https://owaspsamm.org/model/operations/environment-management/"
    type: "remote-binary"
    synced_at: "2026-09-10"
  - url: "https://owaspsamm.org/model/operations/operational-management/"
    type: "remote-binary"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# SAMM Operations

> Maintaining security throughout operational support once software is live — [[samm-standard|SAMM]]'s runtime business function.

## Practices

### Incident Management
Detects and handles security incidents, from best-effort to a mature, proactively managed process.
- **Stream A — Incident Detection:** M1 best-effort detection from available logs → M2 documented process emphasizing automated log evaluation → M3 proactively managed detection.
- **Stream B — Incident Response:** M1 identify roles/responsibilities → M2 formal response process with trained staff → M3 a dedicated, well-trained incident response team.

### Environment Management
Hardens and patches the runtime environment, from best-effort to an enforced, continuously improving process.
- **Stream A — Configuration Hardening:** M1 best-effort hardening from readily available info → M2 consistent hardening following established baselines → M3 active monitoring for non-conformance, handled as security defects.
- **Stream B — Patching and Updating:** M1 best-effort patching → M2 regular full-stack patching with timely customer delivery → M3 active monitoring of update status, proactive vulnerability/update intelligence.

### Operational Management
Maintains security across operational support functions — data protection and legacy/decommissioning.
- **Stream A — Data Protection:** M1 basic data-protection practices → M2 a data catalog and formal protection policy → M3 automated non-compliance detection with periodic audit.
- **Stream B — System Decommissioning / Legacy Management:** M1 decommission unused systems as identified, migrate customers individually → M2 repeatable decommissioning/migration processes → M3 proactive management of end-of-life and legacy migration roadmaps.

## Where it Applies

- [[samm-standard]] — one of its five business functions

## Related Concepts

- [[samm-verification]] — verification findings (vulnerabilities, misconfigurations) feed into what Operations must detect, patch, and respond to
