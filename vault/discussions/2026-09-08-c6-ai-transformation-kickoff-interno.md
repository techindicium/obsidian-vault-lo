---
type: discussion
title: "C6 AI Transformation — Kickoff Interno"
aliases: ["C6 Kickoff Interno", "C6 Internal Kickoff"]
date: "2026-09-08"
summary: "Indicium's internal kickoff for the AI Transformation Project at C6 Bank: contract origin and scope, six workstreams / five squads, full team roster, and the project's operating rules (DLP, manual de bordo, agile cadence)."
conclusions:
  - "Indicium hired as C6 Bank's exclusive strategic partner for its AI transformation."
  - "Scope structured into six workstreams / five squads: Assessment, Esteira AI-nativa, Knowledge Works, AITO, Plataforma, Enablement."
  - "All confidential information and transcription tooling must operate inside C6's network environment, per DLP policy."
  - "Consultants will access C6 via physical machines imaged by the bank, not VMs (VM access was evaluated and discarded as unworkable)."
action_items:
  - "Retest Kiro vs. Claude on telemetry/log export limitations — owner: Guilherme Zanotelli dos Santos"
  - "Research LightLLM for the model hub — owners: Rodrigo Freitas Encáua, Lucas Zanotelli dos Santos"
  - "Hold biweekly tactical squad meetings this week to detail epics/features/user stories"
  - "Map required software/platforms in advance, given slow tool-approval processes in a banking environment"
  - "Create a project Slack channel with the full team"
  - "Run a form for the team to jointly choose a permanent team name (provisionally \"time C6\")"
related_topics: ["[[2026-09-esteira-ai-nativa-c6]]", "[[2026-09-knowledge-works-c6]]", "[[2026-09-plataforma-c6-ai-hub]]", "[[2026-09-enablement-c6]]", "[[2026-09-assessment-c6]]"]
related_actors: []
related_people: ["[[leandro-ciscar]]", "[[alberto-tadashi-yamamoto]]", "[[igor-beninca]]", "[[vagner-strapasson]]", "[[tabi-thuler-santos]]", "[[lucas-zanotelli-dos-santos]]", "[[rodrigo-freitas-encaua]]", "[[pedro-ferraresi]]", "[[douglas-sgrott]]", "[[isadora-busch]]", "[[gabriel-eckschmidt-buso]]", "[[filipe-duarte]]", "[[aluizio-cidral-junior]]", "[[guilherme-zanotelli-dos-santos]]", "[[fabio-gomes-de-oliveira]]", "[[gabriel-bernardo]]", "[[gabriel-klock]]", "[[daniel-avancini]]", "[[lorena-santos]]"]
related_projects: ["[[ai-transformation-project-c6-bank]]"]
related_teams: []
source: "meeting-notes"
sources:
  - url: "c6/meeting_and_notes/2026-09-08-kickoff-interno-transcricao.md"
    type: "local-dir"
    synced_at: "2026-09-10"
  - url: "c6/project_docs/kickoff-interno-transformacao-ai-set2026.md"
    type: "local-dir"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/discussion, domain/growth]
---

<!-- Zettelkasten role: bridge note -->

# C6 AI Transformation — Kickoff Interno

> Indicium's internal kickoff meeting (1h13m, 2026-09-08) for the [[ai-transformation-project-c6-bank]] engagement — the source of most operational detail about the project's origin, scope, team, and rules that doesn't appear in the official deck or manual.

## Context

Opened by [[leandro-ciscar]] (DM). The project originated from a hands-on Claude workshop in São Paulo that Anthropic ran directly with C6's CTO, which became a commercial lead — per [[fabio-gomes-de-oliveira]], C6 chose Indicium over competitor CIT specifically because CIT already serves Itaú (C6's direct competitor) and C6 wanted to avoid competing with Itaú for CIT's best people; C6 explicitly said it wants to be Indicium's largest client in Brazil. Contract signed 2026-09-03: US$3.8M (~R$20M), Indicium's largest LatAm project, 12 months, targeting 4,000 employees and 42M customers.

