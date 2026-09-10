---
type: topic
title: "Esteira AI-nativa — SDLC Redesign (C6 Bank)"
aliases: ["Esteira AI-nativa", "C6 SDLC Redesign"]
category: "rfc"
status: "in-progress"
people: ["[[paulo-pituba]]", "[[thiago-ribeiro]]", "[[filipe-duarte]]", "[[lorena-santos]]", "[[aluizio-cidral-junior]]", "[[guilherme-zanotelli-dos-santos]]", "[[vagner-strapasson]]"]
actors: []
objective: "Redesign C6 Bank's SDLC end-to-end (branch to deploy) with Kiro, for ~1,000 developers across 78 squads."
created_at: "2026-09-08"
sources:
  - url: "c6/meeting_and_notes/2026-09-08-kickoff-interno-transcricao.md"
    type: "local-dir"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/topic, status/in-progress, category/rfc, domain/growth]
---

<!-- Zettelkasten role: bridge note -->

# Esteira AI-nativa — SDLC Redesign (C6 Bank)

> One of the six workstreams of the [[ai-transformation-project-c6-bank]] engagement: redesign C6 Bank's software delivery lifecycle end-to-end using Kiro, for ~1,000 developers across 78 squads.

## Context

Sponsored by [[paulo-pituba]] (CTO) and [[thiago-ribeiro]] ("right-hand," Senior IT Executive). Per [[igor-beninca]] at the 2026-09-08 internal kickoff (see [[2026-09-08-c6-ai-transformation-kickoff-interno]]), this is the workstream that "pays the project's bill": C6 currently spends ~R$10-15M/year on third-party development consultancies, and eliminating that cost by redesigning the SDLC in-house is the sponsors' real objective — a figure that appears in neither the official deck nor the manual, only in the raw kickoff transcript.

A live technical debate at the kickoff pitted Kiro against Claude for this workstream: [[rodrigo-freitas-encaua]] argued Kiro has security/compliance advantages, while [[igor-beninca]] countered that Kiro has a real limitation — it retains telemetry/logs for only ~30 days, which is a problem for exporting to tools like Grafana. [[guilherme-zanotelli-dos-santos]] was assigned to retest Kiro vs. Claude on this point.

## People Involved

| Person | Role |
|---|---|
| [[paulo-pituba]] | sponsor (C6 CTO) |
| [[thiago-ribeiro]] | co-sponsor (C6 Senior IT Executive) |
| [[filipe-duarte]] | Indicium squad member |
| [[lorena-santos]] | Indicium squad member |
| [[aluizio-cidral-junior]] | Indicium squad member |
| [[guilherme-zanotelli-dos-santos]] | Indicium squad member — retesting Kiro vs. Claude |
| [[vagner-strapasson]] | Indicium squad member (Cloud Architect) |

## History

| Date | Event |
|---|---|
| 2026-09-08 | Scope, sponsors, and squad confirmed at the internal kickoff; Kiro-vs-Claude telemetry debate raised as an open technical question |

## Decisions

- Kiro selected as the primary tool for the SDLC redesign, pending resolution of its telemetry/log-retention limitation (~30 days) — re-test assigned to [[guilherme-zanotelli-dos-santos]]

## Next Steps

- [ ] Retest Kiro vs. Claude on telemetry/log export, owner: [[guilherme-zanotelli-dos-santos]]
- [ ] Detail epics/features/user stories in the first biweekly tactical squad meeting

---

## Expected Bidirectional Links

> This section is a reference for agents and can be removed in real pages.

| From | To | Field |
|---|---|---|
| Topic → Person | `[[paulo-pituba]]` etc. | `people` in frontmatter |
| Topic → Project | `[[ai-transformation-project-c6-bank]]` | body reference / project's `related_topics` |
| Person → Topic | `[[2026-09-esteira-ai-nativa-c6]]` | "Active Topics"/"Projects" in Person |
