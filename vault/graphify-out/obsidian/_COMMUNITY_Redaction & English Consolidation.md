---
type: community
cohesion: 0.33
members: 9
---

# Redaction & English Consolidation

**Cohesion:** 0.33 - loosely connected
**Members:** 9 nodes

## Members
- [[ADR 0002 — Relational Postgres for v1]] - rationale - gtc-knowledge-hub-collector.md
- [[ADR 0005 — Knowledge Item Consolidado em Inglês]] - rationale - gtc-knowledge-hub-collector.md
- [[English-Only Knowledge Base]] - rationale - gtc-knowledge-hub-collector.md
- [[GTC Knowledge Hub — Collector]] - document - gtc-knowledge-hub-collector.md
- [[Guilherme Losso]] - concept - gtc-knowledge-hub-collector.md
- [[Person (vocabulary)]] - concept - gtc-knowledge-hub-collector.md
- [[Redaction (vocabulary)]] - concept - gtc-knowledge-hub-collector.md
- [[Redaction Categories]] - concept - gtc-knowledge-hub-collector.md
- [[Redaction Log]] - concept - gtc-knowledge-hub-collector.md

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Redaction__English_Consolidation
SORT file.name ASC
```

## Connections to other communities
- 5 edges to [[_COMMUNITY_Interview Confirmation Workflow]]
- 5 edges to [[_COMMUNITY_Tagging & Item Taxonomy]]
- 4 edges to [[_COMMUNITY_Source-to-Interview Governance]]
- 4 edges to [[_COMMUNITY_Repo Origin & Hackathon Context]]

## Top bridge nodes
- [[GTC Knowledge Hub — Collector]] - degree 25, connects to 4 communities
- [[Redaction (vocabulary)]] - degree 3, connects to 1 community