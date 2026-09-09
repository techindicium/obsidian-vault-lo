---
type: concept
name: "Connectors (AI Integrations)"
aliases: ["Connectors"]
description: "Secure MCP-based connections that let an AI agent read and update an organization's existing systems directly, without copy-pasting between screens."
related_to: ["[[model-context-protocol]]", "[[ai-plugins]]", "[[connection-governance]]", "[[claude-cowork-interaction-model]]"]
sources:
  - url: "https://docs.google.com/presentation/d/1TBAMg5BpdXgbZ2pfnHboCW9WP2IpAc5cpZfWw5IaNEs/edit"
    type: "gdoc"
    synced_at: "2026-09-03"
updated_at: "2026-09-03"
updated_by: "preserve@agent"
tags: [type/concept, domain/product]
graphify_node_id: "claude_cowork_workshop_portobank_connectors"
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Connectors (AI Integrations)

> Live data, at the source — your systems come to you.

## Description

A Connector is a secure connection, built with [[model-context-protocol]], that lets an AI agent reach a system the organization already uses (Teams, Drive, CRM, core banking, etc.). Three properties define a Connector: it can be enabled without custom development ("Connect"); it lets the agent read and update information directly in the source system instead of manual copy-paste ("Access"); and it respects existing permissions with an audit trail and easy disconnection ("Control").

## Key Characteristics

- No-code activation of a connection to an existing system
- Direct read/write access at the data source, not a manual export/import
- Access is capped at what the connecting user is already permitted to see

## Where it Applies

- Taught as one of the three building blocks (with Skills and Automation) of value creation in Indicium's Claude Cowork enablement workshops (e.g., Portobank, Aug 2026), covering CRM, core banking, Drive/SharePoint, Outlook/Gmail, and Teams/Hangout.

## Related Concepts

- [[model-context-protocol]] — the open standard Connectors are built on
- [[ai-plugins]] — bundles that package Connectors together with Skills
- [[connection-governance]] — the control layer applied to each Connector

---

## Expected Bidirectional Links

> This section is a reference for agents and can be removed in real pages.

| From | To | Field |
|---|---|---|
| Concept → Concept | `[[model-context-protocol]]` | "Related Concepts" section |
