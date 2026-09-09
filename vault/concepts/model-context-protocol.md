---
type: concept
name: "MCP (Model Context Protocol)"
aliases: ["MCP", "Model Context Protocol"]
description: "An open integration standard used to build secure connections between an AI agent and the systems an organization already uses."
related_to: ["[[ai-connectors]]", "[[ai-plugins]]", "[[connection-governance]]"]
sources:
  - url: "https://docs.google.com/presentation/d/1TBAMg5BpdXgbZ2pfnHboCW9WP2IpAc5cpZfWw5IaNEs/edit"
    type: "gdoc"
    synced_at: "2026-09-03"
updated_at: "2026-09-03"
updated_by: "preserve@agent"
tags: [type/concept, domain/product]
graphify_node_id: "claude_cowork_workshop_portobank_mcp"
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# MCP (Model Context Protocol)

> MCP is the standard plug that connects the AI to your tools: your systems come to you.

## Description

MCP is an open protocol for building [[ai-connectors]] — secure links between an AI agent and existing systems (CRM, core banking, Drive, Teams, etc.) without custom one-off integration code. It underpins connection, live data access, and permission-respecting control between the agent and external tools.

## Key Characteristics

- Open standard, not a proprietary point-to-point integration
- Enables no-code connection setup for a given system
- Access is bounded by the user's existing permissions, with an audit trail

## Where it Applies

- Presented as the technical foundation of Connectors in Indicium's Claude Cowork enablement workshops (e.g., Portobank, Aug 2026), including core banking, CRM, and Drive/SharePoint integrations.

## Related Concepts

- [[ai-connectors]] — the integrations built on top of MCP
- [[ai-plugins]] — bundles that combine Connectors (via MCP) with Skills
- [[connection-governance]] — the control model applied to every MCP-based connection

---

## Expected Bidirectional Links

> This section is a reference for agents and can be removed in real pages.

| From | To | Field |
|---|---|---|
| Concept → Concept | `[[ai-connectors]]` | "Related Concepts" section |
