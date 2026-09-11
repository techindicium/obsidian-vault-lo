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

---

# Merge on 2026-09-10

# Graph Report - bedrock-learn-nist-1789043300  (2026-09-10)

## Corpus Check
- Corpus is ~16,028 words - fits in a single context window. You may not need a graph.

## Summary
- 43 nodes · 98 edges · 6 communities
- Extraction: 93% EXTRACTED · 6% INFERRED · 1% AMBIGUOUS · INFERRED: 6 edges (avg confidence: 0.78)
- Token cost: 0 input · 135,039 output

## Community Hubs (Navigation)
- Trustworthy AI Characteristics
- AI Actor Roles & Stakeholders
- AI RMF Core Functions
- AI RMF Profiles & Risk Framing
- AI Lifecycle Stages
- Related NIST/Security Frameworks

## God Nodes (most connected - your core abstractions)
1. `NIST AI Risk Management Framework (AI RMF 1.0)` - 13 edges
2. `AI Actor` - 13 edges
3. `MAP Function` - 8 edges
4. `Trustworthy AI` - 8 edges
5. `Valid and Reliable` - 8 edges
6. `GOVERN Function` - 7 edges
7. `Secure and Resilient` - 7 edges
8. `Accountable and Transparent` - 7 edges
9. `AI Lifecycle Dimensions` - 7 edges
10. `MEASURE Function` - 6 edges

## Surprising Connections (you probably didn't know these)
- `AI RMF Profile` --conceptually_related_to--> `AI Lifecycle Dimensions`  [AMBIGUOUS]
  NIST.AI.100-1.md → NIST.AI.100-1.md  _Bridges community 3 → community 4_
- `MEASURE Function` --conceptually_related_to--> `Risk Measurement`  [INFERRED]
  NIST.AI.100-1.md → NIST.AI.100-1.md  _Bridges community 2 → community 3_
- `Explainable and Interpretable` --semantically_similar_to--> `AI Risk Management and Human-AI Interaction`  [INFERRED] [semantically similar]
  NIST.AI.100-1.md → NIST.AI.100-1.md  _Bridges community 0 → community 2_
- `NIST AI Risk Management Framework (AI RMF 1.0)` --references--> `AI Actor`  [EXTRACTED]
  NIST.AI.100-1.md → NIST.AI.100-1.md  _Bridges community 3 → community 1_
- `NIST AI Risk Management Framework (AI RMF 1.0)` --references--> `How AI Risks Differ from Traditional Software Risks`  [EXTRACTED]
  NIST.AI.100-1.md → NIST.AI.100-1.md  _Bridges community 3 → community 5_

## Hyperedges (group relationships)
- **AI RMF Core Operational Cycle** — nist_ai_100_1_govern, nist_ai_100_1_map, nist_ai_100_1_measure, nist_ai_100_1_manage [EXTRACTED 1.00]
- **Trustworthy AI Characteristics** — nist_ai_100_1_valid_and_reliable, nist_ai_100_1_safe, nist_ai_100_1_secure_and_resilient, nist_ai_100_1_accountable_and_transparent, nist_ai_100_1_explainable_and_interpretable, nist_ai_100_1_privacy_enhanced, nist_ai_100_1_fair_with_harmful_bias_managed [EXTRACTED 1.00]
- **AI Actor Task Categories** — nist_ai_100_1_ai_design, nist_ai_100_1_ai_development, nist_ai_100_1_ai_deployment, nist_ai_100_1_operation_and_monitoring, nist_ai_100_1_tevv, nist_ai_100_1_human_factors, nist_ai_100_1_domain_expert [EXTRACTED 1.00]

## Communities (6 total, 0 thin omitted)

### Community 0 - "Trustworthy AI Characteristics"
Cohesion: 0.53
Nodes (10): Accountable and Transparent, Explainable and Interpretable, Fair - with Harmful Bias Managed, ISO/IEC TS 5723:2022 (Trustworthiness Vocabulary), NIST SP 1270: Towards a Standard for Identifying and Managing Bias in Artificial Intelligence, Privacy-Enhanced, Safe, Secure and Resilient (+2 more)

### Community 1 - "AI Actor Roles & Stakeholders"
Cohesion: 0.29
Nodes (8): Affected Individuals/Communities, AI Actor, Domain Expert (Actor Task Category), End Users, General Public, Human Factors (Actor Task Category), OECD Framework for the Classification of AI Systems, Third-Party Entities

### Community 2 - "AI RMF Core Functions"
Cohesion: 0.76
Nodes (7): AI RMF Core, NIST AI RMF Playbook, GOVERN Function, AI Risk Management and Human-AI Interaction, MANAGE Function, MAP Function, MEASURE Function

### Community 3 - "AI RMF Profiles & Risk Framing"
Cohesion: 0.43
Nodes (7): AI RMF Profile, Attributes of the AI RMF, NIST AI Risk Management Framework (AI RMF 1.0), ISO 31000:2018 (Risk Management), Risk Measurement, Risk Prioritization, Risk Tolerance

### Community 4 - "AI Lifecycle Stages"
Cohesion: 0.73
Nodes (6): AI Deployment (Actor Task Category), AI Design (Actor Task Category), AI Development (Actor Task Category), AI Lifecycle Dimensions, Operation and Monitoring (Actor Task Category), Test, Evaluation, Verification, and Validation (TEVV)

### Community 5 - "Related NIST/Security Frameworks"
Cohesion: 0.40
Nodes (5): How AI Risks Differ from Traditional Software Risks, NIST Cybersecurity Framework, NIST Privacy Framework, NIST Risk Management Framework, Secure Software Development Framework

## Ambiguous Edges - Review These
- `AI RMF Profile` → `AI Lifecycle Dimensions`  [AMBIGUOUS]
  NIST.AI.100-1.md · relation: conceptually_related_to

## Knowledge Gaps
- **6 isolated node(s):** `Third-Party Entities`, `Affected Individuals/Communities`, `General Public`, `Secure Software Development Framework`, `NIST SP 1270: Towards a Standard for Identifying and Managing Bias in Artificial Intelligence` (+1 more)
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 6 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **What is the exact relationship between `AI RMF Profile` and `AI Lifecycle Dimensions`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **Why does `NIST AI Risk Management Framework (AI RMF 1.0)` connect `AI RMF Profiles & Risk Framing` to `Trustworthy AI Characteristics`, `AI Actor Roles & Stakeholders`, `AI RMF Core Functions`, `AI Lifecycle Stages`, `Related NIST/Security Frameworks`?**
  _High betweenness centrality (0.629) - this node is a cross-community bridge._
- **Why does `AI Actor` connect `AI Actor Roles & Stakeholders` to `AI RMF Profiles & Risk Framing`, `AI Lifecycle Stages`?**
  _High betweenness centrality (0.378) - this node is a cross-community bridge._
