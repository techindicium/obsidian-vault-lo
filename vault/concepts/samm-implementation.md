---
type: concept
name: "SAMM Implementation"
aliases: ["OWASP SAMM Implementation Function"]
description: "OWASP SAMM's business function for building and shipping software securely: secure build, secure deployment, and defect management."
related_to: ["[[samm-standard]]", "[[samm-design]]", "[[samm-verification]]", "[[shift-left-testing]]", "[[static-code-analysis]]"]
sources:
  - url: "https://owaspsamm.org/model/implementation/secure-build/"
    type: "remote-binary"
    synced_at: "2026-09-10"
  - url: "https://owaspsamm.org/model/implementation/secure-deployment/"
    type: "remote-binary"
    synced_at: "2026-09-10"
  - url: "https://owaspsamm.org/model/implementation/defect-management/"
    type: "remote-binary"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# SAMM Implementation

> Building software in a standardized, repeatable, secure manner and shipping it safely — [[samm-standard|SAMM]]'s build-and-ship business function.

## Practices

### Secure Build
Builds software in a standardized, repeatable manner using secure components, including 3rd-party dependencies.
- **Stream A — Build Process:** M1 a formal, consistent, repeatable build definition → M2 automated, secured pipeline with security checks → M3 mandatory security checks that fail the build on non-compliance.
- **Stream B — Software Dependencies:** M1 create a Bill of Materials, analyze opportunistically → M2 evaluate dependencies, react to risk in time → M3 analyze dependencies for security issues as rigorously as your own code.

### Secure Deployment
Documents and progressively automates deployment with built-in security verification.
- **Stream A — Deployment Process:** M1 formalize the process, secure tooling → M2 automate all stages with security verification tests → M3 automatically verify the integrity of all deployed software.
- **Stream B — Secret Management:** M1 basic access-limiting protections on production secrets → M2 inject secrets dynamically from hardened storage, audit human access → M3 regular rotation and lifecycle management of secrets.

### Defect Management
Tracks security defects and uses that data to reduce future defects, not just fix present ones.
- **Stream A — Defect Tracking:** M1 structured tracking, informed decisions → M2 consistent org-wide severity rating with SLAs → M3 enforced SLAs integrated with other tooling.
- **Stream B — Metrics and Feedback:** M1 review past defects for quick wins from basic metrics → M2 standardized metrics used for prioritization → M3 continuously improved metrics correlated with other sources.

## Where it Applies

- [[samm-standard]] — one of its five business functions
- [[shift-left-testing]] — Secure Build's automated, mandatory-check pipeline is a direct application of shift-left principles to the build stage
- [[static-code-analysis]] — the mechanism behind Secure Build's automated security checks

## Related Concepts

- [[samm-design]] — Implementation builds what Design specified
- [[samm-verification]] — Verification checks whether what Implementation built actually meets requirements
