---
type: topic
title: "Advanced SDLC & Harness Course (Daniel Avancini)"
aliases: ["Advanced SDLC & Harness", "Daniel Avancini SDLC Course"]
category: "compliance"
status: "in-progress"
people: ["[[lorena-santos]]", "[[daniel-avancini]]"]
actors: []
objective: "Read and ingest, one at a time, the full reading list from Daniel Avancini's Advanced SDLC & Harness course, turning each source into vault concepts (shift-left testing, AI governance frameworks, security verification standards) rather than just summarizing them."
created_at: "2026-09-10"
sources: []
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/topic, status/in-progress, category/compliance, domain/engineering]
---

<!-- Zettelkasten role: bridge note -->
<!-- Links in the body explain WHY permanents relate -->

# Advanced SDLC & Harness Course (Daniel Avancini)

> Working through the reading list for the Advanced SDLC & Harness course, ingesting each source into the vault as concepts rather than a one-off summary — /learn one link at a time.

## Context

Lorena is taking a course on Advanced SDLC & Harness created and taught by [[daniel-avancini]]. The course reading list spans shift-left testing practice, AI risk/governance frameworks (NIST AI RMF, ISO/IEC 42001), AI-specific security verification standards (OWASP AISVS, OWASP GenAI LLM Top 10), SDLC maturity measurement (OWASP SAMM), an internal reference repo (`techindicium/idev`), Claude Code output styles docs, a community skills repo (mattpocock/skills), and Theo (t3.gg)'s YouTube channel. Each source is ingested via `/bedrock:learn`, which runs it through graphify extraction and `/bedrock:preserve`, producing new or updated `concept` entities in `domain/engineering` rather than a single "course notes" dump — so the knowledge stays reusable and cross-linkable with the rest of the vault.

## People Involved

| Person | Role |
|---|---|
| [[lorena-santos]] | learner / requester |
| [[daniel-avancini]] | course creator / instructor (Indicium co-founder & Chief Data Officer) |

## Reading List & Progress