- **Why does `Trustworthy AI` connect `Trustworthy AI Characteristics` to `AI RMF Profiles & Risk Framing`?**
  _High betweenness centrality (0.223) - this node is a cross-community bridge._
- **What connects `Third-Party Entities`, `Affected Individuals/Communities`, `General Public` to the rest of the system?**
  _6 weakly-connected nodes found - possible documentation gaps or missing edges._

---

# Merge on 2026-09-10

# Graph Report - bedrock-learn-aisvs-1789044700  (2026-09-10)

## Corpus Check
- Corpus is ~23,013 words - fits in a single context window. You may not need a graph.

## Summary
- 43 nodes · 131 edges · 9 communities (6 shown, 3 thin omitted)
- Extraction: 60% EXTRACTED · 34% INFERRED · 6% AMBIGUOUS · INFERRED: 45 edges (avg confidence: 0.79)
- Token cost: 0 input · 258,484 output

## Community Hubs (Navigation)
- AI Code-Generation Supply Chain Security
- Agentic AI Runtime Security
- AISVS Framework Scope & Alignment
- Model Attack Glossary Terms
- Training Data & Model Lifecycle Provenance
- Infrastructure & Access Control
- Guardrails & Jailbreak
- Hallucination & RAG
- MCP & Trust Boundary

## God Nodes (most connected - your core abstractions)
1. `Input Validation (C2)` - 17 edges
2. `OWASP AI Security Verification Standard (AISVS)` - 13 edges
3. `Supply Chain Security for Models (C6)` - 13 edges
4. `AISVS Glossary` - 13 edges
5. `Model Lifecycle Management & Change Control (C3)` - 12 edges
6. `Orchestration & Agentic Security` - 12 edges
7. `AI Security Controls Inventory` - 12 edges
8. `Adversarial Robustness` - 11 edges
9. `Model Behavior, Output Control & Safety Assurance` - 10 edges
10. `Training Data Integrity & Traceability (C1)` - 9 edges

## Surprising Connections (you probably didn't know these)
- `Training Data Integrity & Traceability (C1)` --semantically_similar_to--> `Supply Chain Security for Models (C6)`  [INFERRED] [semantically similar]
  AISVS/0x10-C01-Training-Data-Integrity-and-Traceability.md → AISVS/0x10-C06-Supply-Chain.md
- `Input Validation (C2)` --semantically_similar_to--> `Access Control & Identity for AI Components & Users (C5)`  [INFERRED] [semantically similar]
  AISVS/0x10-C02-Input-Validation.md → AISVS/0x10-C05-Access-Control-and-Identity.md
- `Input Validation (C2)` --references--> `Adversarial Robustness`  [AMBIGUOUS]
  AISVS/0x10-C02-Input-Validation.md → AISVS/0x10-C11-Adversarial-Robustness.md
- `Input Validation (C2)` --references--> `Model Context Protocol (MCP) Security`  [AMBIGUOUS]
  AISVS/0x10-C02-Input-Validation.md → AISVS/0x10-C10-MCP-Security.md
- `Input Validation (C2)` --references--> `Model Behavior, Output Control & Safety Assurance`  [AMBIGUOUS]
  AISVS/0x10-C02-Input-Validation.md → AISVS/0x10-C07-Model-Behavior.md

## Hyperedges (group relationships)
- **AISVS Core Control Categories (C1-C6)** — aisvs_training_data_integrity_and_traceability, aisvs_input_validation, aisvs_model_lifecycle_management, aisvs_infrastructure, aisvs_access_control_and_identity, aisvs_supply_chain [EXTRACTED 1.00]
- **Model Artifact Trust Chain** — aisvs_model_lifecycle_management, aisvs_infrastructure, aisvs_supply_chain [INFERRED 0.85]
- **AI Isolation & Access Boundary Controls** — aisvs_access_control_and_identity, aisvs_infrastructure, aisvs_model_lifecycle_management [INFERRED 0.75]
- **Agentic AI Control Stack** — aisvs_orchestration_and_agentic_action, aisvs_mcp_security, aisvs_model_behavior [INFERRED 0.85]
- **Data Poisoning Defense Lifecycle** — aisvs_memory_embeddings_and_vector_database, aisvs_adversarial_robustness, aisvs_monitoring_and_logging [INFERRED 0.75]
- **Hallucination Detection Lifecycle** — aisvs_model_behavior, aisvs_memory_embeddings_and_vector_database, aisvs_monitoring_and_logging [INFERRED 0.75]
- **Prompt Injection & Safety Bypass Pattern** — aisvs_prompt_injection, aisvs_indirect_prompt_injection, aisvs_jailbreak, aisvs_guardrails [INFERRED 0.75]
- **Agentic Autonomy Risk Pattern** — aisvs_agentic_ai, aisvs_excessive_agency, aisvs_mcp [INFERRED 0.75]
- **AI for Code Generation Guidance Structure** — aisvs_ai_for_code_generation, aisvs_ai_code_review_bot_hardening, aisvs_cicd_hardening_ai_augmentation, aisvs_adversarial_ai_inbound_contributions, aisvs_ai_artifact_provenance [EXTRACTED 1.00]

## Communities (9 total, 3 thin omitted)

### Community 0 - "AI Code-Generation Supply Chain Security"
Cohesion: 0.39
Nodes (9): Adversarial AI Detection in Inbound Contributions, AI Artifact Origin Validation & Audit Trail, AI for Code Generation (Security Guidance), CI/CD Pipeline Hardening for AI Augmentation, Indirect Prompt Injection, Input Validation (C2), OWASP GenAI Security Project / LLM Top 10, Prompt Injection (+1 more)

### Community 1 - "Agentic AI Runtime Security"
Cohesion: 0.69
Nodes (9): Adversarial Robustness, AI Code-Review & Assistant Bot Hardening, AI Security Controls Inventory, Model Context Protocol (MCP) Security, Memory, Embeddings & Vector Database Security, Model Behavior, Output Control & Safety Assurance, Model Context Protocol (MCP), Monitoring, Logging & Anomaly Detection (+1 more)

### Community 2 - "AISVS Framework Scope & Alignment"
Cohesion: 0.53
Nodes (6): Appendix B: AI Security Controls Inventory, OWASP Application Security Verification Standard (ASVS), Alignment of AISVS Levels with ASVS Levels, OWASP AI Security Verification Standard (AISVS), ISO/IEC 42001:2023 AI Management System, Scope of AISVS (AI-specific narrow scope)

### Community 3 - "Model Attack Glossary Terms"
Cohesion: 0.50
Nodes (5): Adversarial Example, Agent / Agentic AI, Excessive Agency, AISVS Glossary, Model Extraction

### Community 4 - "Training Data & Model Lifecycle Provenance"
Cohesion: 0.60
Nodes (5): Data Poisoning, MITRE ATLAS, Model Lifecycle Management & Change Control (C3), NIST AI Risk Management Framework, Training Data Integrity & Traceability (C1)

