---
type: concept
name: "Excessive Agency"
aliases: ["Excessive Autonomy"]
description: "A risk where an agentic AI system is granted, or arrogates to itself, more permission or capability to act than its task actually requires — leading to unintended or unauthorized actions."
related_to: ["[[aisvs-standard]]", "[[aisvs-core-categories]]", "[[agentic-ai]]", "[[model-context-protocol]]"]
sources:
  - url: "https://github.com/OWASP/AISVS"
    type: "github-repo"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
graphify_node_ids: ["aisvs_excessive_agency"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Excessive Agency

> An [[agentic-ai|agentic]] system holding, or being able to exercise, more permission or capability than its task genuinely requires — the AI-specific analogue of the classic security principle of least privilege.

## Description

Excessive agency manifests when an agent has broader tool access, higher-privilege credentials, or wider action scope than the specific task at hand needs — so a single compromised prompt, a [[prompt-injection|prompt injection]], or a simple planning error can cascade into consequential unauthorized action rather than a contained mistake. AISVS's Orchestration & Agentic Security category and its MCP Security category both address bounding agent authorization tightly per-task and per-tool, rather than granting broad standing permissions.

## Key Characteristics

- The AI-specific analogue of least-privilege: an agent should hold only the permissions its current task needs.
- Amplifies the blast radius of other failures (a single prompt injection can trigger high-impact action if the agent already has broad permissions).
- Bounded primarily through per-tool, per-task authorization scoping — not just overall system-level access control.

## Where it Applies

- [[aisvs-core-categories]] — Orchestration & Agentic Security (C09) and MCP Security (C10) both address bounding agent authorization

## Related Concepts

- [[agentic-ai]] — the system class this risk applies to
- [[model-context-protocol]] — a common mechanism where per-tool authorization scoping is enforced
