---
type: concept
name: "AI for Code Generation (Security Guidance)"
aliases: ["AISVS Appendix C", "AI-Assisted Coding Security"]
description: "AISVS Appendix C — security guidance for AI-assisted software development: hardening AI code-review/assistant bots, securing CI/CD pipelines that use AI augmentation, detecting adversarial AI-generated contributions, and validating the origin of AI-produced artifacts."
related_to: ["[[aisvs-standard]]", "[[aisvs-core-categories]]", "[[shift-left-testing]]", "[[coding-standards]]"]
sources:
  - url: "https://github.com/OWASP/AISVS"
    type: "github-repo"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
graphify_node_ids: ["aisvs_ai_for_code_generation", "aisvs_ai_code_review_bot_hardening", "aisvs_cicd_hardening_ai_augmentation", "aisvs_adversarial_ai_inbound_contributions", "aisvs_ai_artifact_provenance"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# AI for Code Generation (Security Guidance)

> AISVS's Appendix C: security guidance for a specific high-risk use case — using AI to write, review, and contribute code — rather than a general restatement of [[coding-standards|coding standards]].

## Description

As AI-assisted and AI-generated code becomes common, the software supply chain gains new risk surfaces that traditional [[shift-left-testing|shift-left]] and [[coding-standards|coding-standards]] practices weren't designed around: an AI reviewer bot can itself be manipulated, a CI/CD pipeline that lets an AI agent commit or merge code needs its own hardening, and the provenance of AI-authored code needs to be tracked just as carefully as human-authored code's provenance is under [[aisvs-core-categories|Supply Chain Security (C06)]].

## Sub-Themes

### AI Code-Review & Assistant Bot Hardening
Securing the AI tools that review, suggest, or auto-fix code — so the reviewer/assistant itself can't be manipulated (e.g. via a crafted PR description) into approving insecure changes.

### CI/CD Pipeline Hardening for AI Augmentation
Extending pipeline security controls to cover AI agents that participate in the pipeline (auto-committing, auto-merging, auto-deploying) rather than assuming only humans act on it.

### Adversarial AI Detection in Inbound Contributions
Detecting when an incoming contribution (PR, commit) is itself adversarially crafted to exploit an AI reviewer or downstream AI-augmented tooling.

### AI Artifact Origin Validation & Audit Trail
Tracking whether a given code artifact was AI-generated, AI-assisted, or human-authored, with an audit trail — the code-provenance analogue of [[aisvs-core-categories|Training Data Integrity & Traceability (C01)]].

## Where it Applies

- [[aisvs-core-categories]] — extends Supply Chain Security (C06) concerns specifically to AI-assisted code contributions
- [[shift-left-testing]] — AI-assisted coding changes where and how defects get introduced, relevant to shift-left practice
- [[coding-standards]] — AI-generated code still needs to satisfy the same coding standards, verified by different means

## Related Concepts

- [[aisvs-core-categories]]
