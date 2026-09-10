# Graph Report - bedrock-learn-1  (2026-09-01)

## Corpus Check
- Corpus is ~1,115 words - fits in a single context window. You may not need a graph.

## Summary
- 15 nodes · 27 edges · 4 communities (3 shown, 1 thin omitted)
- Extraction: 93% EXTRACTED · 4% INFERRED · 4% AMBIGUOUS · INFERRED: 1 edges (avg confidence: 0.85)
- Token cost: 0 input · 61,915 output

## Community Hubs (Navigation)
- Research Sourcing & Rapport Tactics
- C6 Bank Career & AI Project
- Education & Regulatory Background
- Shared Network Connection

## God Nodes (most connected - your core abstractions)
1. `Strategic Profile — Paulo Pituba (CTO, C6 Bank)` - 11 edges
2. `Paulo Pituba` - 9 edges
3. `C6 Bank` - 5 edges
4. `Nelson Novaes Neto` - 4 edges
5. `AI Transformation Project — C6 Bank` - 4 edges
6. `Lorena Santos` - 3 edges
7. `Rede (Itaú Unibanco Group acquiring/payments company)` - 3 edges
8. `Daniel (Shared LinkedIn Connection)` - 3 edges
9. `Banco Central do Brasil (Bacen)` - 3 edges
10. `Label + Calibrated Question Rapport Tactic` - 3 edges

## Surprising Connections (you probably didn't know these)
- `Paulo Pituba` --references--> `AI Transformation Project — C6 Bank`  [INFERRED]
  perfil-paulo-pituba.md → perfil-paulo-pituba.md  _Bridges community 2 → community 1_
- `Strategic Profile — Paulo Pituba (CTO, C6 Bank)` --references--> `AI Transformation Project — C6 Bank`  [EXTRACTED]
  perfil-paulo-pituba.md → perfil-paulo-pituba.md  _Bridges community 0 → community 1_
- `Strategic Profile — Paulo Pituba (CTO, C6 Bank)` --references--> `Banco Central do Brasil (Bacen)`  [EXTRACTED]
  perfil-paulo-pituba.md → perfil-paulo-pituba.md  _Bridges community 0 → community 2_
- `Strategic Profile — Paulo Pituba (CTO, C6 Bank)` --references--> `Daniel (Shared LinkedIn Connection)`  [EXTRACTED]
  perfil-paulo-pituba.md → perfil-paulo-pituba.md  _Bridges community 0 → community 3_
- `Paulo Pituba` --references--> `Daniel (Shared LinkedIn Connection)`  [EXTRACTED]
  perfil-paulo-pituba.md → perfil-paulo-pituba.md  _Bridges community 2 → community 3_

## Hyperedges (group relationships)
- **AI Transformation Project Stakeholders at C6 Bank** — perfil_paulo_pituba_lorena_santos, perfil_paulo_pituba_paulo_pituba, perfil_paulo_pituba_c6_bank, perfil_paulo_pituba_ai_transformation_project [EXTRACTED 1.00]
- **Paulo Pituba's Career Trajectory (Itaú/Rede → C6 Bank)** — perfil_paulo_pituba_paulo_pituba, perfil_paulo_pituba_rede, perfil_paulo_pituba_itau_unibanco, perfil_paulo_pituba_c6_bank [EXTRACTED 1.00]
- **Calibrated-Question Rapport Tactic Applied to Paulo Pituba** — perfil_paulo_pituba_label_calibrated_question_tactic, perfil_paulo_pituba_never_split_the_difference, perfil_paulo_pituba_paulo_pituba [EXTRACTED 1.00]

## Communities (4 total, 1 thin omitted)

### Community 0 - "Research Sourcing & Rapport Tactics"
Cohesion: 0.50
Nodes (5): Strategic Profile — Paulo Pituba (CTO, C6 Bank), Label + Calibrated Question Rapport Tactic, LinkedIn, Never Split the Difference (Chris Voss), ZoomInfo

### Community 1 - "C6 Bank Career & AI Project"
Cohesion: 0.50
Nodes (4): AI Transformation Project — C6 Bank, C6 Bank, Itaú Unibanco, Rede (Itaú Unibanco Group acquiring/payments company)

### Community 2 - "Education & Regulatory Background"
Cohesion: 0.67
Nodes (4): Banco Central do Brasil (Bacen), Nelson Novaes Neto, Paulo Pituba, Universidade de São Paulo (USP)

## Ambiguous Edges - Review These
- `Paulo Pituba` → `Banco Central do Brasil (Bacen)`  [AMBIGUOUS]
  perfil-paulo-pituba.md · relation: references

## Knowledge Gaps
- **4 isolated node(s):** `Itaú Unibanco`, `Universidade de São Paulo (USP)`, `ZoomInfo`, `LinkedIn`
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 4 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)
- **1 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **What is the exact relationship between `Paulo Pituba` and `Banco Central do Brasil (Bacen)`?**
  _Edge tagged AMBIGUOUS (relation: references) - confidence is low._
- **Why does `Strategic Profile — Paulo Pituba (CTO, C6 Bank)` connect `Research Sourcing & Rapport Tactics` to `C6 Bank Career & AI Project`, `Education & Regulatory Background`, `Shared Network Connection`?**
  _High betweenness centrality (0.481) - this node is a cross-community bridge._
- **Why does `Paulo Pituba` connect `Education & Regulatory Background` to `Research Sourcing & Rapport Tactics`, `C6 Bank Career & AI Project`, `Shared Network Connection`?**
  _High betweenness centrality (0.352) - this node is a cross-community bridge._
- **Why does `Rede (Itaú Unibanco Group acquiring/payments company)` connect `C6 Bank Career & AI Project` to `Education & Regulatory Background`?**
  _High betweenness centrality (0.143) - this node is a cross-community bridge._
- **What connects `Itaú Unibanco`, `Universidade de São Paulo (USP)`, `ZoomInfo` to the rest of the system?**
  _4 weakly-connected nodes found - possible documentation gaps or missing edges._

---

# Merge on 2026-09-01

# Graph Report - bedrock-learn-2  (2026-09-01)

## Corpus Check
- Corpus is ~4,417 words - fits in a single context window. You may not need a graph.

## Summary
- 74 nodes · 113 edges · 8 communities
- Extraction: 87% EXTRACTED · 4% INFERRED · 9% AMBIGUOUS · INFERRED: 5 edges (avg confidence: 0.79)
- Token cost: 0 input · 84,696 output

## Community Hubs (Navigation)
- Public Profile & Affiliations
- MIT Research Collaborations
- C6 Bank C-Suite
- Negotiation Tactics (Voss Playbook)
- Behavioral Security Research
- Secure-by-Design AI at C6
- C6 Bank Founding Ideals
- Additional Academic Publications

## God Nodes (most connected - your core abstractions)
1. `Nelson Novaes Neto` - 35 edges
2. `C6 Bank` - 15 edges
3. `Secure-by-Design AI Framework (10 strategic questions)` - 10 edges
4. `A Case Study of the Capital One Data Breach (2020 paper)` - 9 edges
5. `C6 Bank Hexagon of 6 Founding Ideals` - 9 edges
6. `Never Split the Difference — Negotiation Tactics` - 8 edges
7. `Perfil Estratégico: Nelson Novaes Neto (Strategic Profile Document)` - 6 edges
8. `MIT Sloan School of Management` - 5 edges
9. `An Executive Guide to Secure-by-Design AI (2025 paper)` - 5 edges
10. `Developing a Global Data Breach Database and the Challenges Encountered (2021 paper)` - 5 edges

## Surprising Connections (you probably didn't know these)
- `Nelson Novaes Neto` --conceptually_related_to--> `Alexandra Pain (C6 Bank CMO)`  [AMBIGUOUS]
  perfil-nelson-novaes-neto.md → perfil-nelson-novaes-neto.md  _Bridges community 0 → community 2_
