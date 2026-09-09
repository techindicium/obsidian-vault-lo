---
type: concept
name: "/schedule Command"
aliases: ["/schedule", "scheduled task command"]
description: "The command used inside Claude Cowork to turn any task into a recurring or on-demand automated routine."
related_to: ["[[ai-automation-routines]]", "[[claude-cowork-interaction-model]]"]
sources:
  - url: "https://docs.google.com/presentation/d/1TBAMg5BpdXgbZ2pfnHboCW9WP2IpAc5cpZfWw5IaNEs/edit"
    type: "gdoc"
    synced_at: "2026-09-03"
updated_at: "2026-09-03"
updated_by: "preserve@agent"
tags: [type/concept, domain/product]
graphify_node_id: "claude_cowork_workshop_portobank_schedule_command"
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# /schedule Command

> Type /schedule on any Cowork task, or use "Scheduled" in the sidebar to create and manage tasks.

## Description

The concrete command that turns a one-off Cowork task into an [[ai-automation-routines|automation routine]] — either recurring or on-demand. It requires the host computer to be on, Claude Desktop open, and an active internet connection, since this is unavailable in ordinary chats outside Cowork.

## Key Characteristics

- Invoked with `/schedule` on any existing Cowork task, or via the "Scheduled" sidebar panel
- Requires an always-on machine with Claude Desktop open and internet access
- The mechanism that makes a task recurring rather than one-time

## Where it Applies

- Documented as the concrete how-to for creating routines in Indicium's Claude Cowork enablement workshops (e.g., Portobank, Aug 2026).

## Related Concepts

- [[ai-automation-routines]] — the capability this command creates
- [[claude-cowork-interaction-model]] — the product this command is part of

---

## Expected Bidirectional Links

> This section is a reference for agents and can be removed in real pages.

| From | To | Field |
|---|---|---|
| Concept → Concept | `[[ai-automation-routines]]` | "Related Concepts" section |
