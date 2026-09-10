---
type: concept
name: "Trust Boundary"
aliases: ["Trust Boundaries"]
description: "A point in an AI system's data or control flow where content or authority crosses from one trust level to another — e.g. from an external tool response into the model's context, or from a user's permission scope into an agent's action scope."
related_to: ["[[aisvs-standard]]", "[[aisvs-core-categories]]", "[[model-context-protocol]]", "[[prompt-injection]]", "[[excessive-agency]]"]
sources:
  - url: "https://github.com/OWASP/AISVS"
    type: "github-repo"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
graphify_node_ids: ["aisvs_trust_boundary"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Trust Boundary

> A point where content or authority crosses from a less-trusted context into a more-trusted one within an AI system — the place where validation and authorization checks matter most.

## Description

Every point where an AI system consumes external content as if it were safe, or exercises authority beyond what was directly granted, is a trust boundary. A [[model-context-protocol|MCP]] connection to an external tool is a trust boundary; a [[retrieval-augmented-generation|RAG]] retrieval from an external corpus is a trust boundary; an agent inheriting a user's permissions to take action is a trust boundary. [[prompt-injection|Indirect prompt injection]] and [[excessive-agency|excessive agency]] both exploit trust boundaries where validation was assumed rather than enforced — treating content or delegated authority as more trustworthy than it actually is.

## Key Characteristics

- Applies to both data flow (content crossing into the model's context) and control flow (authority crossing into an agent's action scope).
- The recurring failure mode: treating something that crossed a trust boundary as already-validated, when it hasn't been.
- A useful lens for auditing agentic and tool-integrated AI systems — identify every trust boundary, then verify each one enforces validation/authorization rather than assuming it.

## Where it Applies

- [[model-context-protocol]] — an MCP connection is itself a trust boundary between the agent and an external system
- [[aisvs-core-categories]] — MCP Security (C10) and Orchestration & Agentic Security (C09) are organized around identifying and securing trust boundaries

## Related Concepts

- [[prompt-injection]] — indirect injection specifically exploits unvalidated content crossing a trust boundary
- [[excessive-agency]] — arises when authority crosses a trust boundary without adequate scoping