- `C6 Bank` --implements--> `Four-Part Platform Architecture (experimentation vs. production)`  [AMBIGUOUS]
  perfil-nelson-novaes-neto.md → perfil-nelson-novaes-neto.md  _Bridges community 2 → community 5_
- `Nelson Novaes Neto` --references--> `Executive's Guide to Developing Secure AI Systems (video)`  [INFERRED]
  perfil-nelson-novaes-neto.md → perfil-nelson-novaes-neto.md  _Bridges community 0 → community 5_
- `C6 Bank Hexagon of 6 Founding Ideals` --semantically_similar_to--> `Secure-by-Design AI Framework (10 strategic questions)`  [INFERRED] [semantically similar]
  perfil-nelson-novaes-neto.md → perfil-nelson-novaes-neto.md  _Bridges community 5 → community 6_
- `Secure-by-Design AI Framework (10 strategic questions)` --semantically_similar_to--> `Calibrated Questions (How/What)`  [INFERRED] [semantically similar]
  perfil-nelson-novaes-neto.md → perfil-nelson-novaes-neto.md  _Bridges community 5 → community 4_

## Hyperedges (group relationships)
- **C6 Bank's Six Founding Ideals (Hexagon of Purpose)** — perfil_nelson_novaes_neto_ideal_autorcracia, perfil_nelson_novaes_neto_ideal_quebrar_status_quo, perfil_nelson_novaes_neto_ideal_arte_de_discordar, perfil_nelson_novaes_neto_ideal_bom_humor, perfil_nelson_novaes_neto_ideal_respeito_etica_transparencia, perfil_nelson_novaes_neto_ideal_frescobol [EXTRACTED 1.00]
- **Never Split the Difference Tactical Playbook for Nelson Conversation** — perfil_nelson_novaes_neto_tactical_empathy, perfil_nelson_novaes_neto_calibrated_questions, perfil_nelson_novaes_neto_accusation_audit, perfil_nelson_novaes_neto_black_swan_technique, perfil_nelson_novaes_neto_thats_right_technique, perfil_nelson_novaes_neto_never_split_the_difference_tactics [EXTRACTED 1.00]
- **MIT Cybersecurity Research Collaborators (Madnick Lab Co-Authors)** — perfil_nelson_novaes_neto_nelson_novaes_neto, perfil_nelson_novaes_neto_stuart_madnick, perfil_nelson_novaes_neto_anchises_moraes_g_de_paula, perfil_nelson_novaes_neto_natasha_malara_borges, perfil_nelson_novaes_neto_angelica_marotta, perfil_nelson_novaes_neto_kevin_powers [INFERRED 0.85]

## Communities (8 total, 0 thin omitted)

### Community 0 - "Public Profile & Affiliations"
Cohesion: 0.13
Nodes (18): Angelica Marotta, FGV, Google Scholar, Grupo UOL, (ISC)² Latin America, Itaú Unibanco, Kevin Powers, Cybersecurity at MIT Sloan (CAMS) (+10 more)

### Community 1 - "MIT Research Collaborations"
Cohesion: 0.22
Nodes (11): ACM, Anchises Moraes G. de Paula, Journal of Data and Information Quality (JDIQ), Medium article: A Case Study of the Capital One Data Breach, MIT CISL, Natasha Malara Borges, NIST Cybersecurity Framework 1.1, A Case Study of the Capital One Data Breach (2020 paper) (+3 more)

### Community 2 - "C6 Bank C-Suite"
Cohesion: 0.24
Nodes (10): Alexandra Pain (C6 Bank CMO), AWS (Amazon Web Services), C6 Bank, Cybersecurity Culture at C6 Bank (MIT case study, 2020), Csixer Culture Identity, Fernando Astolfi (C6 Bank Chief Risk Officer), José Santana (C6 Bank CISO), Rafael Brazão (C6 Bank CHRO) (+2 more)

### Community 3 - "Negotiation Tactics (Voss Playbook)"
Cohesion: 0.29
Nodes (8): Accusation Audit, Black Swan (Hidden Leverage), Chris Voss, Perfil Estratégico: Nelson Novaes Neto (Strategic Profile Document), Lorena Santos, Never Split the Difference — Negotiation Tactics, Tactical Empathy (Labeling), 'That's Right' vs 'You're Right' Technique

### Community 4 - "Behavioral Security Research"
Cohesion: 0.29
Nodes (8): Aversive Stimulus Mechanism (security control as aversive stimulus), Behaviorismo / Análise Experimental do Comportamento, A Internet como um laboratório para a análise do comportamento: Psicologia Experimental (book), Calibrated Questions (How/What), The Effects of Security Controls on Human Behavior in Online Social Networks (paper), PUC-SP, Sérgio V. de Luna, Shadow AI

### Community 5 - "Secure-by-Design AI at C6"
Cohesion: 0.32
Nodes (8): C6 Bank blog post: IA generativa com AWS, C6 Bank Generative AI Platform (AWS partnership), Four-Part Platform Architecture (experimentation vs. production), MIT Sloan School of Management, 19 Critical Design Considerations, Secure-by-Design AI Framework (10 strategic questions), TI Inside, Executive's Guide to Developing Secure AI Systems (video)

### Community 6 - "C6 Bank Founding Ideals"
Cohesion: 0.29
Nodes (7): C6 Bank Hexagon of 6 Founding Ideals, A arte de discordar, Autorcracia, Bom humor, Frescobol, Quebrar o status quo, Respeito / Ética / Transparência

### Community 7 - "Additional Academic Publications"
Cohesion: 0.67
Nodes (4): Journal of Information System Security (JISSEC), Keri Pearlson, An Executive Guide to Secure-by-Design AI (2025 paper), ResearchGate

## Ambiguous Edges - Review These
- `Nelson Novaes Neto` → `Alexandra Pain (C6 Bank CMO)`  [AMBIGUOUS]
  perfil-nelson-novaes-neto.md · relation: conceptually_related_to
- `Nelson Novaes Neto` → `Fernando Astolfi (C6 Bank Chief Risk Officer)`  [AMBIGUOUS]
  perfil-nelson-novaes-neto.md · relation: conceptually_related_to
- `Nelson Novaes Neto` → `psyzone.org (Nelson's former personal site, ownership uncertain)`  [AMBIGUOUS]
  perfil-nelson-novaes-neto.md · relation: references
- `Nelson Novaes Neto` → `Rafael Brazão (C6 Bank CHRO)`  [AMBIGUOUS]
  perfil-nelson-novaes-neto.md · relation: conceptually_related_to
- `Nelson Novaes Neto` → `Rene Goncalves (C6 Bank COO)`  [AMBIGUOUS]
  perfil-nelson-novaes-neto.md · relation: conceptually_related_to
- `C6 Bank` → `Four-Part Platform Architecture (experimentation vs. production)`  [AMBIGUOUS]
  perfil-nelson-novaes-neto.md · relation: implements
- `C6 Bank` → `Secure-by-Design AI Framework (10 strategic questions)`  [AMBIGUOUS]
  perfil-nelson-novaes-neto.md · relation: implements
- `Secure-by-Design AI Framework (10 strategic questions)` → `C6 Bank Generative AI Platform (AWS partnership)`  [AMBIGUOUS]
  perfil-nelson-novaes-neto.md · relation: conceptually_related_to
- `Secure-by-Design AI Framework (10 strategic questions)` → `Four-Part Platform Architecture (experimentation vs. production)`  [AMBIGUOUS]
  perfil-nelson-novaes-neto.md · relation: rationale_for
- `Four-Part Platform Architecture (experimentation vs. production)` → `19 Critical Design Considerations`  [AMBIGUOUS]
  perfil-nelson-novaes-neto.md · relation: rationale_for

