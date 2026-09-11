---
type: concept
name: "Shadow AI"
aliases: ["Shadow AI", "Unauthorized AI Use"]
description: "The use of unapproved AI tools, extensions, or APIs by employees, which removes IT's visibility over corporate data and creates uncontrolled data-leakage and prompt-injection exposure."
related_to: ["[[ai-transformation-office]]", "[[2026-09-knowledge-works-c6]]"]
sources:
updated_at: "2026-09-11"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
---

<!-- Zettelkasten role: permanent note -->

# Shadow AI

> The use of a tool, browser extension, or API not approved by IT, which strips away visibility over corporate data and exposes the organization to leakage and prompt-injection risk.

## Description

Shadow AI names the central day-to-day AI-governance risk inside an organization: employees reaching for ungoverned generative-AI tools to move faster, without IT's knowledge. Once data flows through an unapproved tool, IT loses the ability to audit what left the corporate boundary. Two failure modes recur: (1) pasting proprietary code, credentials, or sensitive customer data into a public AI instance — which trains external commercial models on that data, i.e. a data leak; (2) installing an unaudited marketplace extension/add-on, which exposes the local system to prompt injection.

The mitigation pattern is **least privilege + confidentiality by default**: sensitive data (PII, trade secrets, source code, financial data) may only touch AI tooling backed by a no-training guarantee; public/free AI tools are off-limits for any corporate data, since free tiers use prompts to train new commercial models. Synthetic, anonymized, or masked data is the safe substitute when AI assistance is still needed for reasoning.

## Key Characteristics

- Removes IT's visibility over where corporate/client data actually flows
- Two concrete vectors: (1) pasting sensitive data into public AI, which trains external models on it — a data leak; (2) installing an unaudited AI extension/add-on, which exposes the system to prompt injection
- Detectable early via usage signals (e.g., token volume spikes far beyond expected use)
- Mitigated by least-privilege + confidentiality-by-default policy, not by banning AI outright

## Where it Applies

- [[2026-09-knowledge-works-c6]] — C6 Bank's own workstream to bring governed generative AI to business areas specifically to reduce Shadow AI; some users were already found "blowing past" expected token volumes before the workstream started
- [[ai-transformation-office]] — AITO is the governance layer meant to keep Shadow AI in check across an organization's AI rollout

## Related Concepts

- [[ai-transformation-office]] — the governance structure that is supposed to keep Shadow AI contained at an organizational level

---

## Expected Bidirectional Links

> This section is a reference for agents and can be removed in real pages.

| From | To | Field |
|---|---|---|
| Concept → Topic | `[[2026-09-knowledge-works-c6]]` | "Where it Applies" section |
| Concept → Concept | `[[ai-transformation-office]]` | "Related Concepts" section |
| Topic → Concept | `[[shadow-ai]]` | body reference |