### Community 5 - "Infrastructure & Access Control"
Cohesion: 1.00
Nodes (3): Access Control & Identity for AI Components & Users (C5), Infrastructure, Configuration & Deployment Security (C4), AISVS Verification Levels (L1/L2/L3)

## Ambiguous Edges - Review These
- `Input Validation (C2)` → `Adversarial Robustness`  [AMBIGUOUS]
  AISVS/0x03-Using-AISVS.md · relation: references
- `Input Validation (C2)` → `Model Context Protocol (MCP) Security`  [AMBIGUOUS]
  AISVS/0x03-Using-AISVS.md · relation: references
- `Input Validation (C2)` → `Model Behavior, Output Control & Safety Assurance`  [AMBIGUOUS]
  AISVS/0x03-Using-AISVS.md · relation: references
- `Input Validation (C2)` → `Model Lifecycle Management & Change Control (C3)`  [AMBIGUOUS]
  AISVS/0x10-C03-Model-Lifecycle-Management.md · relation: conceptually_related_to
- `Input Validation (C2)` → `Monitoring, Logging & Anomaly Detection`  [AMBIGUOUS]
  AISVS/0x03-Using-AISVS.md · relation: references
- `Input Validation (C2)` → `Orchestration & Agentic Security`  [AMBIGUOUS]
  AISVS/0x03-Using-AISVS.md · relation: references
- `Memory, Embeddings & Vector Database Security` → `Model Context Protocol (MCP) Security`  [AMBIGUOUS]
  AISVS/0x10-C08-Memory-Embeddings-and-Vector-Database.md · relation: conceptually_related_to
- `Model Context Protocol (MCP) Security` → `Adversarial Robustness`  [AMBIGUOUS]
  AISVS/0x10-C11-Adversarial-Robustness.md · relation: conceptually_related_to

## Knowledge Gaps
- **1 isolated node(s):** `Appendix B: AI Security Controls Inventory`
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 1 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)
- **3 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **What is the exact relationship between `Input Validation (C2)` and `Adversarial Robustness`?**
  _Edge tagged AMBIGUOUS (relation: references) - confidence is low._
- **What is the exact relationship between `Input Validation (C2)` and `Model Context Protocol (MCP) Security`?**
  _Edge tagged AMBIGUOUS (relation: references) - confidence is low._
- **What is the exact relationship between `Input Validation (C2)` and `Model Behavior, Output Control & Safety Assurance`?**
  _Edge tagged AMBIGUOUS (relation: references) - confidence is low._
- **What is the exact relationship between `Input Validation (C2)` and `Model Lifecycle Management & Change Control (C3)`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **What is the exact relationship between `Input Validation (C2)` and `Monitoring, Logging & Anomaly Detection`?**
  _Edge tagged AMBIGUOUS (relation: references) - confidence is low._
- **What is the exact relationship between `Input Validation (C2)` and `Orchestration & Agentic Security`?**
  _Edge tagged AMBIGUOUS (relation: references) - confidence is low._
- **What is the exact relationship between `Memory, Embeddings & Vector Database Security` and `Model Context Protocol (MCP) Security`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._

---

# Merge on 2026-09-10

# Graph Report - bedrock-learn-genai-1789050000  (2026-09-10)

## Corpus Check
- Corpus is ~28,041 words - fits in a single context window. You may not need a graph.

## Summary
- 23 nodes · 145 edges · 4 communities
- Extraction: 91% EXTRACTED · 8% INFERRED · 1% AMBIGUOUS · INFERRED: 12 edges (avg confidence: 0.68)
- Token cost: 0 input · 225,763 output

## Community Hubs (Navigation)
- Core Risks & Methodology
- Supply Chain & Retrieval Poisoning
- Output & Context Integrity
- Framework Mappings

## God Nodes (most connected - your core abstractions)
1. `LLM01:2026 Prompt Injection` - 20 edges
2. `LLM04:2026 Supply Chain` - 19 edges
3. `LLM03:2026 Excessive Agency` - 18 edges
4. `LLM02:2026 Sensitive Information Disclosure` - 17 edges
5. `LLM08: Hidden Context Exposure` - 16 edges
6. `LLM09: Vector and Embedding Weaknesses` - 16 edges
7. `LLM07: Misinformation` - 15 edges
8. `LLM05: Data and Model Poisoning` - 14 edges
9. `LLM06: Unbounded Consumption` - 14 edges
10. `LLM10: Improper Output Handling` - 13 edges

## Surprising Connections (you probably didn't know these)
- `LLM08: Hidden Context Exposure` --semantically_similar_to--> `LLM09: Vector and Embedding Weaknesses`  [INFERRED] [semantically similar]
  GenAI-LLM-Top10/LLM08_HiddenContextExposure.md → GenAI-LLM-Top10/LLM09_VectorAndEmbeddingWeaknesses.md
- `LLM01:2026 Prompt Injection` --semantically_similar_to--> `LLM04:2026 Supply Chain`  [INFERRED] [semantically similar]
  GenAI-LLM-Top10/LLM01_PromptInjection.md → GenAI-LLM-Top10/LLM04_SupplyChain.md
- `LLM07: Misinformation` --conceptually_related_to--> `LLM01:2026 Prompt Injection`  [INFERRED]
  GenAI-LLM-Top10/LLM07_Misinformation.md → GenAI-LLM-Top10/LLM01_PromptInjection.md
- `LLM02:2026 Sensitive Information Disclosure` --semantically_similar_to--> `LLM04:2026 Supply Chain`  [INFERRED] [semantically similar]
  GenAI-LLM-Top10/LLM02_SensitiveInformationDisclosure.md → GenAI-LLM-Top10/LLM04_SupplyChain.md
- `LLM09: Vector and Embedding Weaknesses` --shares_data_with--> `LLM02:2026 Sensitive Information Disclosure`  [INFERRED]
  GenAI-LLM-Top10/LLM09_VectorAndEmbeddingWeaknesses.md → GenAI-LLM-Top10/LLM02_SensitiveInformationDisclosure.md

