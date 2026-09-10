---
type: concept
name: "SAMM Design"
aliases: ["OWASP SAMM Design Function"]
description: "OWASP SAMM's business function for building security into a project before implementation: threat assessment, security requirements, and secure architecture."
related_to: ["[[samm-standard]]", "[[samm-governance]]", "[[samm-implementation]]", "[[coding-standards]]"]
sources:
  - url: "https://owaspsamm.org/model/design/threat-assessment/"
    type: "remote-binary"
    synced_at: "2026-09-10"
  - url: "https://owaspsamm.org/model/design/security-requirements/"
    type: "remote-binary"
    synced_at: "2026-09-10"
  - url: "https://owaspsamm.org/model/design/secure-architecture/"
    type: "remote-binary"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# SAMM Design

> Building security consideration into a project's requirements and architecture before code is written — [[samm-standard|SAMM]]'s design-time business function.

## Practices

### Threat Assessment
Identifies and understands project-level risks based on the software's functionality and runtime environment.
- **Stream A — Application Risk Profile:** M1 basic per-app risk assessment → M2 centralized org-wide risk profile inventory → M3 periodic review for accuracy.
- **Stream B — Threat Modeling:** M1 best-effort brainstorming with simple checklists → M2 standardized training/process/tools at scale → M3 continuous optimization and automation.

### Security Requirements
Considers security explicitly during the requirements process, with increasing granularity and mandate.
- **Stream A — Software Requirements:** M1 map high-level AppSec objectives to functional requirements → M2 structured requirements used by dev teams → M3 a requirements framework for product teams.
- **Stream B — Supplier Security:** M1 evaluate suppliers against org security requirements → M2 build security into supplier agreements → M3 ensure proper coverage via clear objectives for external suppliers.

### Secure Architecture
Inserts proactive security guidance into the software design process.
- **Stream A — Architecture Design:** M1 train teams on basic security design principles → M2 establish common design patterns/security solutions → M3 continuously evaluated reference architectures.
- **Stream B — Technology Management:** M1 elicit technologies/frameworks/integrations to identify risk → M2 standardize technologies across applications → M3 impose standard technologies org-wide.

## Where it Applies

- [[samm-standard]] — one of its five business functions
- [[coding-standards]] — Secure Architecture's design patterns and Security Requirements formalize what coding standards enforce at the code level

## Related Concepts

- [[samm-governance]]
- [[samm-implementation]] — Design's requirements and architecture feed directly into what Implementation builds
