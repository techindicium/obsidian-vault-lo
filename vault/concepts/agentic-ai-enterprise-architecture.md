---
type: concept
name: "Agentic AI Enterprise Architecture"
aliases: ["Agentic AI Reference Architecture", "AWS Agentic AI Architecture"]
description: "A layered reference architecture for enterprise agentic AI: an applications layer and an agents layer built on three core services (model access, tools, knowledge bases), governed by cross-layer observability, security, and discoverability."
related_to: ["[[connection-governance]]", "[[model-context-protocol]]"]
sources:
  - url: "https://docs.aws.amazon.com/prescriptive-guidance/latest/govern-architect-agentic-ai/enterprise-architecture.html"
    type: "remote-binary"
    synced_at: "2026-09-09"
updated_at: "2026-09-09"
updated_by: "preserve@agent"
tags: [type/concept, domain/product]
graphify_node_ids:
  - "tmp_bedrock_learn_1788959326_enterprise_architecture_knowledge_bases_component"
  - "tmp_bedrock_learn_1788959326_enterprise_architecture_model_access_component"
  - "tmp_bedrock_learn_1788959326_enterprise_architecture_retrieval_augmented_generation"
  - "tmp_bedrock_learn_1788959326_enterprise_architecture_three_core_service_categories"
  - "tmp_bedrock_learn_1788959326_enterprise_architecture_guardrails"
  - "tmp_bedrock_learn_1788959326_enterprise_architecture_role_based_access_control"
  - "tmp_bedrock_learn_1788959326_enterprise_architecture_agent_to_agent_orchestration"
  - "tmp_bedrock_learn_1788959326_enterprise_architecture_agents_layer"
  - "tmp_bedrock_learn_1788959326_enterprise_architecture_llm"
  - "tmp_bedrock_learn_1788959326_enterprise_architecture_long_term_memory"
  - "tmp_bedrock_learn_1788959326_enterprise_architecture_short_term_memory"
  - "tmp_bedrock_learn_1788959326_enterprise_architecture_applications_layer"
  - "tmp_bedrock_learn_1788959326_enterprise_architecture_genai_end_user_applications"
  - "tmp_bedrock_learn_1788959326_enterprise_architecture_non_genai_applications"
  - "tmp_bedrock_learn_1788959326_enterprise_architecture_tools_component"
  - "tmp_bedrock_learn_1788959326_enterprise_architecture_overview"
  - "tmp_bedrock_learn_1788959326_enterprise_architecture_cross_layer_concerns"
  - "tmp_bedrock_learn_1788959326_enterprise_architecture_discoverability"
  - "tmp_bedrock_learn_1788959326_enterprise_architecture_observability"
  - "tmp_bedrock_learn_1788959326_enterprise_architecture_security"
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->
<!-- Links in the body must have context: "commonly used by [[billing-api]] and [[notification-service]] for resilient HTTP calls" -->

# Agentic AI Enterprise Architecture

> Two layers of applications sit on three governed core services, with observability, security, and discoverability cutting across all of them.

## Description

AWS's prescriptive-guidance reference architecture for enterprise agentic AI organizes the system into layers that let organizations run AI agents in production while keeping enterprise control. An **applications layer** (generative-AI end-user apps plus non-GenAI business systems) sits above an **agents layer**, where agents interpret goals, reason and plan, call tools, retrieve knowledge, and hold short- and long-term memory — including agent-to-agent communication and orchestration for multi-agent collaboration. Agents consume three core service categories: a **model access** component (foundation-model access with policy enforcement, guardrails, and cost tracking), a **tools** component (discovery and secure, authorized execution of tools), and a **knowledge bases** component (vector/graph-backed retrieval for retrieval-augmented generation, gated by role-based access control so retrieval respects least-privilege and need-to-know). Observability, security, and discoverability are cross-layer concerns spanning all of the above, so AI operations stay monitored, auditable, and policy-compliant.

## Key Characteristics

- Two application types (GenAI end-user apps, non-GenAI business systems) share the same underlying agent and service layers
- Model access, tools, and knowledge bases are treated as distinct, independently governed services rather than agent-embedded logic
- RBAC on the knowledge bases component enforces least-privilege/need-to-know specifically for retrieval-augmented generation
- Guardrails and cost tracking are attached to model access, not bolted on afterward
- Observability, security, and discoverability are explicitly cross-layer, not owned by a single layer

## Where it Applies

- Useful as the reference shape when scoping how an AI-transformation initiative structures agent-to-tool and agent-to-data access, rather than letting each agent integrate ad hoc

## Related Concepts

- [[connection-governance]] — a similar least-privilege, per-connection control model, here applied specifically to the knowledge bases component via RBAC
- [[model-context-protocol]] — the kind of standard the tools component's "secure execution and discovery" is implemented with in practice

---

## Expected Bidirectional Links

> This section is a reference for agents and can be removed in real pages.

| From | To | Field |
|---|---|---|
| Concept → Concept | `[[connection-governance]]` | "Related Concepts" section |
| Concept → Concept | `[[model-context-protocol]]` | "Related Concepts" section |