## Knowledge Gaps
- **28 isolated node(s):** `Chris Voss`, `Keri Pearlson`, `Angelica Marotta`, `Kevin Powers`, `Sérgio V. de Luna` (+23 more)
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 32 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **What is the exact relationship between `Nelson Novaes Neto` and `Alexandra Pain (C6 Bank CMO)`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **What is the exact relationship between `Nelson Novaes Neto` and `Fernando Astolfi (C6 Bank Chief Risk Officer)`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **What is the exact relationship between `Nelson Novaes Neto` and `psyzone.org (Nelson's former personal site, ownership uncertain)`?**
  _Edge tagged AMBIGUOUS (relation: references) - confidence is low._
- **What is the exact relationship between `Nelson Novaes Neto` and `Rafael Brazão (C6 Bank CHRO)`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **What is the exact relationship between `Nelson Novaes Neto` and `Rene Goncalves (C6 Bank COO)`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **What is the exact relationship between `C6 Bank` and `Four-Part Platform Architecture (experimentation vs. production)`?**
  _Edge tagged AMBIGUOUS (relation: implements) - confidence is low._
- **What is the exact relationship between `C6 Bank` and `Secure-by-Design AI Framework (10 strategic questions)`?**
  _Edge tagged AMBIGUOUS (relation: implements) - confidence is low._

---

# Merge on 2026-09-01

# Graph Report - bedrock-learn-5  (2026-09-01)

## Corpus Check
- Corpus is ~1,433 words - fits in a single context window. You may not need a graph.

## Summary
- 26 nodes · 47 edges · 5 communities
- Extraction: 74% EXTRACTED · 23% INFERRED · 2% AMBIGUOUS · INFERRED: 11 edges (avg confidence: 0.77)
- Token cost: 0 input · 65,732 output

## Community Hubs (Navigation)
- Redaction & English Consolidation
- Tagging & Item Taxonomy
- Source-to-Interview Governance
- Repo Origin & Hackathon Context
- Interview Confirmation Workflow

## God Nodes (most connected - your core abstractions)
1. `GTC Knowledge Hub — Collector` - 25 edges
2. `gtc-knowledge-hub-agent (sibling repo)` - 4 edges
3. `Source (vocabulary)` - 4 edges
4. `Knowledge Item Types` - 4 edges
5. `Tag Dimensions` - 4 edges
6. `Mandatory Human Confirmation` - 4 edges
7. `Approval Status (draft/approved/rejected)` - 4 edges
8. `Redaction Log` - 4 edges
9. `techindicium (Indicium AI)` - 3 edges
10. `Indicium AI 2026 Brazil Hackathon` - 3 edges

## Surprising Connections (you probably didn't know these)
- `Redaction (vocabulary)` --semantically_similar_to--> `Mandatory Human Confirmation`  [INFERRED] [semantically similar]
  gtc-knowledge-hub-collector.md → gtc-knowledge-hub-collector.md  _Bridges community 0 → community 4_
- `Approval Status (draft/approved/rejected)` --conceptually_related_to--> `Knowledge Item Types`  [INFERRED]
  gtc-knowledge-hub-collector.md → gtc-knowledge-hub-collector.md  _Bridges community 1 → community 4_
- `GTC Knowledge Hub — Collector` --references--> `ADR 0001 — Source como Briefing, não como Insumo`  [EXTRACTED]
  gtc-knowledge-hub-collector.md → gtc-knowledge-hub-collector.md  _Bridges community 0 → community 2_
- `GTC Knowledge Hub — Collector` --references--> `ADR 0003 — Knowledge Item Requires Client, Engagement Nullable`  [EXTRACTED]
  gtc-knowledge-hub-collector.md → gtc-knowledge-hub-collector.md  _Bridges community 0 → community 1_
- `gtc-knowledge-hub-agent (sibling repo)` --shares_data_with--> `GTC Knowledge Hub — Collector`  [EXTRACTED]
  gtc-knowledge-hub-collector.md → gtc-knowledge-hub-collector.md  _Bridges community 0 → community 3_

## Hyperedges (group relationships)
- **Agent-Led Interview Pipeline** — gtc_knowledge_hub_collector_source_concept, gtc_knowledge_hub_collector_interview_concept, gtc_knowledge_hub_collector_mandatory_human_confirmation, gtc_knowledge_hub_collector_knowledge_item_types [EXTRACTED 1.00]
- **Redaction Governance Mechanism** — gtc_knowledge_hub_collector_person_concept, gtc_knowledge_hub_collector_redaction_concept, gtc_knowledge_hub_collector_redaction_log, gtc_knowledge_hub_collector_redaction_categories [EXTRACTED 1.00]
- **Repository Origin Context** — gtc_knowledge_hub_collector, gtc_knowledge_hub_collector_gabriel_bernardo, gtc_knowledge_hub_collector_techindicium, gtc_knowledge_hub_collector_hackathon [EXTRACTED 1.00]

## Communities (5 total, 0 thin omitted)

### Community 0 - "Redaction & English Consolidation"
Cohesion: 0.33
Nodes (9): GTC Knowledge Hub — Collector, ADR 0002 — Relational Postgres for v1, ADR 0005 — Knowledge Item Consolidado em Inglês, English-Only Knowledge Base, Guilherme Losso, Person (vocabulary), Redaction Categories, Redaction (vocabulary) (+1 more)

### Community 1 - "Tagging & Item Taxonomy"
Cohesion: 0.40
Nodes (5): ADR 0003 — Knowledge Item Requires Client, Engagement Nullable, ADR 0004 — Technology and System as Distinct Tag Dimensions, Knowledge Item Types, Tag Dimensions, Controlled / Proposed Tag Status

### Community 2 - "Source-to-Interview Governance"
Cohesion: 0.67
Nodes (4): ADR 0001 — Source como Briefing, não como Insumo, Source (vocabulary), Source ≠ Item Governance Rule, Triage (vocabulary)

### Community 3 - "Repo Origin & Hackathon Context"
Cohesion: 0.67
Nodes (4): gtc-knowledge-hub-agent (sibling repo), Gabriel Bernardo, Indicium AI 2026 Brazil Hackathon, techindicium (Indicium AI)

### Community 4 - "Interview Confirmation Workflow"
Cohesion: 0.67
Nodes (4): Approval Status (draft/approved/rejected), Idempotent Commit, Interview (vocabulary), Mandatory Human Confirmation

## Ambiguous Edges - Review These
- `Gabriel Bernardo` → `gtc-knowledge-hub-agent (sibling repo)`  [AMBIGUOUS]
  gtc-knowledge-hub-collector.md · relation: conceptually_related_to

## Knowledge Gaps
- **1 isolated node(s):** `Guilherme Losso`
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 2 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **What is the exact relationship between `Gabriel Bernardo` and `gtc-knowledge-hub-agent (sibling repo)`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **Why does `GTC Knowledge Hub — Collector` connect `Redaction & English Consolidation` to `Tagging & Item Taxonomy`, `Source-to-Interview Governance`, `Repo Origin & Hackathon Context`, `Interview Confirmation Workflow`?**
  _High betweenness centrality (0.892) - this node is a cross-community bridge._
- **Why does `Knowledge Item Types` connect `Tagging & Item Taxonomy` to `Redaction & English Consolidation`, `Interview Confirmation Workflow`?**
  _High betweenness centrality (0.005) - this node is a cross-community bridge._
- **Why does `Tag Dimensions` connect `Tagging & Item Taxonomy` to `Redaction & English Consolidation`?**
  _High betweenness centrality (0.005) - this node is a cross-community bridge._
- **Are the 2 inferred relationships involving `gtc-knowledge-hub-agent (sibling repo)` (e.g. with `Indicium AI 2026 Brazil Hackathon` and `techindicium (Indicium AI)`) actually correct?**
  _`gtc-knowledge-hub-agent (sibling repo)` has 2 INFERRED edges - model-reasoned connections that need verification._
- **Are the 3 inferred relationships involving `Knowledge Item Types` (e.g. with `ADR 0003 — Knowledge Item Requires Client, Engagement Nullable` and `Approval Status (draft/approved/rejected)`) actually correct?**
  _`Knowledge Item Types` has 3 INFERRED edges - model-reasoned connections that need verification._
