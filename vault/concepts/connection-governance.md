---
type: concept
name: "Connection Governance"
aliases: ["Governança na Conexão"]
description: "The governance model applied to every AI-to-system integration: access never exceeds the user's own permissions, and each connection gets its own specific control."
related_to: ["[[ai-connectors]]", "[[model-context-protocol]]"]
sources:
  - url: "https://docs.google.com/presentation/d/1TBAMg5BpdXgbZ2pfnHboCW9WP2IpAc5cpZfWw5IaNEs/edit"
    type: "gdoc"
    synced_at: "2026-09-03"
updated_at: "2026-09-09"
updated_by: "preserve@agent"
tags: [type/concept, domain/product]
graphify_node_id: "claude_cowork_workshop_portobank_governanca_conexao"
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Connection Governance

> MCP connects without coding — the agent reaches the tools the organization already uses, with an audit trail and easy disconnection.

## Description

A governance model for every AI-to-system integration, built on three rules: (1) access is never greater than the connecting user's own — responses are restricted to that person's profile, group, and inbox; (2) every integration (core banking, CRM, SharePoint, chat) expands the agent's reach and therefore requires its own specific, pre-approved control; (3) [[model-context-protocol|MCP]] connects to existing tools without custom development, with an audit trail and simple disconnection.

## Key Characteristics

- Access is capped at the connecting user's existing permissions
- Each new connection requires its own homologated, specific control — not a blanket policy
- Every connection is auditable and can be disabled easily

## Where it Applies

- Presented as the governance layer over [[ai-connectors]] in Indicium's Claude Cowork enablement workshops (e.g., Portobank, Aug 2026), particularly relevant for regulated industries like banking.

## Related Concepts

- [[ai-connectors]] — the integrations this governance model applies to
- [[model-context-protocol]] — the underlying connection standard
- [[agentic-ai-enterprise-architecture]] — applies this same least-privilege model via RBAC on that architecture's knowledge bases component

---

## Expected Bidirectional Links

> This section is a reference for agents and can be removed in real pages.

| From | To | Field |
|---|---|---|
| Concept → Concept | `[[ai-connectors]]` | "Related Concepts" section |
