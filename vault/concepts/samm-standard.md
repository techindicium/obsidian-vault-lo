---
type: concept
name: "OWASP SAMM (Software Assurance Maturity Model)"
aliases: ["SAMM", "OWASP SAMM v2"]
description: "OWASP's community-driven, technology-agnostic maturity model for measuring and improving an organization's software security posture, organized into 5 business functions, 15 practices, 2 streams per practice, and 3 maturity levels."
related_to: ["[[samm-governance]]", "[[samm-design]]", "[[samm-implementation]]", "[[samm-verification]]", "[[samm-operations]]", "[[aisvs-standard]]", "[[shift-left-testing]]"]
sources:
  - url: "https://owaspsamm.org/"
    type: "remote-binary"
    synced_at: "2026-09-10"
  - url: "https://owaspsamm.org/model/"
    type: "remote-binary"
    synced_at: "2026-09-10"
  - url: "https://owaspsamm.org/about/"
    type: "remote-binary"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# OWASP SAMM (Software Assurance Maturity Model)

> An effective and measurable way for any organization to analyze and improve their software security posture — technology and process agnostic, adaptable to any organization's size or development style.

## Description

SAMM is built on three design principles: **measurable** (defined maturity levels per practice), **actionable** (clear improvement pathways from where an organization is to where it wants to be), and **versatile** (technology/process agnostic). It deliberately does not insist every organization reach the maximum maturity level in every category — the model supports assessing current posture, setting a realistic target maturity, and building a prioritized roadmap to close the gap. Community-driven, maintained by OWASP volunteers, published under CC BY-SA 4.0.

## Model Structure

- **5 business functions**: [[samm-governance|Governance]], [[samm-design|Design]], [[samm-implementation|Implementation]], [[samm-verification|Verification]], [[samm-operations|Operations]]
- **15 practices** — 3 per business function
- **2 streams per practice** — two independent improvement paths within the same practice (e.g. one stream about process/culture, another about the technical mechanism)
- **3 maturity levels per stream** — each level has a successively more sophisticated objective and stricter success metrics than the one before; lower levels are easier to execute and require less formalization

## Where it Applies

- [[samm-governance]], [[samm-design]], [[samm-implementation]], [[samm-verification]], [[samm-operations]] — its five business functions
- [[aisvs-standard]] — a sibling OWASP standard; SAMM measures organizational SDLC maturity broadly, AISVS verifies AI-specific security requirements — complementary, not overlapping
- [[shift-left-testing]] — SAMM's Verification function (particularly Security Testing and Architecture Assessment) operationalizes shift-left practice into a measurable maturity model

## Related Concepts

- [[samm-verification]] — includes a "Security Testing" practice related to, but more formally leveled than, the vault's general [[security-testing]] concept
