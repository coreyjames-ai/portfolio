# The Knowledge Gardener

**For the owner of a large knowledge base that grows every day.**

Canonical: https://coreyjames.ai/agents/roles/knowledge-gardener/  
Author: Corey James · Published: 2026-11-11 · Kind: agent role  

## The story

Each proposed entry is tested against the existing topics and accepted, held or rejected. The agent scores every topic's health and reports the ones that have drifted. Where some topics are overcrowded, it proposes which entries to move and shows the plan as a dry run. New material is embedded so it can be searched, and old stored versions are cleared.

## Function

[Knowledge and memory](https://coreyjames.ai/agents/functions/knowledge-and-memory/): What the team learned, kept searchable and handed to every new worker.

## The crew

The specialists behind this role, grouped by the kind of work they do.

### Keeps knowledge

- [Knowledge Rebalancer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/knowledge-rebalancer) · [page](https://coreyjames.ai/agents/specialists/knowledge-rebalancer/): Finds the overcrowded topics, proposes which entries to move at a cautious, balanced or aggressive setting, and shows the plan as a dry run before anything moves.
- [Vector Library Curator](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/vector-library-curator) · [page](https://coreyjames.ai/agents/specialists/vector-library-curator/): Keeps a large searchable collection healthy: it embeds new material, rebuilds and checks the search indexes, scores how well each topic cluster hangs together on the GPU, accepts or rejects new clusters, rebalances crowded ones, and retires stale index files.
- [Knowledge Base Maintainer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/knowledge-base-maintainer) · [page](https://coreyjames.ai/agents/specialists/knowledge-base-maintainer/): This agent runs the regular upkeep jobs: screening new entries, rebalancing between related topics, refreshing embeddings and rebuilding the search index.

### Runs infrastructure

- [Embedding Backlog Clerk](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/embedding-backlog-clerk) · [page](https://coreyjames.ai/agents/specialists/embedding-backlog-clerk/): Finds the collections with material waiting to be embedded, queues the work and starts the workers.
- [Storage Space Reclaimer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/storage-space-reclaimer) · [page](https://coreyjames.ai/agents/specialists/storage-space-reclaimer/): Lists the old stored versions, confirms which one is active and clears the ones no longer needed.
- [Embedding Migration Operator](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/embedding-migration-operator) · [page](https://coreyjames.ai/agents/specialists/embedding-migration-operator/): Rebuilds the search vectors for a whole index or for all engineering notes, in bulk on a GPU or one item at a time on CPU.

### Audits and guards

- [Knowledge Entry Screener](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/knowledge-entry-screener) · [page](https://coreyjames.ai/agents/specialists/knowledge-entry-screener/): Tests each proposed entry against the existing topics and records an accept, hold or reject decision with the measurement behind it.
- [Knowledge Base Health Analyst](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/knowledge-base-health-analyst) · [page](https://coreyjames.ai/agents/specialists/knowledge-base-health-analyst/): This agent scores every topic on dozens of health measures and reports which topics need more depth or rebalancing.
- [Knowledge Drift Detector](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/knowledge-drift-detector) · [page](https://coreyjames.ai/agents/specialists/knowledge-drift-detector/): Runs a deeper clustering analysis on selected topics and reports those whose content has drifted from where it started.
- [Screening Rule Writer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/screening-rule-writer) · [page](https://coreyjames.ai/agents/specialists/screening-rule-writer/): Writes the rules that tighten or relax acceptance for particular topics and switches individual rules on and off.

## The engineering behind this role

- [GPU vector search and corpus analytics](https://coreyjames.ai/capabilities/gpu-vector-search-and-corpus-analytics/): Capability
- [Redistribution inside the database](https://coreyjames.ai/stories/redistribution-inside-the-database/): Engineering story
- [From health scores to decisions](https://coreyjames.ai/stories/from-health-scores-to-decisions/): Engineering story

## Citation

Corey James. "The Knowledge Gardener." coreyjames.ai, 2026. https://coreyjames.ai/agents/roles/knowledge-gardener/

```bibtex
@misc{coreyjames-agent-role-knowledge-gardener,
  author = {Corey James},
  title = {The Knowledge Gardener},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/roles/knowledge-gardener/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/knowledge-gardener}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
