# The Model Interviewer

**For a research lead who wants what a model knows in a form people can search.**

Canonical: https://coreyjames.ai/agents/roles/model-interviewer/  
Author: Corey James · Published: 2026-11-11 · Kind: agent role  

## The story

The agent questions a model at scale, organises what comes back into a structured knowledge base and audits it for gaps and errors. The same pipeline produces training data for a smaller model.

## Function

[AI and model teams](https://coreyjames.ai/agents/functions/ai-and-model-teams/): Launching, tuning and supervising models and the agents that use them.

## The crew

The specialists behind this role, grouped by the kind of work they do.

### Does the work

- [AI Model Study Runner](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/ai-model-study-runner) · [page](https://coreyjames.ai/agents/specialists/ai-model-study-runner/): This agent prepares large sets of test questions, runs them through a model in one repeatable batch, follows progress, retries failures and stores the results for study.
- [Training Data Producer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/training-data-producer) · [page](https://coreyjames.ai/agents/specialists/training-data-producer/): It writes prompts designed to draw out a model's behaviour, runs resumable collection jobs across graphics servers, and stores what it collects for training, with status and replay.
- [Model Insight Extractor](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/model-insight-extractor) · [page](https://coreyjames.ai/agents/specialists/model-insight-extractor/): Generates a large set of test prompts, runs them through the model, captures the model's internal state for each prompt, and re-runs any that failed.

### Keeps knowledge

- [Knowledge Base Builder](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/knowledge-base-builder) · [page](https://coreyjames.ai/agents/specialists/knowledge-base-builder/): This agent questions an AI model topic by topic, finds the thin areas, proposes new entries, keeps only the ones that pass a quality bar, and deepens weak topics until the knowledge base is full.
- [Knowledge Base Maintainer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/knowledge-base-maintainer) · [page](https://coreyjames.ai/agents/specialists/knowledge-base-maintainer/): This agent runs the regular upkeep jobs: screening new entries, rebalancing between related topics, refreshing embeddings and rebuilding the search index.
- [Vector Library Curator](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/vector-library-curator) · [page](https://coreyjames.ai/agents/specialists/vector-library-curator/): Keeps a large searchable collection healthy: it embeds new material, rebuilds and checks the search indexes, scores how well each topic cluster hangs together on the GPU, accepts or rejects new clusters, rebalances crowded ones, and retires stale index files.
- [Knowledge Base Curator](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/knowledge-base-curator) · [page](https://coreyjames.ai/agents/specialists/knowledge-base-curator/): It finds the thin areas of the knowledge base, writes candidate entries, admits only those that fit the existing topics, labels and rebalances the topics, and reports which areas need repair.

### Runs infrastructure

- [Search Index Manager](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/search-index-manager) · [page](https://coreyjames.ai/agents/specialists/search-index-manager/): This agent counts, builds, checks and reports on the search indexes behind semantic search.

### Audits and guards

- [Knowledge Base Auditor](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/knowledge-base-auditor) · [page](https://coreyjames.ai/agents/specialists/knowledge-base-auditor/): This agent checks that the knowledge base still lines up with its reference material and lists missing or incomplete topics for repair.
- [Knowledge Base Health Analyst](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/knowledge-base-health-analyst) · [page](https://coreyjames.ai/agents/specialists/knowledge-base-health-analyst/): This agent scores every topic on dozens of health measures and reports which topics need more depth or rebalancing.
- [Knowledge Entry Screener](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/knowledge-entry-screener) · [page](https://coreyjames.ai/agents/specialists/knowledge-entry-screener/): Tests each proposed entry against the existing topics and records an accept, hold or reject decision with the measurement behind it.

## The engineering behind this role

- [High-throughput batch inference and embeddings](https://coreyjames.ai/capabilities/high-throughput-batch-inference/): Capability
- [GPU vector search and corpus analytics](https://coreyjames.ai/capabilities/gpu-vector-search-and-corpus-analytics/): Capability
- [The workload that shaped the platform](https://coreyjames.ai/stories/the-workload-that-shaped-the-platform/): Engineering story
- [A detector for a silent corruption](https://coreyjames.ai/stories/a-detector-for-a-silent-corruption/): Engineering story

## Citation

Corey James. "The Model Interviewer." coreyjames.ai, 2026. https://coreyjames.ai/agents/roles/model-interviewer/

```bibtex
@misc{coreyjames-agent-role-model-interviewer,
  author = {Corey James},
  title = {The Model Interviewer},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/roles/model-interviewer/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/model-interviewer}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
