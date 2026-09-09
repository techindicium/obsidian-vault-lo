---
type: community
cohesion: 0.40
members: 5
---

# Tagging & Item Taxonomy

**Cohesion:** 0.40 - moderately connected
**Members:** 5 nodes

## Members
- [[ADR 0003 — Knowledge Item Requires Client, Engagement Nullable]] - rationale - gtc-knowledge-hub-collector.md
- [[ADR 0004 — Technology and System as Distinct Tag Dimensions]] - rationale - gtc-knowledge-hub-collector.md
- [[Controlled  Proposed Tag Status]] - concept - gtc-knowledge-hub-collector.md
- [[Knowledge Item Types]] - concept - gtc-knowledge-hub-collector.md
- [[Tag Dimensions]] - concept - gtc-knowledge-hub-collector.md

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Tagging__Item_Taxonomy
SORT file.name ASC
```

## Connections to other communities
- 5 edges to [[_COMMUNITY_Redaction & English Consolidation]]
- 1 edge to [[_COMMUNITY_Interview Confirmation Workflow]]

## Top bridge nodes
- [[Knowledge Item Types]] - degree 4, connects to 2 communities
- [[Tag Dimensions]] - degree 4, connects to 1 community
- [[ADR 0003 — Knowledge Item Requires Client, Engagement Nullable]] - degree 2, connects to 1 community
- [[ADR 0004 — Technology and System as Distinct Tag Dimensions]] - degree 2, connects to 1 community
- [[Controlled  Proposed Tag Status]] - degree 2, connects to 1 community