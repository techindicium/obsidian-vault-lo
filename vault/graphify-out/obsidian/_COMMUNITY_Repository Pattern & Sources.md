---
type: community
cohesion: 0.50
members: 4
---

# Repository Pattern & Sources

**Cohesion:** 0.50 - moderately connected
**Members:** 4 nodes

## Members
- [[ADR 0005 SQLAlchemy behind a repository]] - rationale - gtc-knowledge-hub-agent.md
- [[ADR 0013 Wiki.js as a source route]] - rationale - gtc-knowledge-hub-agent.md
- [[Groundwork (shared vocabulary)]] - concept - gtc-knowledge-hub-agent.md
- [[gtc-knowledge-hub-collector]] - document - gtc-knowledge-hub-agent.md

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Repository_Pattern__Sources
SORT file.name ASC
```

## Connections to other communities
- 4 edges to [[_COMMUNITY_Repo Origin & Hackathon Context]]
- 2 edges to [[_COMMUNITY_Shared Postgres & Redaction]]
- 1 edge to [[_COMMUNITY_ACLSlack Bot Decisions]]

## Top bridge nodes
- [[gtc-knowledge-hub-collector]] - degree 6, connects to 2 communities
- [[ADR 0013 Wiki.js as a source route]] - degree 3, connects to 2 communities
- [[ADR 0005 SQLAlchemy behind a repository]] - degree 2, connects to 1 community
- [[Groundwork (shared vocabulary)]] - degree 2, connects to 1 community