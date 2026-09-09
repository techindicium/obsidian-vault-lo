---
type: community
cohesion: 0.67
members: 4
---

# Interview Confirmation Workflow

**Cohesion:** 0.67 - moderately connected
**Members:** 4 nodes

## Members
- [[Approval Status (draftapprovedrejected)]] - concept - gtc-knowledge-hub-collector.md
- [[Idempotent Commit]] - rationale - gtc-knowledge-hub-collector.md
- [[Interview (vocabulary)]] - concept - gtc-knowledge-hub-collector.md
- [[Mandatory Human Confirmation]] - rationale - gtc-knowledge-hub-collector.md

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Interview_Confirmation_Workflow
SORT file.name ASC
```

## Connections to other communities
- 5 edges to [[_COMMUNITY_Redaction & English Consolidation]]
- 1 edge to [[_COMMUNITY_Tagging & Item Taxonomy]]

## Top bridge nodes
- [[Approval Status (draftapprovedrejected)]] - degree 4, connects to 2 communities
- [[Mandatory Human Confirmation]] - degree 4, connects to 1 community
- [[Idempotent Commit]] - degree 3, connects to 1 community
- [[Interview (vocabulary)]] - degree 3, connects to 1 community