- **Are the 2 inferred relationships involving `Tag Dimensions` (e.g. with `Knowledge Item Types` and `Controlled / Proposed Tag Status`) actually correct?**
  _`Tag Dimensions` has 2 INFERRED edges - model-reasoned connections that need verification._

---

# Merge on 2026-09-01

# Graph Report - bedrock-learn-4  (2026-09-01)

## Corpus Check
- Corpus is ~1,468 words - fits in a single context window. You may not need a graph.

## Summary
- 37 nodes · 71 edges · 8 communities (6 shown, 2 thin omitted)
- Extraction: 89% EXTRACTED · 7% INFERRED · 4% AMBIGUOUS · INFERRED: 5 edges (avg confidence: 0.79)
- Token cost: 0 input · 89,108 output

## Community Hubs (Navigation)
- Knowledge Item Taxonomy
- ACL/Slack Bot Decisions
- Retrieval Interface & Quality
- Repo Origin & Hackathon Context
- Repository Pattern & Sources
- Client/Engagement Vocabulary
- Shared Postgres & Redaction
- Technology vs System Tagging

## God Nodes (most connected - your core abstractions)
1. `gtc-knowledge-hub-agent` - 30 edges
2. `Knowledge Item` - 14 edges
3. `ADR 0014: Knowledge Item Contract` - 7 edges
4. `gtc-knowledge-hub-collector` - 6 edges
5. `Thin MCP Server (search/get, no synthesis)` - 5 edges
6. `approved_knowledge_item(_expanded) view` - 5 edges
7. `Engagement` - 4 edges
8. `Slack Bot (MCP client)` - 4 edges
9. `Golden Set` - 4 edges
10. `Postgres (shared Knowledge Base instance)` - 4 edges

## Surprising Connections (you probably didn't know these)
- `gtc-knowledge-hub-agent` --references--> `Dormant ACL filtering model (ADR 0006/0007/0012)`  [AMBIGUOUS]
  gtc-knowledge-hub-agent.md → gtc-knowledge-hub-agent.md  _Bridges community 3 → community 1_
- `ADR 0005: SQLAlchemy behind a repository` --rationale_for--> `gtc-knowledge-hub-agent`  [EXTRACTED]
  gtc-knowledge-hub-agent.md → gtc-knowledge-hub-agent.md  _Bridges community 3 → community 4_
- `gtc-knowledge-hub-agent` --cites--> `ADR 0001: Thin MCP server`  [EXTRACTED]
  gtc-knowledge-hub-agent.md → gtc-knowledge-hub-agent.md  _Bridges community 3 → community 2_
- `gtc-knowledge-hub-agent` --references--> `Client`  [EXTRACTED]
  gtc-knowledge-hub-agent.md → gtc-knowledge-hub-agent.md  _Bridges community 3 → community 5_
- `gtc-knowledge-hub-agent` --references--> `Knowledge Item`  [EXTRACTED]
  gtc-knowledge-hub-agent.md → gtc-knowledge-hub-agent.md  _Bridges community 3 → community 0_

## Hyperedges (group relationships)
- **Retrieval Interface: thin MCP server + Slack bot over Knowledge Items** — gtc_knowledge_hub_agent_repo, gtc_knowledge_hub_agent_thin_mcp_server, gtc_knowledge_hub_agent_slack_bot, gtc_knowledge_hub_agent_knowledge_item [INFERRED 0.85]
- **Origin: techindicium, hackathon, and sibling repo behind the Knowledge Hub** — gtc_knowledge_hub_agent_repo, gtc_knowledge_hub_agent_gtc_knowledge_hub_collector, gtc_knowledge_hub_agent_techindicium, gtc_knowledge_hub_agent_indicium_ai_2026_brazil_hackathon [INFERRED 0.80]
- **Draft-to-approved governance pipeline across Collection and Retrieval** — gtc_knowledge_hub_agent_gtc_knowledge_hub_collector, gtc_knowledge_hub_agent_postgres, gtc_knowledge_hub_agent_approved_knowledge_item_view, gtc_knowledge_hub_agent_repo [EXTRACTED 1.00]

## Communities (8 total, 2 thin omitted)

### Community 0 - "Knowledge Item Taxonomy"
Cohesion: 0.25
Nodes (8): Knowledge Item, Decision Record (Knowledge Item type), Lesson Learned (Knowledge Item type), Pitfall (Knowledge Item type), Problem/Solution (Knowledge Item type), Success Case (Knowledge Item type), Methodology, Technologist

### Community 1 - "ACL/Slack Bot Decisions"
Cohesion: 0.38
Nodes (7): Dormant ACL filtering model (ADR 0006/0007/0012), ADR 0004: Postgres full-text search before vectors, ADR 0006: Slack bot as MCP client in this repo, ADR 0007: Self-hosted agent runtime for Slack bot, ADR 0009: Text search language config (portuguese to english), ADR 0014: Knowledge Item Contract, Slack Bot (MCP client)

### Community 2 - "Retrieval Interface & Quality"
Cohesion: 0.33
Nodes (6): ADR 0001: Thin MCP server, ADR 0017: Golden Set corpus, approved_knowledge_item(_expanded) view, Golden Set, Open governance gap: approval is global, not per-reader, Thin MCP Server (search/get, no synthesis)

### Community 3 - "Repo Origin & Hackathon Context"
Cohesion: 0.60
Nodes (5): Indicium AI 2026 Brazil Hackathon, gtc-knowledge-hub-agent, techindicium, Vagner Strapasson, Victor Giuliano

### Community 4 - "Repository Pattern & Sources"
Cohesion: 0.50
Nodes (4): ADR 0005: SQLAlchemy behind a repository, ADR 0013: Wiki.js as a source route, Groundwork (shared vocabulary), gtc-knowledge-hub-collector

### Community 5 - "Client/Engagement Vocabulary"
Cohesion: 0.67
Nodes (3): Client, Engagement, Engagement Team

## Ambiguous Edges - Review These
- `gtc-knowledge-hub-agent` → `Dormant ACL filtering model (ADR 0006/0007/0012)`  [AMBIGUOUS]
  gtc-knowledge-hub-agent.md · relation: references
- `ADR 0006: Slack bot as MCP client in this repo` → `Dormant ACL filtering model (ADR 0006/0007/0012)`  [AMBIGUOUS]
  gtc-knowledge-hub-agent.md · relation: references
- `ADR 0007: Self-hosted agent runtime for Slack bot` → `Dormant ACL filtering model (ADR 0006/0007/0012)`  [AMBIGUOUS]
  gtc-knowledge-hub-agent.md · relation: references

## Knowledge Gaps
- **5 isolated node(s):** `Lesson Learned (Knowledge Item type)`, `Decision Record (Knowledge Item type)`, `Pitfall (Knowledge Item type)`, `Success Case (Knowledge Item type)`, `Problem/Solution (Knowledge Item type)`
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 5 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)
- **2 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **What is the exact relationship between `gtc-knowledge-hub-agent` and `Dormant ACL filtering model (ADR 0006/0007/0012)`?**
  _Edge tagged AMBIGUOUS (relation: references) - confidence is low._
- **What is the exact relationship between `ADR 0006: Slack bot as MCP client in this repo` and `Dormant ACL filtering model (ADR 0006/0007/0012)`?**
  _Edge tagged AMBIGUOUS (relation: references) - confidence is low._
- **What is the exact relationship between `ADR 0007: Self-hosted agent runtime for Slack bot` and `Dormant ACL filtering model (ADR 0006/0007/0012)`?**
  _Edge tagged AMBIGUOUS (relation: references) - confidence is low._
- **Why does `gtc-knowledge-hub-agent` connect `Repo Origin & Hackathon Context` to `Knowledge Item Taxonomy`, `ACL/Slack Bot Decisions`, `Retrieval Interface & Quality`, `Repository Pattern & Sources`, `Client/Engagement Vocabulary`, `Shared Postgres & Redaction`, `Technology vs System Tagging`?**
  _High betweenness centrality (0.759) - this node is a cross-community bridge._
