---
type: community
cohesion: 1.00
members: 2
---

# Shared Postgres & Redaction

**Cohesion:** 1.00 - tightly connected
**Members:** 2 nodes

## Members
- [[Postgres (shared Knowledge Base instance)]] - concept - gtc-knowledge-hub-agent.md
- [[redaction_log]] - concept - gtc-knowledge-hub-agent.md

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Shared_Postgres__Redaction
SORT file.name ASC
```

## Connections to other communities
- 2 edges to [[_COMMUNITY_Repo Origin & Hackathon Context]]
- 2 edges to [[_COMMUNITY_Repository Pattern & Sources]]
- 1 edge to [[_COMMUNITY_Retrieval Interface & Quality]]

## Top bridge nodes
- [[Postgres (shared Knowledge Base instance)]] - degree 4, connects to 3 communities
- [[redaction_log]] - degree 3, connects to 2 communities