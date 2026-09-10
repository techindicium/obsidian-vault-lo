---
type: concept
name: "GenAI LLM Top 10 Framework Mappings"
aliases: ["OWASP GenAI Framework Crosswalk", "LLM Top 10 Appendix A", "LLM Top 10 AISVS Mapping"]
description: "The two appendices of the OWASP LLM Top 10 (2026) that cross-reference its ten risks against external frameworks — MITRE ATLAS/ATT&CK/CWE, NIST AI RMF/AI 600-1, CSA AICM, OWASP AISVS/AIVSS/ASI — as a lookup aid, not new requirements."
related_to: ["[[genai-top10-standard]]", "[[aisvs-standard]]", "[[nist-ai-risk-management-framework]]", "[[mitre-atlas]]"]
sources:
  - url: "https://github.com/GenAI-Security-Project/GenAI-LLM-Top10"
    type: "github-repo"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
graphify_node_ids: ["genai_top10_appendix_a_framework_mappings", "genai_top10_appendix_aisvs_mapping", "genai_top10_dsgai_ref", "genai_top10_mitre_attack_ref", "genai_top10_asi_ref", "genai_top10_mitre_cwe_ref", "genai_top10_csa_aicm_ref", "genai_top10_nist_ai_600_1_ref", "genai_top10_owasp_aivss_ref"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# GenAI LLM Top 10 Framework Mappings

> Two appendices in the [[genai-top10-standard|OWASP LLM Top 10 (2026)]] that map its ten numbered risks against a coverage matrix of external security and governance frameworks — a lookup aid for teams already using one of those frameworks.

## Description

Appendix A provides a coverage matrix (primary vs. supporting mapping) between each of the ten LLM Top 10 risks and each external framework below; a second appendix (informally "LLMZZ") does the same specifically against [[aisvs-standard|OWASP AISVS]]'s twelve control categories. Neither appendix introduces new requirements — they exist purely so a team can navigate between the risk-framed LLM Top 10 and whichever control-framed standard (AISVS, NIST AI RMF, etc.) their organization already follows.

## Frameworks in the Coverage Matrix

- **[[mitre-atlas|MITRE ATLAS]]** — mapped as a primary reference for all ten risks (every risk has documented adversarial-ML technique parallels in ATLAS).
- **MITRE ATT&CK** — supporting-level mapping for risks with a clear traditional-cyberattack analogue.
- **MITRE CWE (Common Weakness Enumeration)** — supporting-level mapping to classic weakness categories the AI-specific risk resembles.
- **[[nist-ai-risk-management-framework|NIST AI RMF]]** — primary mapping for most risks, absent for a few (e.g. LLM10 Improper Output Handling has no direct AI RMF mapping since it's a classic software-security concern applied to AI output).
- **NIST AI 600-1 (Generative AI Profile)** — NIST's companion profile applying the AI RMF specifically to generative AI, referenced here as a distinct document from the base AI RMF text.
- **CSA AI Controls Matrix (AICM)** — the Cloud Security Alliance's AI-specific controls framework, mapped as a complementary control catalogue.
- **OWASP AIVSS (AI Vulnerability Scoring System)** — mapped for risks where a severity-scoring companion metric applies (e.g. Prompt Injection, Excessive Agency, Misinformation).
- **OWASP Top 10 for Agentic Applications (ASI) 2026** — a sibling OWASP project focused specifically on agentic-AI risk, mapped for the risks most relevant to agentic systems.

## Where it Applies

- [[genai-top10-standard]] — these are its two appendices
- [[aisvs-standard]] — the second appendix maps every LLM Top 10 risk to specific AISVS control categories

## Related Concepts

- [[nist-ai-risk-management-framework]] — one of the primary-mapped external frameworks
- [[mitre-atlas]] — mapped against all ten risks
