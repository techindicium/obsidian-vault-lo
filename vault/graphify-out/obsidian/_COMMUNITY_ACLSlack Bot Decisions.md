---
type: community
cohesion: 0.38
members: 7
---

# ACL/Slack Bot Decisions

**Cohesion:** 0.38 - loosely connected
**Members:** 7 nodes

## Members
- [[ADR 0004 Postgres full-text search before vectors]] - rationale - gtc-knowledge-hub-agent.md
- [[ADR 0006 Slack bot as MCP client in this repo]] - rationale - gtc-knowledge-hub-agent.md
- [[ADR 0007 Self-hosted agent runtime for Slack bot]] - rationale - gtc-knowledge-hub-agent.md
- [[ADR 0009 Text search language config (portuguese to english)]] - rationale - gtc-knowledge-hub-agent.md
- [[ADR 0014 Knowledge Item Contract]] - rationale - gtc-knowledge-hub-agent.md
- [[Dormant ACL filtering model (ADR 000600070012)]] - rationale - gtc-knowledge-hub-agent.md
- [[Slack Bot (MCP client)]] - concept - gtc-knowledge-hub-agent.md

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/ACL/Slack_Bot_Decisions
SORT file.name ASC
```

## Connections to other communities
- 7 edges to [[_COMMUNITY_Repo Origin & Hackathon Context]]
- 2 edges to [[_COMMUNITY_Retrieval Interface & Quality]]
- 1 edge to [[_COMMUNITY_Repository Pattern & Sources]]

## Top bridge nodes
- [[ADR 0014 Knowledge Item Contract]] - degree 7, connects to 3 communities
- [[Slack Bot (MCP client)]] - degree 4, connects to 2 communities
- [[ADR 0006 Slack bot as MCP client in this repo]] - degree 4, connects to 1 community
- [[ADR 0007 Self-hosted agent runtime for Slack bot]] - degree 4, connects to 1 community
- [[Dormant ACL filtering model (ADR 000600070012)]] - degree 3, connects to 1 community