---
type: concept
name: "OWASP AI Security Verification Standard (AISVS)"
aliases: ["AISVS", "OWASP AISVS"]
description: "A community-driven OWASP catalogue of testable, verifiable security requirements for AI-enabled systems, modeled on the OWASP ASVS, organized into 12 control categories rated at three verification levels (L1/L2/L3)."
related_to: ["[[aisvs-core-categories]]", "[[ai-security-controls-inventory]]", "[[ai-for-code-generation-security]]", "[[owasp-asvs]]", "[[nist-ai-risk-management-framework]]", "[[iso-42001]]", "[[mitre-atlas]]"]
sources:
  - url: "https://github.com/OWASP/AISVS"
    type: "github-repo"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
graphify_node_ids: ["aisvs_document", "aisvs_scope", "aisvs_verification_levels", "aisvs_asvs_alignment", "aisvs_glossary"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# OWASP AI Security Verification Standard (AISVS)

> An open catalogue of testable security requirements for AI-enabled systems, giving developers, architects, security engineers, and auditors a structured way to design, build, test, and verify AI application security across its lifecycle.

## Description

AISVS v1.0 (released June 24, 2026) is modeled directly on the [[owasp-asvs|OWASP Application Security Verification Standard]] and follows the same philosophy: every requirement should be verifiable, testable, and implementable — not an abstract best practice. It is deliberately scoped to AI-specific security concerns (narrow scope) rather than duplicating general application security, which remains the ASVS's job; the two standards are meant to be applied together. AISVS explicitly cross-references other governance frameworks it complements rather than replaces, including the [[nist-ai-risk-management-framework|NIST AI RMF]] and [[iso-42001|ISO/IEC 42001]], and cites [[mitre-atlas|MITRE ATLAS]] as a source for adversarial-ML threat patterns behind several requirements.

## AISVS Verification Levels (L1/L2/L3)

Like ASVS, every requirement is assigned a level indicating depth of assurance:
- **L1** — baseline requirements applicable to essentially all AI-enabled systems.
- **L2** — the level most production systems handling sensitive data or consequential decisions should target.
- **L3** — the highest assurance level, for systems where AI failure has severe safety, financial, or rights-impacting consequences.

## Scope

AISVS deliberately keeps a narrow, AI-specific scope: it does not re-litigate general web/application security (that's the ASVS's domain) but instead targets the security properties unique to AI-enabled systems — training data integrity, model lifecycle integrity, prompt/input handling, agentic tool use, and the like — organized into [[aisvs-core-categories|12 core control categories]].

## Where it Applies

- [[aisvs-core-categories]] — the 12 control categories this standard is organized around
- [[ai-security-controls-inventory]] — Appendix B's cross-reference table mapping controls to categories/threats
- [[ai-for-code-generation-security]] — Appendix C's guidance on a specific high-risk use case (AI-assisted coding)

## Related Concepts

- [[owasp-asvs]] — the parent standard AISVS is modeled on and meant to be applied alongside
- [[nist-ai-risk-management-framework]] — a complementary governance framework AISVS cites
- [[iso-42001]] — a complementary AI management-system standard AISVS cites
- [[mitre-atlas]] — the adversarial-ML threat knowledge base behind several AISVS requirements
