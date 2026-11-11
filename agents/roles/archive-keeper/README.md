# The Archive Keeper

**For a research lead whose results must still be readable next year.**

Canonical: https://coreyjames.ai/agents/roles/archive-keeper/  
Author: Corey James · Published: 2026-11-11 · Kind: agent role  

## The story

Every large run leaves data behind, and the agent looks after it. It checks a finished run against the original request and reports whether every item is present. Stored files are re-checked for damage. When a new version of the data is built, the agent switches readers to it and keeps the previous one until the new one has been confirmed. If storage fails, it reports what was affected and what was recovered.

## Function

[AI and model teams](https://coreyjames.ai/agents/functions/ai-and-model-teams/): Launching, tuning and supervising models and the agents that use them.

## The crew

The specialists behind this role, grouped by the kind of work they do.

### Keeps knowledge

- [Research Data Archivist](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/research-data-archivist) · [page](https://coreyjames.ai/agents/specialists/research-data-archivist/): This agent manages stored research data by version: it lists what is stored, closes and activates versions, releases checkpoints and clears out old versions.
- [Run Conditions Recorder](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/run-conditions-recorder) · [page](https://coreyjames.ai/agents/specialists/run-conditions-recorder/): This agent records GPU memory and machine load around every run so results are read against the conditions they ran in.

### Runs infrastructure

- [Data Version Promoter](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/data-version-promoter) · [page](https://coreyjames.ai/agents/specialists/data-version-promoter/): Switches readers to a newly built version of stored data, finishes a build that stalled and cancels one that went wrong.
- [Storage Incident Handler](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/storage-incident-handler) · [page](https://coreyjames.ai/agents/specialists/storage-incident-handler/): When storage reports a problem, this agent reads the recovery report, runs a consistency check, sends lost items back for reprocessing and records the sign-off.
- [Storage Spend Reconciler](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/storage-spend-reconciler) · [page](https://coreyjames.ai/agents/specialists/storage-spend-reconciler/): It syncs the day's storage cost into the daily budget so tomorrow's limit reflects real spend.

### Audits and guards

- [Run Verification Clerk](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/run-verification-clerk) · [page](https://coreyjames.ai/agents/specialists/run-verification-clerk/): Checks a finished run against its original request and reports whether every item is present, without running anything again.
- [Stored Data Integrity Checker](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/stored-data-integrity-checker) · [page](https://coreyjames.ai/agents/specialists/stored-data-integrity-checker/): Re-checks that each stored data file is intact and correctly laid out, and reports any file that fails.

## The engineering behind this role

- [GPU vector search and corpus analytics](https://coreyjames.ai/capabilities/gpu-vector-search-and-corpus-analytics/): Capability
- [High-throughput batch inference and embeddings](https://coreyjames.ai/capabilities/high-throughput-batch-inference/): Capability
- [Append-only, with tombstones and lineage](https://coreyjames.ai/ideas/append-only-with-lineage/): Idea
- [Three shards that move together](https://coreyjames.ai/stories/three-shards-that-move-together/): Engineering story
- [Millions of queued items that were not there](https://coreyjames.ai/stories/millions-of-queued-items-that-were-not-there/): Engineering story

## Citation

Corey James. "The Archive Keeper." coreyjames.ai, 2026. https://coreyjames.ai/agents/roles/archive-keeper/

```bibtex
@misc{coreyjames-agent-role-archive-keeper,
  author = {Corey James},
  title = {The Archive Keeper},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/roles/archive-keeper/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/archive-keeper}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
