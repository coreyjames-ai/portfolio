# The Pipeline Foreman

**For a data team lead who needs a new processing job by Thursday.**

Canonical: https://coreyjames.ai/agents/roles/pipeline-foreman/  
Author: Corey James · Published: 2026-11-11 · Kind: agent role  

## The story

The agent generates the skeleton of the job so that only the business logic is left to write. It checks that the job builds, waits for a person to approve the restart and runs a harmless test through it. Once the job is in service the agent starts it, follows it and recovers it, and adds or removes workers as the backlog moves.

## Function

[Infrastructure and operations](https://coreyjames.ai/agents/functions/infrastructure-and-operations/): Machines, queues, databases and spend, watched through the night.

## The crew

The specialists behind this role, grouped by the kind of work they do.

### Does the work

- [Internal Automation Builder](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/internal-automation-builder) · [page](https://coreyjames.ai/agents/specialists/internal-automation-builder/): You describe a recurring data job in plain words, and this agent designs it, sets up the database pieces, writes the code, checks it against the team's rules and switches it on.

### Runs infrastructure

- [Data Job Builder](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/data-job-builder) · [page](https://coreyjames.ai/agents/specialists/data-job-builder/): Generates the full skeleton of a new processing job so the only thing left to write is the business logic, checks that it builds, waits for a person to approve the restart, runs a harmless test job through it, and opens a merge request.
- [Service Function Builder](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/service-function-builder) · [page](https://coreyjames.ai/agents/specialists/service-function-builder/): Plans a new data-processing function, prepares its database work queue, generates its files, registers it as a tool and runs a harmless smoke test through it.
- [Job Dispatcher](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/job-dispatcher) · [page](https://coreyjames.ai/agents/specialists/job-dispatcher/): This agent starts, follows and recovers processing jobs across every automated job the team owns, and reports their status on request.
- [Worker Fleet Scaler](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/worker-fleet-scaler) · [page](https://coreyjames.ai/agents/specialists/worker-fleet-scaler/): This agent adds or removes background workers as the backlog grows and shrinks, restarts stuck ones and clears out dead connections.
- [Self-Starting Job Scheduler](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/self-starting-job-scheduler) · [page](https://coreyjames.ai/agents/specialists/self-starting-job-scheduler/): This agent turns a job into a standing service that starts itself when work piles up or on a schedule, and lets you list or stop those services at any time.
- [Batch Job Controller](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/batch-job-controller) · [page](https://coreyjames.ai/agents/specialists/batch-job-controller/): Runs a large job on a local card or a rented one, pauses, scales or stops it mid-flight, turns a one-off job into an always-on service, and isolates a job that misbehaves.
- [Database Traffic Controller](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/database-traffic-controller) · [page](https://coreyjames.ai/agents/specialists/database-traffic-controller/): Keeps heavy bulk writes from flattening the database: it prices each write by its expected load, lets cheap work through, holds heavy work until there is room, and tunes the write workers.
- [Smoke Test Runner](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/smoke-test-runner) · [page](https://coreyjames.ai/agents/specialists/smoke-test-runner/): Sends a small harmless batch through the service, once or on a trigger, and confirms it came out the other end.

### Audits and guards

- [Launch Pre-flight Checker](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/launch-pre-flight-checker) · [page](https://coreyjames.ai/agents/specialists/launch-pre-flight-checker/): Checks the machine image, the settings and the budget before a job starts, and names what is wrong while fixing it is still free.

## The engineering behind this role

- [A human at the privileged step](https://coreyjames.ai/ideas/a-human-at-the-privileged-step/): Idea
- [Tools that build tools, under governance](https://coreyjames.ai/stories/tools-that-build-tools-under-governance/): Engineering story
- [A write path that sizes itself](https://coreyjames.ai/stories/a-write-path-that-sizes-itself/): Engineering story

## Citation

Corey James. "The Pipeline Foreman." coreyjames.ai, 2026. https://coreyjames.ai/agents/roles/pipeline-foreman/

```bibtex
@misc{coreyjames-agent-role-pipeline-foreman,
  author = {Corey James},
  title = {The Pipeline Foreman},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/roles/pipeline-foreman/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/pipeline-foreman}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
