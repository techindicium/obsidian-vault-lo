---
type: concept
name: "AISVS Core Control Categories (C01-C12)"
aliases: ["AISVS Chapters", "AISVS Control Categories"]
description: "The 12 control categories that make up the operational core of the OWASP AISVS, from training data integrity through monitoring and logging, each containing leveled (L1/L2/L3) testable verification requirements."
related_to: ["[[aisvs-standard]]", "[[ai-security-controls-inventory]]", "[[prompt-injection]]", "[[model-context-protocol]]", "[[trust-boundary]]"]
sources:
  - url: "https://github.com/OWASP/AISVS"
    type: "github-repo"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
graphify_node_ids: ["aisvs_training_data_integrity_and_traceability", "aisvs_input_validation", "aisvs_model_lifecycle_management", "aisvs_infrastructure", "aisvs_access_control_and_identity", "aisvs_supply_chain", "aisvs_model_behavior", "aisvs_memory_embeddings_and_vector_database", "aisvs_orchestration_and_agentic_action", "aisvs_mcp_security", "aisvs_adversarial_robustness", "aisvs_monitoring_and_logging"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# AISVS Core Control Categories (C01-C12)

> The twelve control categories the [[aisvs-standard|OWASP AISVS]] organizes its testable requirements into, spanning the AI system lifecycle from training data through production monitoring.

## Description

Each category groups related, individually numbered, leveled (L1/L2/L3) verification requirements — the [[ai-security-controls-inventory|Controls Inventory]] (Appendix B) cross-references all of them against specific threats.

## The Twelve Categories

### C01 — Training Data Integrity & Traceability
Verifying that training/fine-tuning data is sourced, validated, and tracked so it can't be silently poisoned or its provenance lost. Closely tied to [[supply-chain-security-for-models|supply chain security]] concerns for third-party datasets.

### C02 — Input Validation
Validating and sanitizing inputs to AI systems — the AI-specific analogue of classic input validation, but extended to cover [[prompt-injection|prompt injection]] and adversarial inputs an LLM must handle that a traditional parser wouldn't see. Closely related to C05 (Access Control) and C11 (Adversarial Robustness) below.

### C03 — Model Lifecycle Management & Change Control
Controlling how models move from training through versioning, deployment, and retirement, with auditability of changes — the AI-specific analogue of change management.

### C04 — Infrastructure, Configuration & Deployment Security
Securing the infrastructure AI systems run on — compute, storage, serving infrastructure — against misconfiguration and unauthorized access.

### C05 — Access Control & Identity for AI Components & Users
Ensuring AI components and the humans/systems that interact with them are properly authenticated and authorized, with least-privilege access to models, data, and tools.

### C06 — Supply Chain Security for Models
Verifying the integrity and provenance of third-party models, datasets, and libraries an AI system depends on — closely related to C01 (Training Data Integrity) above and C03's model lifecycle controls.

### C07 — Model Behavior, Output Control & Safety Assurance
Ensuring model outputs stay within safe, intended bounds — covering [[hallucination|hallucination]] mitigation and output filtering.

### C08 — Memory, Embeddings & Vector Database Security
Securing the retrieval/memory layer of AI systems — protecting vector databases and embeddings from poisoning or unauthorized retrieval, central to secure [[retrieval-augmented-generation|RAG]] implementations.

### C09 — Orchestration & Agentic Security
Securing multi-step, tool-using agent workflows — preventing [[excessive-agency|excessive agency]] and unsafe autonomous action chains.

### C10 — MCP Security
Security requirements specific to the [[model-context-protocol|Model Context Protocol]] — scoping tool authorization, validating tool responses as untrusted input, and preventing a compromised MCP server from escalating agent privileges across the [[trust-boundary|trust boundary]] it represents.

### C11 — Adversarial Robustness
Hardening models against [[jailbreak|jailbreaks]], [[adversarial-example|adversarial examples]], and other deliberate attempts to manipulate model behavior.

### C12 — Monitoring, Logging & Anomaly Detection
Instrumenting AI systems so [[prompt-injection|prompt injection]] attempts, [[hallucination|hallucinations]], [[jailbreak|jailbreaks]], and anomalous agent behavior are detectable in production, not just at test time.

## Where it Applies

- [[aisvs-standard]] — these twelve categories are its operational core

## Related Concepts

- [[ai-security-controls-inventory]] — cross-references every category against specific threats and controls
