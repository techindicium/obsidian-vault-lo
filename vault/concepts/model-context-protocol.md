---
type: concept
name: "MCP (Model Context Protocol)"
aliases: ["MCP", "Model Context Protocol"]
description: "An open integration standard used to build secure connections between an AI agent and the systems an organization already uses."
related_to: ["[[ai-connectors]]", "[[ai-plugins]]", "[[connection-governance]]", "[[aisvs-standard]]", "[[aisvs-core-categories]]", "[[trust-boundary]]"]
sources:
  - url: "https://github.com/OWASP/AISVS"
    type: "github-repo"
    synced_at: "2026-09-10"
  - url: "https://docs.google.com/presentation/d/1TBAMg5BpdXgbZ2pfnHboCW9WP2IpAc5cpZfWw5IaNEs/edit"
    type: "gdoc"
    synced_at: "2026-09-03"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/product, domain/engineering]
graphify_node_ids: ["claude_cowork_workshop_portobank_mcp", "aisvs_mcp", "aisvs_model_context_protocol"]
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
- [[agentic-ai-enterprise-architecture]] — the kind of standard that architecture's tools component implements for secure tool discovery and execution
- [[aisvs-core-categories]] — treats "MCP Security" as its own verification category (tool-authorization scoping, prompt/tool-response provenance, preventing a compromised MCP server from escalating agent privileges)
- [[trust-boundary]] — an MCP connection is itself a trust boundary the agent crosses into an external system

## Security Considerations (AISVS)

The [[aisvs-standard|OWASP AI Security Verification Standard]] treats MCP as a distinct verification category precisely because it crosses a [[trust-boundary|trust boundary]]: an agent invoking tools over MCP must have its authorization scoped per-tool (not blanket trust of the MCP server), tool responses must be treated as untrusted input subject to the same validation as any external data, and a compromised or malicious MCP server should not be able to escalate the agent's effective privileges beyond what the connecting user/system was granted.

---

## Expected Bidirectional Links

> This section is a reference for agents and can be removed in real pages.

| From | To | Field |
|---|---|---|
| Concept → Concept | `[[ai-connectors]]` | "Related Concepts" section |
