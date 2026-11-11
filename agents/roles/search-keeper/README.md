# The Search Keeper

**For a platform lead whose company relies on searching its own code and documents.**

Canonical: https://coreyjames.ai/agents/roles/search-keeper/  
Author: Corey James · Published: 2026-11-11 · Kind: agent role  

## The story

A new codebase is taken in and mapped. From then on the agent re-scans on a timer and again whenever new code lands. It removes entries for deleted files, resets an indexing job that has stalled and rebuilds everything when the model behind the search changes. The service itself is watched, restarted on request and kept licensed.

## Function

[Knowledge and memory](https://coreyjames.ai/agents/functions/knowledge-and-memory/): What the team learned, kept searchable and handed to every new worker.

## The crew

The specialists behind this role, grouped by the kind of work they do.

### Keeps knowledge

- [Codebase Intake Engineer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/codebase-intake-engineer) · [page](https://coreyjames.ai/agents/specialists/codebase-intake-engineer/): Brings a codebase in from a local folder or straight from GitHub or GitLab, recommends which file types to include, splits the code along function and type boundaries for eight languages, and makes it searchable by meaning and by name.
- [Code Map Builder](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/code-map-builder) · [page](https://coreyjames.ai/agents/specialists/code-map-builder/): Builds and maintains the dependency map: calls, imports, implementations, references, definitions and re-exports.
- [Deleted Code Cleaner](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/deleted-code-cleaner) · [page](https://coreyjames.ai/agents/specialists/deleted-code-cleaner/): Deletes the search entries and dependency links for code that no longer exists, without holding up the scan.
- [Reference Library Keeper](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/reference-library-keeper) · [page](https://coreyjames.ai/agents/specialists/reference-library-keeper/): Keeps each document collection fresh on its own schedule by re-reading only files that changed, re-summarising and re-indexing them, and retrying any sections whose summary failed.

### Runs infrastructure

- [Scheduled Index Refresher](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/scheduled-index-refresher) · [page](https://coreyjames.ai/agents/specialists/scheduled-index-refresher/): Re-scans each codebase for changes and updates its search index and dependency map, skipping a tick when another indexing job is already running.
- [Commit-Triggered Re-Indexer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/commit-triggered-re-indexer) · [page](https://coreyjames.ai/agents/specialists/commit-triggered-re-indexer/): Starts a re-index of the affected codebase as soon as new code lands and reports progress to the team lead's inbox.
- [Index Upkeep Operator](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/index-upkeep-operator) · [page](https://coreyjames.ai/agents/specialists/index-upkeep-operator/): Keeps every index matching its source.
- [Embedding Migration Operator](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/embedding-migration-operator) · [page](https://coreyjames.ai/agents/specialists/embedding-migration-operator/): Rebuilds the search vectors for a whole index or for all engineering notes, in bulk on a GPU or one item at a time on CPU.
- [Memory Service Operator](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/memory-service-operator) · [page](https://coreyjames.ai/agents/specialists/memory-service-operator/): Looks after the service day to day.
- [Search Index Manager](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/search-index-manager) · [page](https://coreyjames.ai/agents/specialists/search-index-manager/): This agent counts, builds, checks and reports on the search indexes behind semantic search.

### Audits and guards

- [Index Stall Watchdog](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/index-stall-watchdog) · [page](https://coreyjames.ai/agents/specialists/index-stall-watchdog/): Resets the stuck job so scheduled indexing carries on, and records the reset.

## The engineering behind this role

- [Memory and code intelligence for agents](https://coreyjames.ai/capabilities/memory-and-code-intelligence-for-agents/): Capability

## Citation

Corey James. "The Search Keeper." coreyjames.ai, 2026. https://coreyjames.ai/agents/roles/search-keeper/

```bibtex
@misc{coreyjames-agent-role-search-keeper,
  author = {Corey James},
  title = {The Search Keeper},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/roles/search-keeper/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/search-keeper}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
