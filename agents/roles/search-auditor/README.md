# The Search Auditor

**For a manager asking whether the company's memory is earning its keep.**

Canonical: https://coreyjames.ai/agents/roles/search-auditor/  
Author: Corey James · Published: 2026-11-11 · Kind: agent role  

## The story

The agent runs fixed question sets through the search and compares the answers with a baseline. It reviews how people searched recently and proposes setting changes. It checks that every note taken reached storage. Then it prices the result: what was spent creating each note against what was saved each time one was reused.

## Function

[Knowledge and memory](https://coreyjames.ai/agents/functions/knowledge-and-memory/): What the team learned, kept searchable and handed to every new worker.

## The crew

The specialists behind this role, grouped by the kind of work they do.

### Keeps knowledge

- [Search Tuning Analyst](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/search-tuning-analyst) · [page](https://coreyjames.ai/agents/specialists/search-tuning-analyst/): Reviews recent search behaviour with a language model and proposes setting changes.
- [Note Queue Reconciler](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/note-queue-reconciler) · [page](https://coreyjames.ai/agents/specialists/note-queue-reconciler/): Checks that every queued note reached storage, flags stragglers past a grace period, and records a summary.
- [Memory Return-on-Investment Reporter](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/memory-return-on-investment-reporter) · [page](https://coreyjames.ai/agents/specialists/memory-return-on-investment-reporter/): Reports the tokens spent creating each note against the tokens saved each time a note is reused or compressed, priced per model provider on per-token or flat-fee plans, and shows project-level totals on a live dashboard.

### Audits and guards

- [Search Quality Analyst](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/search-quality-analyst) · [page](https://coreyjames.ai/agents/specialists/search-quality-analyst/): Measures and tunes search quality.
- [Search Health Reporter](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/search-health-reporter) · [page](https://coreyjames.ai/agents/specialists/search-health-reporter/): Runs the search quality comparison, the cache gap count and a smoke test, and leaves a short health summary in the team lead's inbox.

## The engineering behind this role

- [Memory and code intelligence for agents](https://coreyjames.ai/capabilities/memory-and-code-intelligence-for-agents/): Capability
- [Measure the instrument](https://coreyjames.ai/ideas/measure-the-instrument/): Idea

## Citation

Corey James. "The Search Auditor." coreyjames.ai, 2026. https://coreyjames.ai/agents/roles/search-auditor/

```bibtex
@misc{coreyjames-agent-role-search-auditor,
  author = {Corey James},
  title = {The Search Auditor},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/roles/search-auditor/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/search-auditor}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
