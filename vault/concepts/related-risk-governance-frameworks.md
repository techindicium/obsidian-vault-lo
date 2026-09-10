---
type: concept
name: "Related Risk & Governance Frameworks Cited by the AI RMF"
aliases: ["NIST AI RMF Playbook", "NIST Cybersecurity Framework", "NIST Privacy Framework", "ISO 31000"]
description: "A reference index of the external standards and frameworks the NIST AI RMF cites as related or complementary — NIST's own Cybersecurity, Privacy, and Risk Management Frameworks, the Secure Software Development Framework, ISO 31000 and ISO/IEC TS 5723, the OECD AI classification framework, and the AI RMF's own companion Playbook."
related_to: ["[[nist-ai-risk-management-framework]]"]
sources:
  - url: "https://www.nist.gov/itl/ai-risk-management-framework"
    type: "remote-binary"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
graphify_node_ids: ["nist_ai_100_1_ai_rmf_playbook", "nist_ai_100_1_nist_cybersecurity_framework", "nist_ai_100_1_nist_privacy_framework", "nist_ai_100_1_nist_risk_management_framework", "nist_ai_100_1_secure_software_development_framework", "nist_ai_100_1_nist_sp_1270", "nist_ai_100_1_iso_31000", "nist_ai_100_1_iso_iec_ts_5723", "nist_ai_100_1_oecd_classification_framework"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Related Risk & Governance Frameworks Cited by the AI RMF

> The external standards and companion resources the [[nist-ai-risk-management-framework|NIST AI RMF]] cites as related or complementary, rather than duplicating.

## Description

The AI RMF is designed to interoperate with — not replace — an organization's existing risk and security practice. Each entry below is captured here as a lightweight reference stub; if a future source provides substantial standalone content about any one of these, it should be promoted to its own concept entity rather than expanded in place here.

## Frameworks Cited

- **NIST AI RMF Playbook** — a companion resource providing suggested actions, references, and documentation guidance for implementing the AI RMF Core functions in practice.
- **NIST Cybersecurity Framework (CSF)** — NIST's widely adopted framework for managing cybersecurity risk (Identify, Protect, Detect, Respond, Recover), referenced as a model the AI RMF's structure draws on.
- **NIST Privacy Framework** — NIST's companion framework for managing privacy risk in system design and operation, relevant to the AI RMF's Privacy-Enhanced trustworthiness characteristic.
- **NIST Risk Management Framework (RMF)** — NIST's general-purpose framework (SP 800-37) for managing information-system security and privacy risk, which the AI RMF adapts concepts from for the AI-specific context.
- **Secure Software Development Framework (SSDF, NIST SP 800-218)** — practices for building security into the software development lifecycle, relevant background for AI systems as software artifacts.
- **NIST SP 1270** — "Towards a Standard for Identifying and Managing Bias in Artificial Intelligence," cited as foundational work behind the Fair — with Harmful Bias Managed trustworthiness characteristic.
- **ISO 31000:2018** — the international standard for general risk management principles and guidelines, which the AI RMF's risk-framing approach is consistent with.
- **ISO/IEC TS 5723:2022** — a trustworthiness vocabulary standard, cited as a shared-terminology reference for the AI RMF's trustworthiness characteristics.
- **OECD Framework for the Classification of AI Systems** — an international reference classification for AI systems that informs how AI Actor roles and system contexts are described.

## Where it Applies

- [[nist-ai-risk-management-framework]] — these are the frameworks the AI RMF explicitly positions itself alongside

## Related Concepts

- [[trustworthy-ai-characteristics]] — several characteristics trace directly to specific cited standards (Fair→NIST SP 1270, Privacy-Enhanced→NIST Privacy Framework)