## Hyperedges (group relationships)
- **Lethal Trifecta: Untrusted Input + Private Data + External Action** — genai_top10_llm01_prompt_injection, genai_top10_llm02_sensitive_information_disclosure, genai_top10_llm03_excessive_agency [INFERRED 0.85]
- **Agentic Tool-Chain Compromise via Injection, Agency, and Supply Chain** — genai_top10_llm01_prompt_injection, genai_top10_llm03_excessive_agency, genai_top10_llm04_supply_chain [INFERRED 0.85]
- **Poisoned Model and Data Supply Chain** — genai_top10_llm05_data_model_poisoning, genai_top10_llm04_supply_chain, genai_top10_llm09_vector_and_embedding_weaknesses [INFERRED 0.75]
- **Agentic Tool Abuse and Resource/Privilege Escalation** — genai_top10_llm06_unbounded_consumption, genai_top10_llm03_excessive_agency, genai_top10_llm10_improper_output_handling [INFERRED 0.65]
- **Hidden Context Disclosure Amplifying Adjacent Risks** — genai_top10_llm08_hidden_context_exposure, genai_top10_llm01_prompt_injection, genai_top10_llm02_sensitive_information_disclosure, genai_top10_llm03_excessive_agency, genai_top10_llm10_improper_output_handling [EXTRACTED 1.00]
- **All 10 LLM risks primary-mapped to MITRE ATLAS** — genai_top10_llm01_prompt_injection, genai_top10_llm02_sensitive_information_disclosure, genai_top10_llm03_excessive_agency, genai_top10_llm04_supply_chain, genai_top10_llm05_data_model_poisoning, genai_top10_llm06_unbounded_consumption, genai_top10_llm07_misinformation, genai_top10_llm08_hidden_context_exposure, genai_top10_llm09_vector_and_embedding_weaknesses, genai_top10_llm10_improper_output_handling, genai_top10_mitre_atlas_ref [INFERRED 0.85]
- **LLM risks with primary OWASP AIVSS scoring relevance** — genai_top10_llm01_prompt_injection, genai_top10_llm03_excessive_agency, genai_top10_llm07_misinformation, genai_top10_owasp_aivss_ref [INFERRED 0.85]
- **LLM risks with only supporting (not primary) MITRE ATT&CK mapping** — genai_top10_llm05_data_model_poisoning, genai_top10_llm07_misinformation, genai_top10_llm08_hidden_context_exposure, genai_top10_llm09_vector_and_embedding_weaknesses, genai_top10_mitre_attack_ref [INFERRED 0.75]

## Communities (4 total, 0 thin omitted)

### Community 0 - "Core Risks & Methodology"
Cohesion: 0.82
Nodes (8): OWASP Top 10 for LLM Applications and Generative AI (2026), OWASP GenAI Data Security 2026 (DSGAI), LLM01:2026 Prompt Injection, LLM02:2026 Sensitive Information Disclosure, LLM03:2026 Excessive Agency, LLM04:2026 Supply Chain, 2026 Evidence-Weighted Ranking Methodology, MITRE ATT&CK

### Community 1 - "Supply Chain & Retrieval Poisoning"
Cohesion: 0.73
Nodes (6): OWASP AISVS Mapping, OWASP Top 10 for Agentic Applications (ASI) 2026, LLM05: Data and Model Poisoning, LLM06: Unbounded Consumption, LLM09: Vector and Embedding Weaknesses, MITRE CWE (Common Weakness Enumeration)

### Community 2 - "Output & Context Integrity"
Cohesion: 0.80
Nodes (6): CSA AI Controls Matrix (AICM), LLM07: Misinformation, LLM08: Hidden Context Exposure, LLM10: Improper Output Handling, MITRE ATLAS, NIST AI 600-1 (Generative AI Profile)

### Community 3 - "Framework Mappings"
Cohesion: 0.67
Nodes (3): Appendix A: Related Framework Mappings, NIST AI RMF (AI 100-1), OWASP AIVSS (AI Vulnerability Scoring System)

## Ambiguous Edges - Review These
- `LLM07: Misinformation` → `LLM08: Hidden Context Exposure`  [AMBIGUOUS]
  GenAI-LLM-Top10/LLM07_Misinformation.md · relation: conceptually_related_to

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **What is the exact relationship between `LLM07: Misinformation` and `LLM08: Hidden Context Exposure`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **Why does `LLM01:2026 Prompt Injection` connect `Core Risks & Methodology` to `Supply Chain & Retrieval Poisoning`, `Output & Context Integrity`, `Framework Mappings`?**
  _High betweenness centrality (0.068) - this node is a cross-community bridge._
- **Why does `LLM04:2026 Supply Chain` connect `Core Risks & Methodology` to `Supply Chain & Retrieval Poisoning`, `Output & Context Integrity`, `Framework Mappings`?**
  _High betweenness centrality (0.061) - this node is a cross-community bridge._
- **Why does `LLM03:2026 Excessive Agency` connect `Core Risks & Methodology` to `Supply Chain & Retrieval Poisoning`, `Output & Context Integrity`, `Framework Mappings`?**
  _High betweenness centrality (0.057) - this node is a cross-community bridge._
- **Are the 2 inferred relationships involving `LLM01:2026 Prompt Injection` (e.g. with `LLM04:2026 Supply Chain` and `LLM07: Misinformation`) actually correct?**
  _`LLM01:2026 Prompt Injection` has 2 INFERRED edges - model-reasoned connections that need verification._
- **Are the 4 inferred relationships involving `LLM04:2026 Supply Chain` (e.g. with `LLM01:2026 Prompt Injection` and `LLM02:2026 Sensitive Information Disclosure`) actually correct?**
  _`LLM04:2026 Supply Chain` has 4 INFERRED edges - model-reasoned connections that need verification._
- **Are the 3 inferred relationships involving `LLM03:2026 Excessive Agency` (e.g. with `LLM02:2026 Sensitive Information Disclosure` and `LLM04:2026 Supply Chain`) actually correct?**
  _`LLM03:2026 Excessive Agency` has 3 INFERRED edges - model-reasoned connections that need verification._

---

# Merge on 2026-09-10

# Graph Report - bedrock-learn-1789076127  (2026-09-10)

## Corpus Check
- Corpus is ~14,701 words - fits in a single context window. You may not need a graph.

## Summary
- 80 nodes · 212 edges · 9 communities
- Extraction: 94% EXTRACTED · 5% INFERRED · 1% AMBIGUOUS · INFERRED: 10 edges (avg confidence: 0.82)
- Token cost: 0 input · 179,868 output

## Community Hubs (Navigation)
- AI Vendors & Guardrails
- AI-native SDLC Squad
- Platform / AI Hub Team
- Nelson Novaes Neto & Security Research
- Knowledge Workers Squad
- Assessment & Project 5x
- Paulo Pituba Negotiation Profile
- AITO Governance Office
- Enablement Squad

## God Nodes (most connected - your core abstractions)
1. `[C6] KickOff Interno — Transcrição Comentada` - 55 edges
2. `Jornada de Transformação AI — Kick-off Interno (deck)` - 49 edges
3. `Nelson Novaes Neto` - 15 edges
4. `Perfil Estratégico — Nelson Novaes Neto` - 14 edges
5. `C6 Bank` - 13 edges
6. `Plataforma / C6 AI Hub` - 12 edges
7. `Projeto de Transformação AI C6` - 11 edges
8. `Esteira AI-nativa (redesenho do SDLC)` - 11 edges
9. `Notas Rápidas (Scratch) — C6` - 10 edges
10. `Manual de Bordo - C6` - 10 edges

## Surprising Connections (you probably didn't know these)
- `Paulo Pituba` --conceptually_related_to--> `Daniel Avancini`  [AMBIGUOUS]
  c6/people_profile/perfil-paulo-pituba.md → c6/meeting_and_notes/2026-09-08-kickoff-interno-transcricao.md