- **Why does `Knowledge Item` connect `Knowledge Item Taxonomy` to `Retrieval Interface & Quality`, `Repo Origin & Hackathon Context`, `Client/Engagement Vocabulary`, `Technology vs System Tagging`?**
  _High betweenness centrality (0.282) - this node is a cross-community bridge._
- **Why does `ADR 0014: Knowledge Item Contract` connect `ACL/Slack Bot Decisions` to `Retrieval Interface & Quality`, `Repo Origin & Hackathon Context`, `Repository Pattern & Sources`?**
  _High betweenness centrality (0.033) - this node is a cross-community bridge._
- **What connects `Lesson Learned (Knowledge Item type)`, `Decision Record (Knowledge Item type)`, `Pitfall (Knowledge Item type)` to the rest of the system?**
  _5 weakly-connected nodes found - possible documentation gaps or missing edges._

---

# Merge on 2026-09-02

# Graph Report - bedrock-learn-1788373178  (2026-09-02)

## Corpus Check
- Corpus is ~1,443 words - fits in a single context window. You may not need a graph.

## Summary
- 31 nodes · 43 edges · 5 communities
- Extraction: 88% EXTRACTED · 12% INFERRED · 0% AMBIGUOUS · INFERRED: 5 edges (avg confidence: 0.75)
- Token cost: 65,926 input · 5,697 output

## Community Hubs (Navigation)
- Data Stack Evolution
- Consensus & Eval Traces
- Agent Discoverability
- Cloud Warehouse Vendors
- Agent-Operable Integration

## God Nodes (most connected - your core abstractions)
1. `Post-AI Data Stack` - 9 edges
2. `The Shape and Feel of the Post-AI Data Stack` - 7 edges
3. `Cloud Data Warehouse` - 7 edges
4. `Modern Data Stack` - 6 edges
5. `Trace Patterns` - 6 edges
6. `Semantic Layers` - 5 edges
7. `Data Science Lifecycle` - 5 edges
8. `Agent-Readable Artifacts` - 4 edges
9. `Agent-Testable Consensus` - 4 edges
10. `Compounding Improvements` - 4 edges

## Surprising Connections (you probably didn't know these)
- `Semantic Layers` --conceptually_related_to--> `Agent-Testable Consensus`  [INFERRED]
  post-ai-data-stack.md → post-ai-data-stack.md  _Bridges community 1 → community 0_
- `The Shape and Feel of the Post-AI Data Stack` --references--> `Cloud Data Warehouse`  [EXTRACTED]
  post-ai-data-stack.md → post-ai-data-stack.md  _Bridges community 0 → community 3_
- `Modern Data Stack` --references--> `Reverse ETL`  [EXTRACTED]
  post-ai-data-stack.md → post-ai-data-stack.md  _Bridges community 0 → community 4_
- `Post-AI Data Stack` --conceptually_related_to--> `Agent-Readable Artifacts`  [EXTRACTED]
  post-ai-data-stack.md → post-ai-data-stack.md  _Bridges community 0 → community 2_

## Hyperedges (group relationships)
- **Cloud Data Warehouse Providers** — post_ai_data_stack_cloud_data_warehouse, post_ai_data_stack_snowflake, post_ai_data_stack_redshift, post_ai_data_stack_gcp_bigquery [EXTRACTED 1.00]
- **Post-AI Data Stack Components** — post_ai_data_stack_post_ai_data_stack, post_ai_data_stack_agent_readable_artifacts, post_ai_data_stack_agent_operable_tools, post_ai_data_stack_agent_agnostic_context, post_ai_data_stack_agent_testable_consensus, post_ai_data_stack_compounding_improvements, post_ai_data_stack_beyond_sql [EXTRACTED 1.00]
- **Evaluation Trace Pattern Flow** — post_ai_data_stack_read_domain_doc, post_ai_data_stack_view_dashboard, post_ai_data_stack_read_semantic_view, post_ai_data_stack_execute_sql, post_ai_data_stack_synthesize_answer [EXTRACTED 1.00]

## Communities (5 total, 0 thin omitted)

### Community 0 - "Data Stack Evolution"
Cohesion: 0.36
Nodes (10): Agent-Agnostic Context, The Shape and Feel of the Post-AI Data Stack, Beyond SQL, Data Science Lifecycle, Fivetran, Ian Macomber, Modern Data Stack, Post-AI Data Stack (+2 more)

### Community 1 - "Consensus & Eval Traces"
Cohesion: 0.20
Nodes (10): Agent-Testable Consensus, Compounding Improvements, Consensus Divergence Rate, EXECUTE_SQL, Failure Taxonomies, READ_DOMAIN_DOC, READ_SEMANTIC_VIEW, SYNTHESIZE_ANSWER (+2 more)

### Community 2 - "Agent Discoverability"
Cohesion: 0.50
Nodes (4): Agent-Readable Artifacts, llms.txt, SEO, Saturday Night Live (SNL) Analogy

### Community 3 - "Cloud Warehouse Vendors"
Cohesion: 0.50
Nodes (4): Cloud Data Warehouse, GCP BigQuery, Redshift, Snowflake

### Community 4 - "Agent-Operable Integration"
Cohesion: 0.67
Nodes (3): Agent-Operable Tools, Model Context Protocol (MCP), Reverse ETL

## Knowledge Gaps
- **16 isolated node(s):** `Ian Macomber`, `Snowflake`, `Redshift`, `GCP BigQuery`, `Fivetran` (+11 more)
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 16 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `Post-AI Data Stack` connect `Data Stack Evolution` to `Consensus & Eval Traces`, `Agent Discoverability`, `Agent-Operable Integration`?**
  _High betweenness centrality (0.641) - this node is a cross-community bridge._
- **Why does `Compounding Improvements` connect `Consensus & Eval Traces` to `Data Stack Evolution`?**
  _High betweenness centrality (0.384) - this node is a cross-community bridge._
- **What connects `Ian Macomber`, `Snowflake`, `Redshift` to the rest of the system?**
  _16 weakly-connected nodes found - possible documentation gaps or missing edges._

---

# Merge on 2026-09-02

# Graph Report - bedrock-learn-1788376529  (2026-09-02)

## Corpus Check
- Corpus is ~1,433 words - fits in a single context window. You may not need a graph.

## Summary
- 62 nodes · 81 edges · 6 communities
- Extraction: 96% EXTRACTED · 2% INFERRED · 1% AMBIGUOUS · INFERRED: 2 edges (avg confidence: 0.7)
- Token cost: 0 input · 98,520 output

## Community Hubs (Navigation)
- Repository & Team Identity
- Knowledge Item Data Model
- Redaction & Confidentiality
- The Interview Ritual
- Source vs. Knowledge Item Boundary
- Tag Dimensions & Taxonomy

## God Nodes (most connected - your core abstractions)
1. `GTC Knowledge Hub Collector (Repository)` - 16 edges
2. `KNOWLEDGE_ITEM (table)` - 15 edges
3. `REDACTION_LOG (table)` - 8 edges
4. `Postgres schema (owned by this repo)` - 7 edges
5. `TAG (table)` - 5 edges
6. `Source (vocabulary term / SOURCE table)` - 4 edges
7. `Interview (vocabulary term / INTERVIEW table)` - 4 edges
8. `Person (vocabulary term / PERSON table)` - 4 edges
9. `ENGAGEMENT (table)` - 4 edges
10. `Phase 3 — Draft item` - 4 edges

## Surprising Connections (you probably didn't know these)
- `Triage (vocabulary term)` --semantically_similar_to--> `Phase 3 — Draft item`  [INFERRED] [semantically similar]
  gtc-knowledge-hub-collector.md → gtc-knowledge-hub-collector.md  _Bridges community 4 → community 3_
