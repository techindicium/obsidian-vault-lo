---
type: concept
name: "SAMM Verification"
aliases: ["OWASP SAMM Verification Function"]
description: "OWASP SAMM's business function for confirming security posture through review and testing: architecture assessment, requirements-driven testing, and security testing."
related_to: ["[[samm-standard]]", "[[samm-implementation]]", "[[samm-operations]]", "[[security-testing]]", "[[shift-left-testing]]"]
sources:
  - url: "https://owaspsamm.org/model/verification/architecture-assessment/"
    type: "remote-binary"
    synced_at: "2026-09-10"
  - url: "https://owaspsamm.org/model/verification/requirements-driven-testing/"
    type: "remote-binary"
    synced_at: "2026-09-10"
  - url: "https://owaspsamm.org/model/verification/security-testing/"
    type: "remote-binary"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# SAMM Verification

> Confirming that the application and infrastructure actually meet security and compliance requirements — [[samm-standard|SAMM]]'s review-and-testing business function.

## Practices

### Architecture Assessment
Ensures architecture adequately meets security/compliance requirements and mitigates identified threats.
- **Stream A — Architecture Validation:** M1 identify components, basic security review → M2 validate architecture security mechanisms → M3 review the components' actual effectiveness.
- **Stream B — Architecture Mitigation:** M1 ad-hoc review for unmitigated threats → M2 analyze against known threats → M3 feed results back into enterprise architecture and reference patterns.

### Requirements-driven Testing
Confirms implemented security controls operate as expected and satisfy stated requirements.
- **Stream A — Control Verification:** M1 test for security controls → M2 derive test cases from known requirements → M3 regression testing with security unit tests.
- **Stream B — Misuse/Abuse Testing:** M1 security fuzz testing → M2 abuse-case and business-logic-flaw testing → M3 denial-of-service and security stress testing.

### Security Testing
Discovers security defects via manual and tool-based testing, progressively integrated into development/deployment workflows — distinguished from Requirements-driven Testing by focusing on uncovering unknown technical/business-logic weaknesses rather than verifying known requirements. This is the SAMM-formalized, maturity-leveled counterpart to the vault's general [[security-testing]] concept.
- **Stream A — Scalable Baseline:** M1 automated security testing tools → M2 application-specific test automation → M3 integrated into the build/deploy process.
- **Stream B — Deep Understanding:** M1 manual testing of high-risk components → M2 manual penetration testing → M3 integrated into the development process.

## Where it Applies

- [[samm-standard]] — one of its five business functions
- [[security-testing]] — SAMM's Security Testing practice is the maturity-leveled, process-formalized version of this general concept
- [[shift-left-testing]] — Security Testing's M3 goal (integrated into build/deploy) is a direct shift-left outcome

## Related Concepts

- [[samm-implementation]] — Verification checks what Implementation produced
- [[samm-operations]] — Verification findings feed into ongoing operational security
