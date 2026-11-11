# The Database Guard

**For a team whose database takes writes from many directions.**

Canonical: https://coreyjames.ai/agents/roles/database-guard/  
Author: Corey James · Published: 2026-11-11 · Kind: agent role  

## The story

The agent meters every writer so bulk loads go in only as fast as the database can take them. When pressure rises it slows the loads, and it has an emergency stop. Asked where a row came from, it traces it back to the job that wrote it.

## Function

[Infrastructure and operations](https://coreyjames.ai/agents/functions/infrastructure-and-operations/): Machines, queues, databases and spend, watched through the night.

## The crew

The specialists behind this role, grouped by the kind of work they do.

### Runs infrastructure

- [Database Traffic Controller](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/database-traffic-controller) · [page](https://coreyjames.ai/agents/specialists/database-traffic-controller/): Keeps heavy bulk writes from flattening the database: it prices each write by its expected load, lets cheap work through, holds heavy work until there is room, and tunes the write workers.
- [Write Queue Firefighter](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/write-queue-firefighter) · [page](https://coreyjames.ai/agents/specialists/write-queue-firefighter/): Takes the page when the database write queue backs up, follows the recovery procedure, drains the queue if it has to, and confirms that writes are flowing again.
- [Batch Job Controller](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/batch-job-controller) · [page](https://coreyjames.ai/agents/specialists/batch-job-controller/): Runs a large job on a local card or a rented one, pauses, scales or stops it mid-flight, turns a one-off job into an always-on service, and isolates a job that misbehaves.
- [Worker Fleet Scaler](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/worker-fleet-scaler) · [page](https://coreyjames.ai/agents/specialists/worker-fleet-scaler/): This agent adds or removes background workers as the backlog grows and shrinks, restarts stuck ones and clears out dead connections.
- [Throttle Rehearsal Analyst](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/throttle-rehearsal-analyst) · [page](https://coreyjames.ai/agents/specialists/throttle-rehearsal-analyst/): Runs a new limit in rehearsal mode, where every decision is logged and nothing is delayed, then reports which jobs would have waited before the limit is enforced.
- [Throughput Tuner](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/throughput-tuner) · [page](https://coreyjames.ai/agents/specialists/throughput-tuner/): Adjusts how work is batched and flushed, from a careful standard setting to a very high-volume one, and measures the result.
- [Stuck Job Unblocker](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/stuck-job-unblocker) · [page](https://coreyjames.ai/agents/specialists/stuck-job-unblocker/): Finds the locks left behind by dead jobs, confirms nothing live depends on them and releases them so the queue moves again.

### Audits and guards

- [Database Overload Guard](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/database-overload-guard) · [page](https://coreyjames.ai/agents/specialists/database-overload-guard/): This agent lets bulk loads into the database only as fast as the database can take them, frees stuck jobs and recommends capacity changes.
- [Data Lineage Investigator](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/data-lineage-investigator) · [page](https://coreyjames.ai/agents/specialists/data-lineage-investigator/): This agent traces a record back through every job and change that touched it and writes up the answer.
- [Stored Data Integrity Checker](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/stored-data-integrity-checker) · [page](https://coreyjames.ai/agents/specialists/stored-data-integrity-checker/): Re-checks that each stored data file is intact and correctly laid out, and reports any file that fails.

## The engineering behind this role

- [Budgets and refusals](https://coreyjames.ai/ideas/budgets-and-refusals/): Idea
- [Append-only, with tombstones and lineage](https://coreyjames.ai/ideas/append-only-with-lineage/): Idea
- [Pricing writes by what they cost the database](https://coreyjames.ai/stories/pricing-writes-by-what-they-cost/): Engineering story
- [A write path that sizes itself](https://coreyjames.ai/stories/a-write-path-that-sizes-itself/): Engineering story
- [196 deadlocks to zero](https://coreyjames.ai/stories/196-deadlocks-to-zero/): Engineering story

## Citation

Corey James. "The Database Guard." coreyjames.ai, 2026. https://coreyjames.ai/agents/roles/database-guard/

```bibtex
@misc{coreyjames-agent-role-database-guard,
  author = {Corey James},
  title = {The Database Guard},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/roles/database-guard/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/database-guard}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