- `GTC Knowledge Hub Collector (Repository)` --references--> `load_interview.py`  [EXTRACTED]
  gtc-knowledge-hub-collector.md → gtc-knowledge-hub-collector.md  _Bridges community 0 → community 3_
- `GTC Knowledge Hub Collector (Repository)` --references--> `data/db/seed.sql`  [EXTRACTED]
  gtc-knowledge-hub-collector.md → gtc-knowledge-hub-collector.md  _Bridges community 0 → community 4_
- `Source (vocabulary term / SOURCE table)` --shares_data_with--> `REDACTION_LOG (table)`  [EXTRACTED]
  gtc-knowledge-hub-collector.md → gtc-knowledge-hub-collector.md  _Bridges community 4 → community 2_
- `Interview (vocabulary term / INTERVIEW table)` --shares_data_with--> `KNOWLEDGE_ITEM (table)`  [EXTRACTED]
  gtc-knowledge-hub-collector.md → gtc-knowledge-hub-collector.md  _Bridges community 4 → community 1_

## Import Cycles
- None detected.

## Hyperedges (group relationships)
- **Interview Ritual — Four-Phase Flow** — gtc_knowledge_hub_collector_phase1_briefing, gtc_knowledge_hub_collector_phase2_live_interview, gtc_knowledge_hub_collector_phase3_draft_item, gtc_knowledge_hub_collector_phase4_closing [EXTRACTED 1.00]
- **ADRs Governing the Collector Schema** — gtc_knowledge_hub_collector_adr_0001, gtc_knowledge_hub_collector_adr_0002, gtc_knowledge_hub_collector_adr_0003, gtc_knowledge_hub_collector_adr_0004, gtc_knowledge_hub_collector_adr_0005 [EXTRACTED 1.00]
- **Redaction Category Taxonomy** — gtc_knowledge_hub_collector_pii_category, gtc_knowledge_hub_collector_client_identity_category, gtc_knowledge_hub_collector_commercial_category, gtc_knowledge_hub_collector_client_financial_category [EXTRACTED 1.00]

## Communities (6 total, 0 thin omitted)

### Community 0 - "Repository & Team Identity"
Cohesion: 0.19
Nodes (15): ADR 0002 — Relational Postgres for v1, approved_knowledge_item (Postgres view), Collection (system role), CONTEXT.md, Curation Screen, docs/architecture/data-model.md, Gabriel Bernardo, Groundwork (shared vocabulary) (+7 more)

### Community 1 - "Knowledge Item Data Model"
Cohesion: 0.20
Nodes (12): ADR 0003 — Client required, Engagement nullable, ADR 0005 — Knowledge Item consolidated in English, Approval status (governance mechanism), CLIENT (table), decision_record (Knowledge Item type), ENGAGEMENT (table), KNOWLEDGE_ITEM (table), lesson_learned (Knowledge Item type) (+4 more)

### Community 2 - "Redaction & Confidentiality"
Cohesion: 0.22
Nodes (10): client_financial (Redaction category), client_identity (Redaction category), commercial (Redaction category), ENGAGEMENT_PERSON (table), Person (vocabulary term / PERSON table), PERSON_ALIAS (table), pii (Redaction category), Redaction (vocabulary term) (+2 more)

### Community 3 - "The Interview Ritual"
Cohesion: 0.22
Nodes (10): Coverage limitation, Idempotent commit (governance mechanism), load_interview.py, Mandatory human confirmation (governance mechanism), Phase 1 — Briefing, Phase 2 — Live interview, Phase 3 — Draft item, Phase 4 — Closing (+2 more)

### Community 4 - "Source vs. Knowledge Item Boundary"
Cohesion: 0.25
Nodes (8): ADR 0001 — Source as briefing, not input, knowledge_item.origin = 'backfill', Freshness limitation, Interview (vocabulary term / INTERVIEW table), KNOWLEDGE_ITEM_SOURCE (table), data/db/seed.sql, Source (vocabulary term / SOURCE table), Triage (vocabulary term)

### Community 5 - "Tag Dimensions & Taxonomy"
Cohesion: 0.33
Nodes (7): ADR 0004 — technology/system dimensions kept distinct, Controlled / Proposed tag status, KNOWLEDGE_ITEM_TAG (table), methodology (Tag dimension), system (Tag dimension), TAG (table), technology (Tag dimension)

## Ambiguous Edges - Review These
- `approved_knowledge_item (Postgres view)` → `Curation Screen`  [AMBIGUOUS]
  gtc-knowledge-hub-collector.md · relation: conceptually_related_to

## Knowledge Gaps
- **17 isolated node(s):** `Gabriel Bernardo`, `Guilherme Losso`, `techindicium (GitHub organization)`, `Indicium AI 2026 Brazil Hackathon (Challenge #1)`, `Controlled / Proposed tag status` (+12 more)
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 22 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **What is the exact relationship between `approved_knowledge_item (Postgres view)` and `Curation Screen`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **Why does `KNOWLEDGE_ITEM (table)` connect `Knowledge Item Data Model` to `Redaction & Confidentiality`, `Source vs. Knowledge Item Boundary`, `Tag Dimensions & Taxonomy`?**
  _High betweenness centrality (0.667) - this node is a cross-community bridge._
- **Why does `knowledge_item.origin = 'backfill'` connect `Source vs. Knowledge Item Boundary` to `Knowledge Item Data Model`?**
  _High betweenness centrality (0.386) - this node is a cross-community bridge._
- **Why does `GTC Knowledge Hub Collector (Repository)` connect `Repository & Team Identity` to `The Interview Ritual`, `Source vs. Knowledge Item Boundary`?**
  _High betweenness centrality (0.382) - this node is a cross-community bridge._
- **What connects `Gabriel Bernardo`, `Guilherme Losso`, `techindicium (GitHub organization)` to the rest of the system?**
  _17 weakly-connected nodes found - possible documentation gaps or missing edges._

---

# Merge on 2026-09-03

# Graph Report - bedrock-learn-1788449558  (2026-09-03)

## Corpus Check
- Corpus is ~3,136 words - fits in a single context window. You may not need a graph.

## Summary
- 86 nodes · 126 edges · 8 communities
- Extraction: 92% EXTRACTED · 7% INFERRED · 1% AMBIGUOUS · INFERRED: 9 edges (avg confidence: 0.82)
- Token cost: 0 input · 113,013 output

## Community Hubs (Navigation)
- Skills, MCP & Automation
- Cowork Adoption Journey
- AITO & Value Axes
- Model Benchmarks & Security
- Portobank Skill Library
- AI Misuse & Governance
- AI Business Results
- Workshop Provenance & Partners

## God Nodes (most connected - your core abstractions)
1. `Cowork (2026)` - 16 edges
2. `Skills em Camadas (Você / Seu Time / Sua Organização)` - 11 edges
3. `Connectors` - 10 edges
4. `Três Eixos onde a IA Gera Valor` - 8 edges
5. `Índice Finance & Accounting (Artificial Analysis)` - 8 edges
6. `Segurança sob Ataque: Taxa de Sucesso de Prompt Injection` - 8 edges
7. `Skills` - 7 edges
8. `Hands-on 2: Um Relatório que se Monta Sozinho (Demo)` - 7 edges
9. `IA na Prática: Comitê Executivo` - 7 edges
10. `Mau Uso de IA no Setor Financeiro` - 6 edges

## Surprising Connections (you probably didn't know these)
- `Anthropic` --conceptually_related_to--> `Claude (AI Assistant)`  [INFERRED]
  claude-cowork-workshop-portobank.md → claude-cowork-workshop-portobank.md  _Bridges community 1 → community 7_
- `Crédito & Risco: Triagem de Alertas` --semantically_similar_to--> `/parecer-credito`  [INFERRED] [semantically similar]
  claude-cowork-workshop-portobank.md → claude-cowork-workshop-portobank.md  _Bridges community 4 → community 1_
