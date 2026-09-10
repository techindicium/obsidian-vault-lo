---
type: concept
name: "Agent / Agentic AI"
aliases: ["Agentic AI", "AI Agent"]
description: "An AI system that autonomously plans and takes multi-step actions — calling tools, invoking other systems, making decisions — toward a goal, rather than producing a single response to a single input."
related_to: ["[[aisvs-standard]]", "[[aisvs-core-categories]]", "[[excessive-agency]]", "[[model-context-protocol]]"]
sources:
  - url: "https://github.com/OWASP/AISVS"
    type: "github-repo"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
graphify_node_ids: ["aisvs_agentic_ai"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Agent / Agentic AI

> An AI system that autonomously plans and executes multi-step actions toward a goal — calling tools, invoking other systems, chaining decisions — rather than just producing one response to one input.

## Description

Agentic AI introduces security concerns beyond single-turn LLM interaction: an agent that can call tools and take action needs its autonomy explicitly bounded, or it risks [[excessive-agency|excessive agency]] — taking actions beyond what was actually authorized. Tool invocation itself is frequently mediated through protocols like [[model-context-protocol|MCP]], which introduces its own [[trust-boundary|trust-boundary]] concerns. AISVS dedicates a full control category (Orchestration & Agentic Security) to these risks, distinct from the model-behavior concerns of single-turn interactions.

## Key Characteristics

- Multi-step, autonomous, tool-using — not a single-turn Q&A interaction.
- Introduces the risk of [[excessive-agency|excessive agency]]: acting beyond intended authorization.
- Tool invocation commonly mediated via protocols like [[model-context-protocol|MCP]], each a distinct trust boundary.

## Where it Applies

- [[aisvs-core-categories]] — Orchestration & Agentic Security (C09) and MCP Security (C10) both address agentic-AI-specific risks

## Related Concepts

- [[excessive-agency]] — the central risk agentic systems introduce
- [[model-context-protocol]] — the common mechanism agents use to invoke external tools
