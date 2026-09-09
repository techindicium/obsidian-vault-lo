---
type: community
cohesion: 0.33
members: 6
---

# Retrieval Interface & Quality

**Cohesion:** 0.33 - loosely connected
**Members:** 6 nodes

## Members
- [[ADR 0001 Thin MCP server]] - rationale - gtc-knowledge-hub-agent.md
- [[ADR 0017 Golden Set corpus]] - rationale - gtc-knowledge-hub-agent.md
- [[Golden Set]] - concept - gtc-knowledge-hub-agent.md
- [[Open governance gap approval is global, not per-reader]] - rationale - gtc-knowledge-hub-agent.md
- [[Thin MCP Server (searchget, no synthesis)]] - concept - gtc-knowledge-hub-agent.md
- [[approved_knowledge_item(_expanded) view]] - concept - gtc-knowledge-hub-agent.md

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Retrieval_Interface__Quality
SORT file.name ASC
```

## Connections to other communities
- 5 edges to [[_COMMUNITY_Repo Origin & Hackathon Context]]
- 2 edges to [[_COMMUNITY_Knowledge Item Taxonomy]]
- 2 edges to [[_COMMUNITY_ACLSlack Bot Decisions]]
- 1 edge to [[_COMMUNITY_Shared Postgres & Redaction]]

## Top bridge nodes
- [[Thin MCP Server (searchget, no synthesis)]] - degree 5, connects to 3 communities
- [[approved_knowledge_item(_expanded) view]] - degree 5, connects to 2 communities
- [[Golden Set]] - degree 4, connects to 2 communities
- [[ADR 0001 Thin MCP server]] - degree 2, connects to 1 community
- [[ADR 0017 Golden Set corpus]] - degree 2, connects to 1 community