- `O Efeito Composto` --semantically_similar_to--> `Três Eixos onde a IA Gera Valor`  [INFERRED] [semantically similar]
  claude-cowork-workshop-portobank.md → claude-cowork-workshop-portobank.md  _Bridges community 0 → community 2_
- `Context Engineering` --rationale_for--> `Cowork (2026)`  [EXTRACTED]
  claude-cowork-workshop-portobank.md → claude-cowork-workshop-portobank.md  _Bridges community 1 → community 0_
- `Skills` --rationale_for--> `Skills em Camadas (Você / Seu Time / Sua Organização)`  [EXTRACTED]
  claude-cowork-workshop-portobank.md → claude-cowork-workshop-portobank.md  _Bridges community 0 → community 4_

## Hyperedges (group relationships)
- **AITO Integra Pessoas, Processos e Produtos como Motor Único** — claude_cowork_workshop_portobank_aito, claude_cowork_workshop_portobank_workplace_transformation, claude_cowork_workshop_portobank_agentic_dev, claude_cowork_workshop_portobank_core_innovation [EXTRACTED 1.00]
- **Skills + Connectors = Plugins** — claude_cowork_workshop_portobank_skills, claude_cowork_workshop_portobank_connectors, claude_cowork_workshop_portobank_plugins [EXTRACTED 1.00]
- **Fluxo do Relatório Semanal que se Monta Sozinho** — claude_cowork_workshop_portobank_automacao_rotinas, claude_cowork_workshop_portobank_schedule_command, claude_cowork_workshop_portobank_drive_sharepoint, claude_cowork_workshop_portobank_outlook_gmail, claude_cowork_workshop_portobank_hands_on_2 [EXTRACTED 0.90]

## Communities (8 total, 0 thin omitted)

### Community 0 - "Skills, MCP & Automation"
Cohesion: 0.16
Nodes (19): Automação: Boas Práticas, Automação (Rotinas), Connectors, Context Engineering, Core Bancário (Sistema), CRM, Drive/SharePoint, O Efeito Composto (+11 more)

### Community 1 - "Cowork Adoption Journey"
Cohesion: 0.26
Nodes (13): Chat (2023), Claude (AI Assistant), Code (2025), Comercial: Registro de Reunião e Follow-up, Compliance: Resumo de Normativos BACEN/CVM, Cowork (2026), Fluxo Entender-Planejar-Executar-Verificar-Entregar, Crédito & Risco: Triagem de Alertas (+5 more)

### Community 2 - "AITO & Value Axes"
Cohesion: 0.21
Nodes (12): Agentic Dev (Eng. de Software e Claude Code), AI Transformation Office (AITO), Core Innovation (Esteira Nativa), Estratégia de Transformação (Ritmo Organizacional), Faster Processes (Processos), Smarter Employees (Pessoas), Transformação Simultânea (Agressivo), Transformação Sequenciada (Balanceado) (+4 more)

### Community 3 - "Model Benchmarks & Security"
Cohesion: 0.21
Nodes (12): Artificial Analysis, Claude Fable 5, Claude Opus 4.8, Claude Sonnet 4.6, Claude Sonnet 5, Índice Finance & Accounting (Artificial Analysis), Gemini 3.5 Flash, Gemini 3.6 Flash (+4 more)

### Community 4 - "Portobank Skill Library"
Cohesion: 0.18
Nodes (11): /analise-carteira, /brand-portobank, /conciliacao-contabil, /normativos-bacen, /parecer-credito, /portobank-slides, /prep-comite, /rascunho-email (+3 more)

### Community 5 - "AI Misuse & Governance"
Cohesion: 0.24
Nodes (10): AI Washing, Deepfake de William Bonner (Golpe Resgata Brasil), Delphia, Febraban, Global Predictions, Governança, Mau Uso de IA no Setor Financeiro, Polícia Federal (+2 more)

### Community 6 - "AI Business Results"
Cohesion: 0.40
Nodes (5): Pitchmaker (Investbank), Portfólio IA · Novos Negócios, Refinanciamento (REFF WhatsApp), SDR no WhatsApp (Consórcio LH), Venda Autônoma (CLT Consignado)

### Community 7 - "Workshop Provenance & Partners"
Cohesion: 0.67
Nodes (4): Anthropic, Claude Sonnet 5 System Card, IA na Prática: Comitê Executivo, IndiciumAI

## Ambiguous Edges - Review These
- `Gemini 3.6 Flash` → `Gemini 3.5 Flash`  [AMBIGUOUS]
  claude-cowork-workshop-portobank.md · relation: conceptually_related_to

## Knowledge Gaps
- **25 isolated node(s):** `/prep-comite`, `/rascunho-email`, `/resumo-hangout`, `/analise-carteira`, `/conciliacao-contabil` (+20 more)
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 27 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **What is the exact relationship between `Gemini 3.6 Flash` and `Gemini 3.5 Flash`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **Why does `Governança` connect `AI Misuse & Governance` to `Skills, MCP & Automation`, `Model Benchmarks & Security`, `Workshop Provenance & Partners`?**
  _High betweenness centrality (0.371) - this node is a cross-community bridge._
- **Why does `IA na Prática: Comitê Executivo` connect `Workshop Provenance & Partners` to `Skills, MCP & Automation`, `Cowork Adoption Journey`, `AITO & Value Axes`, `AI Misuse & Governance`?**
  _High betweenness centrality (0.347) - this node is a cross-community bridge._
- **Why does `Três Eixos onde a IA Gera Valor` connect `AITO & Value Axes` to `Skills, MCP & Automation`, `Cowork Adoption Journey`, `Workshop Provenance & Partners`?**
  _High betweenness centrality (0.243) - this node is a cross-community bridge._
- **What connects `/prep-comite`, `/rascunho-email`, `/resumo-hangout` to the rest of the system?**
  _25 weakly-connected nodes found - possible documentation gaps or missing edges._

---

# Merge on 2026-09-09

# Graph Report - bedrock-learn-1788959326  (2026-09-09)

## Corpus Check
- Corpus is ~427 words - fits in a single context window. You may not need a graph.

## Summary
- 20 nodes · 27 edges · 4 communities
- Extraction: 78% EXTRACTED · 22% INFERRED · 0% AMBIGUOUS · INFERRED: 6 edges (avg confidence: 0.75)
- Token cost: 0 input · 65,042 output

## Community Hubs (Navigation)
- Model & Data Governance
- Agent Reasoning & Memory
- Applications & Tools Layer
- Observability, Security & Discoverability

## God Nodes (most connected - your core abstractions)
1. `Agents Layer` - 8 edges
2. `Cross-Layer Concerns` - 7 edges
3. `Three Core Service Categories` - 5 edges
4. `Agentic AI Architecture in the Enterprise` - 4 edges
5. `Knowledge Bases Component` - 4 edges
6. `Applications Layer` - 3 edges
7. `Model Access Component` - 3 edges
8. `Tools Component` - 3 edges
9. `Generative AI End-User Applications` - 2 edges
10. `Non-GenAI Applications` - 2 edges

## Surprising Connections (you probably didn't know these)
- `Generative AI End-User Applications` --conceptually_related_to--> `Agents Layer`  [INFERRED]
  enterprise-architecture.md → enterprise-architecture.md  _Bridges community 2 → community 1_
- `Model Access Component` --conceptually_related_to--> `Cross-Layer Concerns`  [INFERRED]
  enterprise-architecture.md → enterprise-architecture.md  _Bridges community 0 → community 3_
- `Tools Component` --conceptually_related_to--> `Cross-Layer Concerns`  [INFERRED]
  enterprise-architecture.md → enterprise-architecture.md  _Bridges community 2 → community 3_
- `Agentic AI Architecture in the Enterprise` --references--> `Three Core Service Categories`  [EXTRACTED]
  enterprise-architecture.md → enterprise-architecture.md  _Bridges community 2 → community 0_
- `Agents Layer` --references--> `Discoverability`  [EXTRACTED]
  enterprise-architecture.md → enterprise-architecture.md  _Bridges community 1 → community 3_