| # | Source | Status | Key concepts created/updated |
|---|---|---|---|
| 1 | [Applying the Shift-Left Approach](https://www.stickyminds.com/article/shift-left-approach-software-testing) | ✅ done | [[shift-left-testing]], [[static-code-analysis]], [[unit-testing]], [[software-testing-pyramid]], [[coding-standards]], [[service-virtualization]], [[continuous-testing]], [[security-testing]], [[performance-testing]], [[capers-jones-cost-of-defect-graph]], [[gdpr]], [[devops]] |
| 2 | [NIST AI Risk Management Framework](https://www.nist.gov/itl/ai-risk-management-framework) | ✅ done | [[nist-ai-risk-management-framework]], [[ai-rmf-core-functions]], [[trustworthy-ai-characteristics]], [[ai-rmf-profile]], [[ai-actor-taxonomy]], [[ai-lifecycle-dimensions]], [[ai-rmf-risk-framing-challenges]], [[ai-risks-vs-traditional-software-risks]], [[human-ai-interaction-risk]], [[related-risk-governance-frameworks]] |
| 3 | [OWASP AISVS](https://github.com/OWASP/AISVS) | ✅ done | [[aisvs-standard]], [[aisvs-core-categories]], [[ai-security-controls-inventory]], [[ai-for-code-generation-security]], [[prompt-injection]], [[jailbreak]], [[guardrails]], [[hallucination]], [[retrieval-augmented-generation]], [[data-poisoning]], [[model-extraction]], [[adversarial-example]], [[agentic-ai]], [[excessive-agency]], [[trust-boundary]], [[owasp-asvs]], [[mitre-atlas]], [[iso-42001]] (stub), [[owasp-genai-llm-top10]] (stub); updated [[model-context-protocol]] |
| 4 | [OWASP GenAI Threats / LLM Top 10](https://genai.owasp.org/) | ✅ done | [[genai-top10-standard]], [[sensitive-information-disclosure]], [[ai-supply-chain-risk]], [[unbounded-consumption]], [[misinformation]], [[hidden-context-exposure]], [[vector-and-embedding-weaknesses]], [[improper-output-handling]], [[genai-top10-framework-mappings]]; updated [[prompt-injection]], [[excessive-agency]], [[data-poisoning]], [[mitre-atlas]], [[nist-ai-risk-management-framework]], [[ai-rmf-profile]] |
| 5 | [ISO/IEC 42001](https://www.iso.org/standard/42001) | ✅ done (secondary sources — iso.org blocks fetch + full text is paywalled) | Enriched [[iso-42001]] stub (clause structure, Annex A controls, certification, EU AI Act/ISO 27001 relationship); created [[iso-27001]], [[eu-ai-act]] |
| 6 | [OWASP SAMM](https://owaspsamm.org/) | ✅ done (fetched 15 individual practice pages directly — PDF conversion was killed/too heavy) | [[samm-standard]], [[samm-governance]], [[samm-design]], [[samm-implementation]], [[samm-verification]], [[samm-operations]]; updated [[security-testing]], [[coding-standards]], [[shift-left-testing]], [[static-code-analysis]] |
| 7 | [idev](https://github.com/techindicium/idev) | ❌ skipped (Lorena's request) | — |
| 8 | [Claude Code Output Styles](https://code.claude.com/docs/en/output-styles) | ⬜ pending | — |
| 9 | [Mattpocock skills](https://github.com/mattpocock/skills) | ⬜ pending | — |
| 10 | [Theo — t3.gg (YouTube)](https://www.youtube.com/@t3dotgg) | ⬜ pending | — |

## History

| Date | Event |
|---|---|
| 2026-09-10 | Started the course reading list; ingested sources 1-4 (shift-left testing, NIST AI RMF, OWASP AISVS, OWASP GenAI LLM Top 10) via `/bedrock:learn`; paused at Lorena's request before continuing to source 5 |
| 2026-09-10 | Created `person` entities for [[lorena-santos]] (learner) and [[daniel-avancini]] (course creator, Indicium co-founder & CDO) and linked them to this topic; Lorena confirmed continuing the list and asked to skip source 7 (idev) |
| 2026-09-10 | Ingested source 5 (ISO/IEC 42001) from secondary sources since `iso.org` blocks automated fetching and the standard itself is paywalled; enriched the [[iso-42001]] stub and created [[iso-27001]] and [[eu-ai-act]] stubs |
| 2026-09-10 | Ingested source 6 (OWASP SAMM): PDF conversion via docling was killed for excessive resource use, so fetched all 15 practice pages directly instead; created [[samm-standard]] + 5 business-function concepts, cross-linked into existing shift-left/security-testing concepts. Lorena asked to stop after this one and schedule sources 8-10 to run overnight |

## Decisions

- Course content classified under a new `domain/engineering` tag rather than the vault's existing PM domains (`product`, `design`, `research`, `analytics`, `growth`), since it's SDLC/security/governance practice content, not product management content. Documented in the vault's `CLAUDE.md`.
- Overlapping concepts across sources (e.g. `prompt-injection`, `excessive-agency`, `data-poisoning`, `nist-ai-risk-management-framework`, `mitre-atlas` appearing in both AISVS and GenAI Top 10) are updated in place — sources and cross-links accumulate — rather than duplicated per source.
- Citations to frameworks not yet ingested directly (ISO 42001, MITRE ATLAS parts, OWASP ASVS, GenAI LLM Top 10 initially) were captured as lightweight stub concepts, to be enriched when this topic's own reading list reaches them.

## Next Steps

- [x] ~~Ingest ISO/IEC 42001~~ — enriched [[iso-42001]] from secondary sources (RSI Security, Konfirmity), since iso.org blocks fetching and the full standard is paywalled
- [x] ~~Ingest OWASP SAMM~~ — done; the PDF conversion attempt was killed (resource-heavy), so fetched the 15 practice pages directly from owaspsamm.org instead
- [ ] Schedule remaining sources (8-10) to run overnight, per Lorena's request 2026-09-10
- [x] ~~Ingest idev~~ — skipped per Lorena's request
- [ ] Ingest [Claude Code Output Styles docs](https://code.claude.com/docs/en/output-styles)
- [ ] Ingest [Mattpocock skills repo](https://github.com/mattpocock/skills)
- [ ] Ingest [Theo (t3.gg) YouTube channel](https://www.youtube.com/@t3dotgg)

---

## Expected Bidirectional Links

> This section is a reference for agents and can be removed in real pages.

| From | To | Field |
|---|---|---|
| Topic → Person | `[[lorena-santos]]` | `people` in frontmatter |
| Person → Topic | `[[2026-09-compliance-advanced-sdlc-harness-course]]` | "Active Topics" in Person |