- `Secure-by-Design AI (framework, 10 perguntas)` --semantically_similar_to--> `AITO (AI Transformation Office)`  [INFERRED] [semantically similar]
  c6/people_profile/perfil-nelson-novaes-neto.md → c6/project_docs/kickoff-interno-transformacao-ai-set2026.md
- `[C6] KickOff Interno — Transcrição Comentada` --references--> `C6 Assistant`  [EXTRACTED]
  c6/meeting_and_notes/2026-09-08-kickoff-interno-transcricao.md → c6/project_docs/kickoff-interno-transformacao-ai-set2026.md
- `[C6] KickOff Interno — Transcrição Comentada` --references--> `Eduardo Scarpellini (Platform Head, C6)`  [INFERRED]
  c6/meeting_and_notes/2026-09-08-kickoff-interno-transcricao.md → c6/project_docs/kickoff-interno-transformacao-ai-set2026.md
- `[C6] KickOff Interno — Transcrição Comentada` --references--> `Gustavo Torres ("GT", CIO C6)`  [EXTRACTED]
  c6/meeting_and_notes/2026-09-08-kickoff-interno-transcricao.md → c6/project_docs/kickoff-interno-transformacao-ai-set2026.md

## Hyperedges (group relationships)
- **Seis Frentes / Cinco Squads do Projeto C6** — c6_project_docs_kickoff_interno_transformacao_ai_set2026_aito, c6_project_docs_kickoff_interno_transformacao_ai_set2026_esteira_ai_nativa, c6_project_docs_kickoff_interno_transformacao_ai_set2026_knowledge_workers, c6_project_docs_kickoff_interno_transformacao_ai_set2026_plataforma_c6_ai_hub, c6_project_docs_kickoff_interno_transformacao_ai_set2026_enablement, c6_project_docs_kickoff_interno_transformacao_ai_set2026_assessment [INFERRED 0.85]
- **Estratégia de Negociação Tática para Stakeholders C6 (Never Split the Difference)** — c6_people_profile_perfil_nelson_novaes_neto_nelson_novaes_neto, c6_people_profile_perfil_paulo_pituba_paulo_pituba, c6_people_profile_perfil_nelson_novaes_neto_never_split_the_difference [INFERRED 0.80]
- **Licenças de IA já Adquiridas pelo C6 (Kiro, Claude, Gemini)** — c6_project_docs_kickoff_interno_transformacao_ai_set2026_kiro, c6_project_docs_kickoff_interno_transformacao_ai_set2026_claude, c6_project_docs_kickoff_interno_transformacao_ai_set2026_gemini, c6_project_docs_kickoff_interno_transformacao_ai_set2026_c6_bank [INFERRED 0.75]

## Communities (9 total, 0 thin omitted)

### Community 0 - "AI Vendors & Guardrails"
Cohesion: 0.21
Nodes (16): Notas Rápidas (Scratch) — C6, Repositório Oficial Indicium dentro do C6 (meta), Anthropic, AWS, C6 Bank, Claude, Gemini, Google (+8 more)

### Community 1 - "AI-native SDLC Squad"
Cohesion: 0.22
Nodes (13): Aluízio Cidral Júnior, Cristiano Pisin ("Cris"), Filipe Duarte, Guilherme Zanotelli dos Santos, Lorena Sales Santos, Natália Kauatoto, Thiago Ribeiro, Jornada de Transformação AI — Kick-off Interno (deck) (+5 more)

### Community 2 - "Platform / AI Hub Team"
Cohesion: 0.20
Nodes (12): LightLLM / "Light" (hub de modelos inspirado no Nubank), Lucas Zanotelli dos Santos, Marco Zoada, Nubank, Rodrigo Freitas Encáua, Terraform (IaC sendo substituído), Vagner Strapasson, Eduardo Scarpellini (Platform Head, C6) (+4 more)

### Community 3 - "Nelson Novaes Neto & Security Research"
Cohesion: 0.36
Nodes (12): Perfil LinkedIn — Nelson Novaes Neto (dados brutos), Perfil Estratégico — Nelson Novaes Neto, A Case Study of the Capital One Data Breach (2020), Cultura "Csixer" / Hexágono de valores C6, Cybersecurity Culture at C6 Bank (MIT CAMS case study, 2020), An Executive Guide to Secure-by-Design AI (2025, JISSEC), Developing a Global Data Breach Database and the Challenges Encountered (2021), Itaú Unibanco (+4 more)

### Community 4 - "Knowledge Workers Squad"
Cohesion: 0.25
Nodes (11): [C6] KickOff Interno — Transcrição Comentada, CIT (consultoria concorrente), Douglas Sgrott, Fabio Gomes de Oliveira, Gabriel Bernardo, Gabriel Eckschmidt Buso, Gabriel Klock, Isadora Busch (+3 more)

### Community 5 - "Assessment & Project 5x"
Cohesion: 0.40
Nodes (5): Igor Benincá, Leandro Ciscar, Projeto "5x" (projeto irmão interno), Assessment, Projeto de Transformação AI C6

### Community 6 - "Paulo Pituba Negotiation Profile"
Cohesion: 0.50
Nodes (5): Never Split the Difference (Chris Voss, framework de negociação), Perfil Estratégico — Paulo Pituba, Paulo Pituba, Rede (adquirência, grupo Itaú), CNV (Comunicação Não-Violenta)

### Community 7 - "AITO Governance Office"
Cohesion: 0.67
Nodes (3): Alberto Tadashi Yamamoto, Daniel Avancini, AITO (AI Transformation Office)

### Community 8 - "Enablement Squad"
Cohesion: 0.67
Nodes (3): Pedro Ferraresi, Tabi Thuler Santos, Enablement

## Ambiguous Edges - Review These
- `Daniel Avancini` → `Paulo Pituba`  [AMBIGUOUS]
  c6/people_profile/perfil-paulo-pituba.md · relation: conceptually_related_to
- `Marco Zoada` → `Marcos Wada (Architecture Specialist, C6)`  [AMBIGUOUS]
  c6/meeting_and_notes/2026-09-08-kickoff-interno-transcricao.md · relation: conceptually_related_to

## Knowledge Gaps
- **7 isolated node(s):** `Fabio Gomes de Oliveira`, `Gabriel Bernardo`, `Marcel (AI Head, C6)`, `Gabriel Klock`, `Matheus Dellagnelo` (+2 more)
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 7 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **What is the exact relationship between `Daniel Avancini` and `Paulo Pituba`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **What is the exact relationship between `Marco Zoada` and `Marcos Wada (Architecture Specialist, C6)`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **Why does `[C6] KickOff Interno — Transcrição Comentada` connect `Knowledge Workers Squad` to `AI Vendors & Guardrails`, `AI-native SDLC Squad`, `Platform / AI Hub Team`, `Nelson Novaes Neto & Security Research`, `Assessment & Project 5x`, `Paulo Pituba Negotiation Profile`, `AITO Governance Office`, `Enablement Squad`?**
  _High betweenness centrality (0.468) - this node is a cross-community bridge._