## Hyperedges (group relationships)
- **Three Core Service Categories (Model Access, Tools, Knowledge Bases)** — tmp_bedrock_learn_1788959326_enterprise_architecture_model_access_component, tmp_bedrock_learn_1788959326_enterprise_architecture_tools_component, tmp_bedrock_learn_1788959326_enterprise_architecture_knowledge_bases_component [EXTRACTED 1.00]
- **Cross-Layer Concerns (Observability, Security, Discoverability)** — tmp_bedrock_learn_1788959326_enterprise_architecture_cross_layer_concerns, tmp_bedrock_learn_1788959326_enterprise_architecture_observability, tmp_bedrock_learn_1788959326_enterprise_architecture_security, tmp_bedrock_learn_1788959326_enterprise_architecture_discoverability [EXTRACTED 1.00]

## Communities (4 total, 0 thin omitted)

### Community 0 - "Model & Data Governance"
Cohesion: 0.40
Nodes (6): Guardrails (Safety Measures), Knowledge Bases Component, Model Access Component, Retrieval-Augmented Generation (RAG), Role-Based Access Control (RBAC), Three Core Service Categories

### Community 1 - "Agent Reasoning & Memory"
Cohesion: 0.40
Nodes (5): Agent-to-Agent Communication and Orchestration, Agents Layer, Large Language Model (LLM), Long-Term Memory (Agent Insights), Short-Term Memory (Agent Conversations)

### Community 2 - "Applications & Tools Layer"
Cohesion: 0.40
Nodes (5): Applications Layer, Generative AI End-User Applications, Non-GenAI Applications, Agentic AI Architecture in the Enterprise, Tools Component

### Community 3 - "Observability, Security & Discoverability"
Cohesion: 0.50
Nodes (4): Cross-Layer Concerns, Discoverability, Observability, Security

## Knowledge Gaps
- **7 isolated node(s):** `Retrieval-Augmented Generation (RAG)`, `Agent-to-Agent Communication and Orchestration`, `Short-Term Memory (Agent Conversations)`, `Long-Term Memory (Agent Insights)`, `Observability` (+2 more)
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 7 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `Agents Layer` connect `Agent Reasoning & Memory` to `Model & Data Governance`, `Applications & Tools Layer`, `Observability, Security & Discoverability`?**
  _High betweenness centrality (0.457) - this node is a cross-community bridge._
- **Why does `Cross-Layer Concerns` connect `Observability, Security & Discoverability` to `Model & Data Governance`, `Applications & Tools Layer`?**
  _High betweenness centrality (0.318) - this node is a cross-community bridge._
- **Why does `Three Core Service Categories` connect `Model & Data Governance` to `Agent Reasoning & Memory`, `Applications & Tools Layer`?**
  _High betweenness centrality (0.285) - this node is a cross-community bridge._
- **Are the 3 inferred relationships involving `Cross-Layer Concerns` (e.g. with `Knowledge Bases Component` and `Model Access Component`) actually correct?**
  _`Cross-Layer Concerns` has 3 INFERRED edges - model-reasoned connections that need verification._
- **What connects `Retrieval-Augmented Generation (RAG)`, `Agent-to-Agent Communication and Orchestration`, `Short-Term Memory (Agent Conversations)` to the rest of the system?**
  _7 weakly-connected nodes found - possible documentation gaps or missing edges._

---

# Merge on 2026-09-10

# Graph Report - bedrock-learn-1789041903  (2026-09-10)

## Corpus Check
- Corpus is ~1,735 words - fits in a single context window. You may not need a graph.

## Summary
- 24 nodes · 30 edges · 4 communities
- Extraction: 90% EXTRACTED · 10% INFERRED · 0% AMBIGUOUS · INFERRED: 3 edges (avg confidence: 0.78)
- Token cost: 0 input · 61,115 output

## Community Hubs (Navigation)
- Continuous & Security Testing
- Author & Industry Affiliations
- Shift-Left Testing Fundamentals
- Cost-of-Defect Research

## God Nodes (most connected - your core abstractions)
1. `Shift-Left Testing` - 9 edges
2. `Arthur Hicken` - 6 edges
3. `The Shift-Left Approach to Software Testing` - 4 edges
4. `Coding Standards` - 4 edges
5. `Service Virtualization` - 4 edges
6. `Security Testing` - 4 edges
7. `Capers Jones Cost-of-Defect Graph` - 3 edges
8. `Static Code Analysis` - 3 edges
9. `Unit Testing` - 3 edges
10. `Software Testing Pyramid` - 2 edges

## Surprising Connections (you probably didn't know these)
- `The Shift-Left Approach to Software Testing` --references--> `Arthur Hicken`  [EXTRACTED]
  shift-left-approach-software-testing.md → shift-left-approach-software-testing.md  _Bridges community 3 → community 1_
- `The Shift-Left Approach to Software Testing` --conceptually_related_to--> `Shift-Left Testing`  [EXTRACTED]
  shift-left-approach-software-testing.md → shift-left-approach-software-testing.md  _Bridges community 3 → community 2_
- `Shift-Left Testing` --conceptually_related_to--> `Coding Standards`  [EXTRACTED]
  shift-left-approach-software-testing.md → shift-left-approach-software-testing.md  _Bridges community 2 → community 0_

## Hyperedges (group relationships)
- **Core Shift-Left Development Practices** — shift_left_approach_software_testing_static_code_analysis, shift_left_approach_software_testing_unit_testing, shift_left_approach_software_testing_coding_standards, shift_left_approach_software_testing_service_virtualization [INFERRED 0.85]
- **Testing Types Enabled by Service Virtualization** — shift_left_approach_software_testing_service_virtualization, shift_left_approach_software_testing_continuous_testing, shift_left_approach_software_testing_performance_testing, shift_left_approach_software_testing_security_testing [INFERRED 0.85]

## Communities (4 total, 0 thin omitted)

### Community 0 - "Continuous & Security Testing"
Cohesion: 0.38
Nodes (7): Coding Standards, Continuous Testing, GDPR, Performance Testing, Build Security In, Not Test It In (Secure by Design), Security Testing, Service Virtualization

### Community 1 - "Author & Industry Affiliations"
Cohesion: 0.33
Nodes (6): Arthur Hicken, Cisco, Motorola, Parasoft, The Code Curmudgeon (blog), Vanguard

### Community 2 - "Shift-Left Testing Fundamentals"
Cohesion: 0.47
Nodes (6): Avoid Overloading Developers With Testing Burden, Goal Is Fewer Bugs Introduced, Not Just More Bugs Found, Shift-Left Testing, Software Testing Pyramid, Static Code Analysis, Unit Testing

### Community 3 - "Cost-of-Defect Research"
Cohesion: 0.40
Nodes (5): Capers Jones, Cost of Defect Remediation Escalates the Later It Is Found, Capers Jones Cost-of-Defect Graph, DevOps, The Shift-Left Approach to Software Testing

## Knowledge Gaps
- **8 isolated node(s):** `Capers Jones`, `Continuous Testing`, `Parasoft`, `The Code Curmudgeon (blog)`, `Cisco` (+3 more)
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 10 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `Shift-Left Testing` connect `Shift-Left Testing Fundamentals` to `Continuous & Security Testing`, `Cost-of-Defect Research`?**
  _High betweenness centrality (0.694) - this node is a cross-community bridge._
- **Why does `The Shift-Left Approach to Software Testing` connect `Cost-of-Defect Research` to `Author & Industry Affiliations`, `Shift-Left Testing Fundamentals`?**
  _High betweenness centrality (0.518) - this node is a cross-community bridge._
- **Why does `Arthur Hicken` connect `Author & Industry Affiliations` to `Cost-of-Defect Research`?**
  _High betweenness centrality (0.395) - this node is a cross-community bridge._
- **What connects `Capers Jones`, `Continuous Testing`, `Parasoft` to the rest of the system?**
  _8 weakly-connected nodes found - possible documentation gaps or missing edges._