---
type: concept
name: "SAMM Governance"
aliases: ["OWASP SAMM Governance Function"]
description: "OWASP SAMM's business function for how an organization manages overall software security activities at a cross-project level: strategy/metrics, policy/compliance, and education/guidance."
related_to: ["[[samm-standard]]", "[[samm-design]]", "[[coding-standards]]"]
sources:
  - url: "https://owaspsamm.org/model/governance/"
    type: "remote-binary"
    synced_at: "2026-09-10"
  - url: "https://owaspsamm.org/model/governance/strategy-and-metrics/"
    type: "remote-binary"
    synced_at: "2026-09-10"
  - url: "https://owaspsamm.org/model/governance/policy-and-compliance/"
    type: "remote-binary"
    synced_at: "2026-09-10"
  - url: "https://owaspsamm.org/model/governance/education-and-guidance/"
    type: "remote-binary"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# SAMM Governance

> "Governance focuses on the processes and activities related to how an organization manages overall software development activities" — the cross-project, organization-level layer of [[samm-standard|SAMM]].

## Practices

### Strategy & Metrics
Builds an efficient, prioritized plan for software security so effort isn't unaligned or counterproductive, and measures its own effectiveness.
- **Stream A — Create and Promote:** M1 identify risk-tolerance drivers → M2 publish a unified AppSec strategy → M3 align the program to organizational growth.
- **Stream B — Measure and Improve:** M1 define effectiveness/efficiency metrics → M2 set targets/KPIs → M3 influence strategy from metrics and org needs.

### Policy & Compliance
Understands and meets external legal/regulatory requirements while driving internal security standards aligned with the business.
- **Stream A — Policy and Standards:** M1 determine a security baseline → M2 develop requirements applicable to all applications → M3 measure/report each application's adherence.
- **Stream B — Compliance Management:** M1 identify 3rd-party compliance drivers, map to existing policy → M2 publish compliance-specific requirements/test guidance → M3 measure/report compliance per application.

### Education & Guidance
Builds staff capability in secure development, from passive resources to in-house training programs.
- **Stream A — Training and Awareness:** M1 security awareness training for all → M2 technology/role-specific guidance → M3 standardized in-house secure-development guidance.
- **Stream B — Organization and Culture:** M1 a Security Champion per team → M2 a secure-software center of excellence → M3 an org-wide secure-software community.

## Where it Applies

- [[samm-standard]] — one of its five business functions
- [[coding-standards]] — Policy & Compliance's org-wide security baseline is the SAMM-formalized analogue of coding standards

## Related Concepts

- [[samm-design]]
