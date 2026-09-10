---
type: concept
name: "NIST AI Risk Management Framework (AI RMF 1.0)"
aliases: ["NIST AI RMF", "AI RMF 1.0", "NIST AI 100-1"]
description: "A voluntary, non-prescriptive, rights-preserving US framework (NIST AI 100-1, Jan 2023) that helps organizations manage risks and build trustworthy AI systems through four core functions applied across the AI lifecycle."
related_to: ["[[ai-rmf-core-functions]]", "[[trustworthy-ai-characteristics]]", "[[ai-rmf-profile]]", "[[ai-actor-taxonomy]]", "[[ai-lifecycle-dimensions]]", "[[ai-rmf-risk-framing-challenges]]", "[[ai-risks-vs-traditional-software-risks]]", "[[human-ai-interaction-risk]]", "[[related-risk-governance-frameworks]]", "[[aisvs-standard]]", "[[genai-top10-framework-mappings]]"]
sources:
  - url: "https://github.com/GenAI-Security-Project/GenAI-LLM-Top10"
    type: "github-repo"
    synced_at: "2026-09-10"
  - url: "https://github.com/OWASP/AISVS"
    type: "github-repo"
    synced_at: "2026-09-10"
  - url: "https://www.nist.gov/itl/ai-risk-management-framework"
    type: "remote-binary"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
graphify_node_ids: ["nist_ai_100_1_document", "nist_ai_100_1_attributes_of_ai_rmf", "aisvs_nist_ai_rmf", "genai_top10_nist_ai_rmf_ref"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# NIST AI Risk Management Framework (AI RMF 1.0)

> A voluntary framework (NIST AI 100-1, released January 26, 2023) to help organizations manage risks to individuals, organizations, and society posed by AI systems, and to promote trustworthy AI.

## Description

The AI RMF is organized in two parts: Part 1 frames AI risk (understanding risks/impacts/harms, the challenges of measuring and prioritizing risk, and the [[trustworthy-ai-characteristics|seven characteristics of trustworthy AI]]), and Part 2 defines the operational core — [[ai-rmf-core-functions|four functions]] (GOVERN, MAP, MEASURE, MANAGE) applied continuously across the [[ai-lifecycle-dimensions|AI lifecycle]] — plus [[ai-rmf-profile|AI RMF Profiles]] that tailor the functions to specific use cases or sectors. The framework was developed through a consensus-driven, open, transparent, collaborative process with public comment periods (RFI July 2021, multiple public drafts December 2021–August 2022) and is maintained by NIST's Trustworthy and Responsible AI Resource Center (launched March 30, 2023), with companion resources including the [[related-risk-governance-frameworks|AI RMF Playbook]], an AI RMF Roadmap, and a Crosswalk to other standards.

## Design Attributes (Appendix D)

The framework is deliberately designed to be:
- **Voluntary** — organizations choose whether and how to adopt it.
- **Non-prescriptive and flexible** — usable across sectors, technologies, and organization sizes/maturity levels, and adaptable as AI technology and risk understanding evolve.
- **Rights-preserving** — oriented toward protecting civil rights, civil liberties, and privacy alongside technical risk management.
- **Structured for actionability** — organized around concrete functions ([[ai-rmf-core-functions]]) and profiles ([[ai-rmf-profile]]) rather than abstract principles alone.
- **Common-language building** — intended to give a shared vocabulary and structure ([[trustworthy-ai-characteristics]], [[ai-actor-taxonomy]]) for AI risk discussions across an organization and its stakeholders.

## Key Characteristics

- Applies across the full [[ai-lifecycle-dimensions|AI lifecycle]], not just at deployment.
- Distinguishes AI-specific risk from traditional software risk (see [[ai-risks-vs-traditional-software-risks]]).
- Explicitly addresses [[human-ai-interaction-risk|human-AI interaction]] as a risk dimension.
- Cross-references established risk/security frameworks rather than replacing them (see [[related-risk-governance-frameworks]]).

## Where it Applies

- [[ai-rmf-core-functions]] — the operational core this framework defines
- [[trustworthy-ai-characteristics]] — the definition of "trustworthy AI" this framework organizes around
- [[ai-actor-taxonomy]] — the stakeholder roles this framework's guidance is addressed to

## Related Concepts

- [[ai-rmf-profile]] — tailored implementations of the framework for specific contexts
- [[ai-rmf-risk-framing-challenges]] — the foundational risk-framing challenges (tolerance, prioritization, measurement) the framework responds to
- [[aisvs-standard]] — the OWASP AI Security Verification Standard cites the AI RMF as a related governance framework its testable security requirements complement
- [[genai-top10-framework-mappings]] — the OWASP GenAI LLM Top 10 (2026) maps most of its ten risks against the AI RMF, with NIST AI 600-1 cited separately as the companion Generative AI profile