- **Why does `Jornada de Transformação AI — Kick-off Interno (deck)` connect `AI-native SDLC Squad` to `AI Vendors & Guardrails`, `Platform / AI Hub Team`, `Nelson Novaes Neto & Security Research`, `Knowledge Workers Squad`, `Assessment & Project 5x`, `Paulo Pituba Negotiation Profile`, `AITO Governance Office`, `Enablement Squad`?**
  _High betweenness centrality (0.336) - this node is a cross-community bridge._
- **Why does `Nelson Novaes Neto` connect `Nelson Novaes Neto & Security Research` to `AI Vendors & Guardrails`, `AI-native SDLC Squad`, `Knowledge Workers Squad`, `Paulo Pituba Negotiation Profile`?**
  _High betweenness centrality (0.170) - this node is a cross-community bridge._
- **Are the 2 inferred relationships involving `Jornada de Transformação AI — Kick-off Interno (deck)` (e.g. with `Cristiano Pisin ("Cris")` and `Natália Kauatoto`) actually correct?**
  _`Jornada de Transformação AI — Kick-off Interno (deck)` has 2 INFERRED edges - model-reasoned connections that need verification._
- **What connects `Fabio Gomes de Oliveira`, `Gabriel Bernardo`, `Marcel (AI Head, C6)` to the rest of the system?**
  _7 weakly-connected nodes found - possible documentation gaps or missing edges._

---

# Merge on 2026-09-11

# Graph Report - bedrock-learn-deck-16493  (2026-09-11)

## Corpus Check
- Corpus is ~2,395 words - fits in a single context window. You may not need a graph.

## Summary
- 63 nodes · 110 edges · 8 communities
- Extraction: 89% EXTRACTED · 10% INFERRED · 1% AMBIGUOUS · INFERRED: 11 edges (avg confidence: 0.8)
- Token cost: 0 input · 95,361 output

## Community Hubs (Navigation)
- AITO Governance & Cross-Workstream
- Project Objectives & Key Results
- Esteira AI-Nativa Squad
- C6 Bank History & Leadership
- Plataforma / C6 AI Hub Team
- Indicium Team & Contract Origin
- Contract & Manual de Bordo
- Knowledge Workers & AI Licenses

## God Nodes (most connected - your core abstractions)
1. `C6 Bank` - 20 edges
2. `Indicium` - 17 edges
3. `Plataforma (frente)` - 16 edges
4. `Esteira AI-nativa` - 14 edges
5. `Jornada de Transformação AI (C6/Indicium)` - 11 edges
6. `AITO (governança e portfólio)` - 11 edges
7. `Knowledge Workers (frente)` - 9 edges
8. `Objetivos do Projeto` - 6 edges
9. `Assessment (frente)` - 5 edges
10. `Enablement (frente)` - 4 edges

## Surprising Connections (you probably didn't know these)
- `Acelerar a Produtividade (Pessoas)` --conceptually_related_to--> `Esteira AI-nativa`  [INFERRED]
  kickoff-interno-transformacao-ai-set2026.md → kickoff-interno-transformacao-ai-set2026.md  _Bridges community 2 → community 1_
- `Acelerar a Produtividade (Pessoas)` --conceptually_related_to--> `Knowledge Workers (frente)`  [INFERRED]
  kickoff-interno-transformacao-ai-set2026.md → kickoff-interno-transformacao-ai-set2026.md  _Bridges community 7 → community 1_
- `Escalar com Sustentabilidade` --conceptually_related_to--> `Plataforma (frente)`  [INFERRED]
  kickoff-interno-transformacao-ai-set2026.md → kickoff-interno-transformacao-ai-set2026.md  _Bridges community 4 → community 1_
- `Produtos AI-Native (Produtos)` --conceptually_related_to--> `Valor em Produtos (KR)`  [INFERRED]
  kickoff-interno-transformacao-ai-set2026.md → kickoff-interno-transformacao-ai-set2026.md  _Bridges community 0 → community 1_
- `Jornada de Transformação AI (C6/Indicium)` --conceptually_related_to--> `AITO (governança e portfólio)`  [EXTRACTED]
  kickoff-interno-transformacao-ai-set2026.md → kickoff-interno-transformacao-ai-set2026.md  _Bridges community 6 → community 0_

## Hyperedges (group relationships)
- **Frentes de Atuação do Projeto** — kickoff_interno_transformacao_ai_set2026_assessment, kickoff_interno_transformacao_ai_set2026_esteira_ai_nativa, kickoff_interno_transformacao_ai_set2026_knowledge_workers, kickoff_interno_transformacao_ai_set2026_aito, kickoff_interno_transformacao_ai_set2026_plataforma, kickoff_interno_transformacao_ai_set2026_enablement [EXTRACTED 1.00]
- **Cadência de Governança com o C6** — kickoff_interno_transformacao_ai_set2026_aito, kickoff_interno_transformacao_ai_set2026_plataforma, kickoff_interno_transformacao_ai_set2026_enablement, kickoff_interno_transformacao_ai_set2026_assessment [EXTRACTED 1.00]
- **Squad Plat. Eng. AI SDLC V2** — kickoff_interno_transformacao_ai_set2026_vagner_strapasson, kickoff_interno_transformacao_ai_set2026_alberto_tadashi, kickoff_interno_transformacao_ai_set2026_daniel_avancini, kickoff_interno_transformacao_ai_set2026_leandro_ciscar, kickoff_interno_transformacao_ai_set2026_igor_beninca [EXTRACTED 1.00]

## Communities (8 total, 0 thin omitted)

### Community 0 - "AITO Governance & Cross-Workstream"
Cohesion: 0.27
Nodes (10): AITO (governança e portfólio), Assessment (frente), C6 Assistant, Enablement (frente), Governança e Cadência de Rituais com o C6, Governança e Cadência de Rituais - Interno, Gustavo Torres (GT) (AI Head), Marcel (+2 more)

### Community 1 - "Project Objectives & Key Results"
Cohesion: 0.25
Nodes (9): Acelerar a Produtividade (Pessoas), Aumentar Eficiência (Processos), Escalar com Sustentabilidade, Garantir Governança (AITO), Objetivos do Projeto, Produtividade Imediata (KR), Redução de Custo Operacional (KR), Resultados-Chave Estratégicos (+1 more)

### Community 2 - "Esteira AI-Nativa Squad"
Cohesion: 0.25
Nodes (8): Alberto Tadashi (Plat. Eng. AI SDLC V2), Daniel Avancini (Plat. Eng. AI SDLC V2), Esteira AI-nativa, Guilherme Zanotelli (Consultant Development), Igor Benincá (Plat. Eng. AI SDLC V2), Leandro Ciscar (Plat. Eng. AI SDLC V2), Lorena Sales (Consultant Product), Vagner Strapasson (Plat. Eng. AI SDLC V2)