[[alberto-tadashi-yamamoto]] framed the project against a failed ~R$60M Itaú AI initiative that only reached 15% of its goal by focusing on technology while ignoring process and human resistance — arguing the real difficulty here isn't banking as a domain, but organizational scale (4,000 employees, 800 in IT).

C6 has already purchased AI licenses directly from Anthropic (900 Kiro, 200 Claude, 100 Gemini) and expects the project to activate them for productivity, then redesign processes/products for new AI-native revenue starting around month 9.

## Participants

| Person | Role |
|---|---|
| [[leandro-ciscar]] | Delivery Manager, opened the meeting |
| [[alberto-tadashi-yamamoto]] | AITO / Consulting |
| [[igor-beninca]] | AITO / Consulting, Principal Consultant |
| [[vagner-strapasson]] | Cloud Architect (AWS FSI) |
| [[tabi-thuler-santos]] | Change Management |
| [[lucas-zanotelli-dos-santos]] | Plataforma lead |
| [[rodrigo-freitas-encaua]] | Plataforma / SecOps |
| [[pedro-ferraresi]] | Enablement lead |
| [[douglas-sgrott]] | Knowledge Works |
| [[isadora-busch]] | Knowledge Works, Consultant Product |
| [[gabriel-eckschmidt-buso]] | Knowledge Works, Consultant Process |
| [[filipe-duarte]] | Esteira AI-nativa |
| [[aluizio-cidral-junior]] | Esteira AI-nativa |
| [[guilherme-zanotelli-dos-santos]] | Esteira AI-nativa |
| [[fabio-gomes-de-oliveira]] | Commercial |
| [[gabriel-bernardo]] | attendee, raised the DLP/transcription question |
| [[gabriel-klock]] | attendee, role unconfirmed |
| [[daniel-avancini]] | AITO / Consulting (20%), gave closing remarks |
| [[lorena-santos]] | Esteira AI-nativa (Consultant Product) |

## Conclusions

- Indicium hired as C6 Bank's exclusive strategic partner for its AI transformation.
- Scope structured into six workstreams / five squads: [[2026-09-assessment-c6]], [[2026-09-esteira-ai-nativa-c6]], [[2026-09-knowledge-works-c6]], AITO, [[2026-09-plataforma-c6-ai-hub]], [[2026-09-enablement-c6]].
- All confidential information and transcription tooling must operate inside C6's network environment, per DLP policy — reinforcing the [[ai-transformation-project-c6-bank]] Manual de Bordo's "nothing leaves the C6 environment" rule.
- Consultants will access C6 via physical machines imaged by the bank, not VMs — VM access was evaluated and discarded as unworkable.

## Action Items

- [ ] Retest Kiro vs. Claude on telemetry/log export limitations — owner: [[guilherme-zanotelli-dos-santos]]
- [ ] Research LightLLM for the model hub — owners: [[rodrigo-freitas-encaua]], [[lucas-zanotelli-dos-santos]]
- [ ] Hold biweekly tactical squad meetings this week to detail epics/features/user stories
- [ ] Map required software/platforms in advance, given slow tool-approval processes in a banking environment
- [ ] Create a project Slack channel with the full team
- [ ] Run a form for the team to jointly choose a permanent team name (provisionally "time C6")

## Related Projects

- [[ai-transformation-project-c6-bank]]

## Related Topics

- [[2026-09-esteira-ai-nativa-c6]]
- [[2026-09-knowledge-works-c6]]
- [[2026-09-plataforma-c6-ai-hub]]
- [[2026-09-enablement-c6]]
- [[2026-09-assessment-c6]]

---

## Expected Bidirectional Links

> This section is a reference for agents and can be removed in real pages.

| From | To | Field |
|---|---|---|
| Discussion → Person | `[[leandro-ciscar]]` etc. | `related_people` in frontmatter |
| Discussion → Project | `[[ai-transformation-project-c6-bank]]` | `related_projects` in frontmatter |
| Discussion → Topic | `[[2026-09-esteira-ai-nativa-c6]]` etc. | `related_topics` in frontmatter |
| Project → Discussion | `[[2026-09-08-c6-ai-transformation-kickoff-interno]]` | "Discussions" section in Project |
