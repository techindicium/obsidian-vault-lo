---
type: topic
title: "Plataforma / C6 AI Hub"
aliases: ["Plataforma", "C6 AI Hub"]
category: "feature"
status: "in-progress"
people: ["[[rodrigo-freitas-encaua]]", "[[lucas-zanotelli-dos-santos]]", "[[marcos-wada]]", "[[everson-tavares]]", "[[marcelo-arakaki]]", "[[eduardo-scarpellini]]"]
actors: []
objective: "Sustain the C6 AI Hub (Hub and Spoke model) with centralized security, governance, and telemetry/observability."
created_at: "2026-09-08"
sources:
  - url: "https://docs.google.com/document/d/1Fo-4N6U46H-fmslNRm9R6yBZKEhA_dseO0W7irHO2PE/edit"
    type: "gdoc"
    synced_at: "2026-09-11"
  - url: "https://docs.google.com/presentation/d/1X5J3edLcAK9rNlnhhF2VLPW_qDLYvyp736uXlRJd6wI/edit"
    type: "gdoc"
    synced_at: "2026-09-11"
updated_at: "2026-09-11"
updated_by: "preserve@agent"
tags: [type/topic, status/in-progress, category/feature, domain/growth]
---

<!-- Zettelkasten role: bridge note -->

# Plataforma / C6 AI Hub

> One of the six workstreams of the [[ai-transformation-project-c6-bank]] engagement: sustain the "C6 AI Hub" (Hub and Spoke model) with centralized security, governance, and telemetry/observability.

## Context

Owned by [[rodrigo-freitas-encaua]] and [[lucas-zanotelli-dos-santos]] (Indicium side), with [[marcos-wada]] as the C6-side architecture contact, and [[everson-tavares]] / [[marcelo-arakaki]] / [[eduardo-scarpellini]] on the C6 platform team. The team is testing a model-hub tool inspired by Nubank's internal equivalent ("Light"), targeting ~4,500 users. C6 is also migrating its AWS infrastructure away from Terraform toward a Kubernetes-based IaC tool not yet confirmed by the team.

## People Involved

| Person | Role |
|---|---|
| [[rodrigo-freitas-encaua]] | Indicium co-owner (SecOps Security) |
| [[lucas-zanotelli-dos-santos]] | Indicium co-owner (Platform lead) |
| [[marcos-wada]] | C6 architecture contact |
| [[everson-tavares]] | C6 platform specialist |
| [[marcelo-arakaki]] | C6 platform tech lead |
| [[eduardo-scarpellini]] | C6 platform head |

## History

| Date | Event |
|---|---|
| 2026-09-08 | Scope and squad confirmed at the internal kickoff; LightLLM research assigned |

## Decisions

- (none formalized yet — IaC tool replacing Terraform still unconfirmed)

## Next Steps

- [ ] Research LightLLM as the model-hub candidate, owners: [[rodrigo-freitas-encaua]], [[lucas-zanotelli-dos-santos]]
- [ ] Confirm the Kubernetes-based IaC tool replacing Terraform

---

## Expected Bidirectional Links

> This section is a reference for agents and can be removed in real pages.

| From | To | Field |
|---|---|---|
| Topic → Person | `[[rodrigo-freitas-encaua]]` etc. | `people` in frontmatter |
| Topic → Project | `[[ai-transformation-project-c6-bank]]` | body reference / project's `related_topics` |