### Community 3 - "C6 Bank History & Leadership"
Cohesion: 0.25
Nodes (8): BTG Pactual, C6 Bank, C6 Graphene, JPMorgan, Marcelo Kalim (CEO C6), Natalia Kawatoko, Paulo Pituba (PP), Thiago Ribeiro

### Community 4 - "Plataforma / C6 AI Hub Team"
Cohesion: 0.25
Nodes (8): C6 AI Hub, Cristiano Piccin, Eduardo Scarpellini (Platform Tech Lead), Everson Tavares (Platform Specialist), Marcelo Arakaki, Marcos Wada (Architecture Specialist), Nelson Neto, Plataforma (frente)

### Community 5 - "Indicium Team & Contract Origin"
Cohesion: 0.29
Nodes (7): Aluizio Júnior (FDE SDLC Lead), Filipe Duarte (AI Engineer), Indicium, Lucas Santos (Platform Engineer Lead), Matheus Dellagnelo, Rodrigo Encáua (SecOps Security), Tabi Santos (Consultant Change Mgt.)

### Community 6 - "Contract & Manual de Bordo"
Cohesion: 0.29
Nodes (7): Contrato C6-Indicium, Jornada de Transformação AI (C6/Indicium), Manual de Bordo - C6, Onboarding e Infraestrutura, Os 3 Não Negociáveis, Próximos Passos (Ações Internas), Workshop Claude Code (São Paulo)

### Community 7 - "Knowledge Workers & AI Licenses"
Cohesion: 0.33
Nodes (6): Douglas Sgrott (AI Engineer), Gabriel Buso (Consultant Processes), Isadora Busch (Consultant Product), Knowledge Workers (frente), Licenças de IA (900 Kiro, 200 Claude, 100 Gemini), Rafael Ribeiro (FDE Knowledge Lead)

## Ambiguous Edges - Review These
- `AITO (governança e portfólio)` → `Marcel`  [AMBIGUOUS]
  kickoff-interno-transformacao-ai-set2026.md · relation: references

## Knowledge Gaps
- **12 isolated node(s):** `Workshop Claude Code (São Paulo)`, `Matheus Dellagnelo`, `Marcelo Kalim (CEO C6)`, `JPMorgan`, `BTG Pactual` (+7 more)
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 13 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **What is the exact relationship between `AITO (governança e portfólio)` and `Marcel`?**
  _Edge tagged AMBIGUOUS (relation: references) - confidence is low._
- **Why does `C6 Bank` connect `C6 Bank History & Leadership` to `AITO Governance & Cross-Workstream`, `Plataforma / C6 AI Hub Team`, `Indicium Team & Contract Origin`, `Contract & Manual de Bordo`, `Knowledge Workers & AI Licenses`?**
  _High betweenness centrality (0.283) - this node is a cross-community bridge._
- **Why does `Jornada de Transformação AI (C6/Indicium)` connect `Contract & Manual de Bordo` to `AITO Governance & Cross-Workstream`, `Project Objectives & Key Results`, `Esteira AI-Nativa Squad`, `Plataforma / C6 AI Hub Team`, `Knowledge Workers & AI Licenses`?**
  _High betweenness centrality (0.277) - this node is a cross-community bridge._
- **Why does `Esteira AI-nativa` connect `Esteira AI-Nativa Squad` to `AITO Governance & Cross-Workstream`, `Project Objectives & Key Results`, `Indicium Team & Contract Origin`, `Contract & Manual de Bordo`, `Knowledge Workers & AI Licenses`?**
  _High betweenness centrality (0.229) - this node is a cross-community bridge._
- **Are the 2 inferred relationships involving `Jornada de Transformação AI (C6/Indicium)` (e.g. with `Onboarding e Infraestrutura` and `Próximos Passos (Ações Internas)`) actually correct?**
  _`Jornada de Transformação AI (C6/Indicium)` has 2 INFERRED edges - model-reasoned connections that need verification._
- **What connects `Workshop Claude Code (São Paulo)`, `Matheus Dellagnelo`, `Marcelo Kalim (CEO C6)` to the rest of the system?**
  _12 weakly-connected nodes found - possible documentation gaps or missing edges._

---

# Merge on 2026-09-11

# Graph Report - bedrock-learn-transcript-1  (2026-09-11)

## Corpus Check
- Corpus is ~17,379 words - fits in a single context window. You may not need a graph.

## Summary
- 84 nodes · 112 edges · 8 communities
- Extraction: 85% EXTRACTED · 12% INFERRED · 3% AMBIGUOUS · INFERRED: 14 edges (avg confidence: 0.74)
- Token cost: 0 input · 141,360 output

## Community Hubs (Navigation)
- Contract Origin & Commercial Choice
- Plataforma & Model Hub Tooling
- AITO/Enablement & DLP Governance
- Esteira AI-Nativa & Coding Agents
- Internal Next Steps & Action Items
- Assessment Cases & AI Assistants
- Knowledge Works & Sabotage Risk
- C6 Bank Leadership & Core Banking

## God Nodes (most connected - your core abstractions)
1. `C6 AI Transformation Project` - 17 edges
2. `C6 Bank` - 10 edges
3. `Frente Esteira AI-Nativa (SDLC)` - 9 edges
4. `Leandro Ciscar` - 8 edges
5. `Kiro` - 8 edges
6. `Indicium` - 7 edges
7. `Alberto Tadashi Yamamoto` - 6 edges
8. `Daniel Avancini` - 6 edges
9. `Frente Knowledge Works` - 6 edges
10. `Frente AITO (AI Transformation Office)` - 6 edges

## Surprising Connections (you probably didn't know these)
- `Frente Assessment` --shares_data_with--> `Frente Esteira AI-Nativa (SDLC)`  [INFERRED]
  kickoff-interno-transcricao-raw.md → kickoff-interno-transcricao-raw.md  _Bridges community 5 → community 3_
- `Frente Esteira AI-Nativa (SDLC)` --semantically_similar_to--> `Why C6 Needs Infra Migration Urgency`  [INFERRED] [semantically similar]
  kickoff-interno-transcricao-raw.md → kickoff-interno-transcricao-raw.md  _Bridges community 3 → community 0_
- `Synthetic Workers Concept` --conceptually_related_to--> `Frente Esteira AI-Nativa (SDLC)`  [INFERRED]
  kickoff-interno-transcricao-raw.md → kickoff-interno-transcricao-raw.md  _Bridges community 3 → community 2_
- `Frente Plataforma` --shares_data_with--> `Frente AITO (AI Transformation Office)`  [INFERRED]
  kickoff-interno-transcricao-raw.md → kickoff-interno-transcricao-raw.md  _Bridges community 2 → community 1_
- `Telemetria Project (Gemini/GCP)` --shares_data_with--> `C6 AI Hub`  [INFERRED]
  kickoff-interno-transcricao-raw.md → kickoff-interno-transcricao-raw.md  _Bridges community 1 → community 5_

## Hyperedges (group relationships)
- **Six Workstreams of C6 AI Transformation** — kickoff_interno_transcricao_raw_frente_assessment, kickoff_interno_transcricao_raw_frente_esteira_ai_nativa, kickoff_interno_transcricao_raw_frente_knowledge_works, kickoff_interno_transcricao_raw_frente_aito, kickoff_interno_transcricao_raw_frente_plataforma, kickoff_interno_transcricao_raw_frente_enablement, kickoff_interno_transcricao_raw_c6_ai_transformation_project [EXTRACTED 1.00]
- **Kiro vs Claude Security/Telemetry Debate** — kickoff_interno_transcricao_raw_kiro, kickoff_interno_transcricao_raw_claude_tool, kickoff_interno_transcricao_raw_rodrigo_freitas_encaua, kickoff_interno_transcricao_raw_igor_beninca, kickoff_interno_transcricao_raw_guilherme_zanotelli_dos_santos [EXTRACTED 1.00]
- **DLP Data Sovereignty Discussion** — kickoff_interno_transcricao_raw_rationale_dlp_data_restriction_rule, kickoff_interno_transcricao_raw_gabriel_bernardo, kickoff_interno_transcricao_raw_alberto_tadashi_yamamoto, kickoff_interno_transcricao_raw_c6_bank, kickoff_interno_transcricao_raw_rationale_vm_access_discarded [EXTRACTED 1.00]

## Communities (8 total, 0 thin omitted)

### Community 0 - "Contract Origin & Commercial Choice"
Cohesion: 0.17
Nodes (16): Anthropic, C6 AI Transformation Project, CIT, Cristiano Pisin (Cris), Daniel Avancini, Fabio Gomes de Oliveira, 5x Project (Parallel Indicium Project), Gabriel Klock (+8 more)

### Community 1 - "Plataforma & Model Hub Tooling"
Cohesion: 0.17
Nodes (13): Action: Research LightLLM, C6 AI Hub, Eduardo (Platform Tech Lead), Frente Plataforma, Grafana, Kubernetes, LightLLM, Lucas Zanotelli dos Santos (+5 more)

### Community 2 - "AITO/Enablement & DLP Governance"
Cohesion: 0.20
Nodes (12): Action: Ship Physical Equipment to C6, Alberto Tadashi Yamamoto, Frente AITO (AI Transformation Office), Frente Enablement, Gabriel Bernardo, JP Morgan, Manual de Bordo (Code of Conduct), Pedro Guilherme Volpato Ferraresi (+4 more)

### Community 3 - "Esteira AI-Nativa & Coding Agents"
Cohesion: 0.21
Nodes (12): Action: Re-test Kiro vs Claude, Aluizio Cidral Júnior, AWS, Claude, Filipe Duarte da Rocha Paço, Frente Esteira AI-Nativa (SDLC), Guilherme Zanotelli dos Santos, Igor Benincá (+4 more)

### Community 4 - "Internal Next Steps & Action Items"
Cohesion: 0.25
Nodes (8): Action: Contact Natália Kauatoto on Change Management, Action: Create Slack Channel for C6 Team, Action: Define Team Name, Action: Schedule Biweekly Squad Meetings, Action: Share Conduct Manual, Leandro Ciscar, Natália Kauatoto, Slack

### Community 5 - "Assessment Cases & AI Assistants"
Cohesion: 0.25
Nodes (8): C6 Assistant, Contestação de Despesas Use Case, Frente Assessment, GCP, Gemini, Marcelo (Head de IA, C6 Assistant), Revisão de Documentos Jurídicos Use Case, Telemetria Project (Gemini/GCP)

### Community 6 - "Knowledge Works & Sabotage Risk"
Cohesion: 0.29
Nodes (8): Douglas Sgrott, Frente Knowledge Works, Gabriel Eckschmidt Buso, Isadora Busch, Nelson, Rafael Ribeiro, Internal Sabotage / Resistance Risk, Shadow AI Risk

### Community 7 - "C6 Bank Leadership & Core Banking"
Cohesion: 0.29
Nodes (7): BTG Pactual, C6 Bank, Docket, GT (CIO, C6), Marcelo Calim, Matera, Paulo Pituba (PP)

## Ambiguous Edges - Review These
- `Gabriel Klock` → `C6 AI Transformation Project`  [AMBIGUOUS]
  kickoff-interno-transcricao-raw.md · relation: conceptually_related_to
- `Nelson` → `Internal Sabotage / Resistance Risk`  [AMBIGUOUS]
  kickoff-interno-transcricao-raw.md · relation: conceptually_related_to
- `LightLLM` → `Unnamed Terraform Replacement Tool (C6 IaC)`  [AMBIGUOUS]
  kickoff-interno-transcricao-raw.md · relation: shares_data_with

## Knowledge Gaps
- **37 isolated node(s):** `Fabio Gomes de Oliveira`, `Vagner Strapasson`, `Douglas Sgrott`, `Rafael Ribeiro`, `Isadora Busch` (+32 more)
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 37 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **What is the exact relationship between `Gabriel Klock` and `C6 AI Transformation Project`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **What is the exact relationship between `Nelson` and `Internal Sabotage / Resistance Risk`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **What is the exact relationship between `LightLLM` and `Unnamed Terraform Replacement Tool (C6 IaC)`?**
  _Edge tagged AMBIGUOUS (relation: shares_data_with) - confidence is low._
- **Why does `C6 AI Transformation Project` connect `Contract Origin & Commercial Choice` to `AITO/Enablement & DLP Governance`, `Esteira AI-Nativa & Coding Agents`, `Internal Next Steps & Action Items`, `C6 Bank Leadership & Core Banking`?**
  _High betweenness centrality (0.393) - this node is a cross-community bridge._
- **Why does `Frente AITO (AI Transformation Office)` connect `AITO/Enablement & DLP Governance` to `Plataforma & Model Hub Tooling`, `Internal Next Steps & Action Items`, `Knowledge Works & Sabotage Risk`?**
  _High betweenness centrality (0.240) - this node is a cross-community bridge._
- **Why does `C6 Bank` connect `C6 Bank Leadership & Core Banking` to `Contract Origin & Commercial Choice`, `AITO/Enablement & DLP Governance`, `Assessment Cases & AI Assistants`, `Knowledge Works & Sabotage Risk`?**
  _High betweenness centrality (0.237) - this node is a cross-community bridge._
- **Are the 3 inferred relationships involving `Frente Esteira AI-Nativa (SDLC)` (e.g. with `Frente Assessment` and `Why C6 Needs Infra Migration Urgency`) actually correct?**
  _`Frente Esteira AI-Nativa (SDLC)` has 3 INFERRED edges - model-reasoned connections that need verification._