# The Safe Change Desk

**For an operations lead who has to change a live system on a weekday.**

Canonical: https://coreyjames.ai/agents/roles/safe-change-desk/  
Author: Corey James · Published: 2026-11-11 · Kind: agent role  

## The story

The agent rehearses the change first. A new limit runs in a mode where every decision is logged and nothing is held back, so the lead sees which jobs would have waited. Before a job starts on a paid machine, the agent checks the image, the settings and the budget. After the change it sends a small harmless batch through, saves the settings that worked and keeps the record of who changed what.

## Function

[Infrastructure and operations](https://coreyjames.ai/agents/functions/infrastructure-and-operations/): Machines, queues, databases and spend, watched through the night.

## The crew

The specialists behind this role, grouped by the kind of work they do.

### Challenges decisions

- [Change Risk Reviewer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/change-risk-reviewer) · [page](https://coreyjames.ai/agents/specialists/change-risk-reviewer/): Before a change goes in, this agent works out how risky it is from what it touches, maps everything that depends on it and asks for the matching level of checking.

### Keeps knowledge

- [Settings Change Keeper](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/settings-change-keeper) · [page](https://coreyjames.ai/agents/specialists/settings-change-keeper/): Compares the live settings with the saved ones, shows the history of changes, saves a known-good set and reloads it on request.

### Runs infrastructure

- [Throttle Rehearsal Analyst](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/throttle-rehearsal-analyst) · [page](https://coreyjames.ai/agents/specialists/throttle-rehearsal-analyst/): Runs a new limit in rehearsal mode, where every decision is logged and nothing is delayed, then reports which jobs would have waited before the limit is enforced.
- [Smoke Test Runner](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/smoke-test-runner) · [page](https://coreyjames.ai/agents/specialists/smoke-test-runner/): Sends a small harmless batch through the service, once or on a trigger, and confirms it came out the other end.
- [Throughput Tuner](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/throughput-tuner) · [page](https://coreyjames.ai/agents/specialists/throughput-tuner/): Adjusts how work is batched and flushed, from a careful standard setting to a very high-volume one, and measures the result.
- [Data Version Promoter](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/data-version-promoter) · [page](https://coreyjames.ai/agents/specialists/data-version-promoter/): Switches readers to a newly built version of stored data, finishes a build that stalled and cancels one that went wrong.
- [Planned Maintenance Coordinator](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/planned-maintenance-coordinator) · [page](https://coreyjames.ai/agents/specialists/planned-maintenance-coordinator/): Drains work, takes the database backup, shuts the services down in the documented order, brings them back in order, and checks each stage before moving on.

### Audits and guards

- [Launch Pre-flight Checker](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/launch-pre-flight-checker) · [page](https://coreyjames.ai/agents/specialists/launch-pre-flight-checker/): Checks the machine image, the settings and the budget before a job starts, and names what is wrong while fixing it is still free.
- [Operations Audit Clerk](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/operations-audit-clerk) · [page](https://coreyjames.ai/agents/specialists/operations-audit-clerk/): Keeps the trail of every pause, resume, scale and stop, and answers who did what to which job and when.

## The engineering behind this role

- [Pricing writes by what they cost the database](https://coreyjames.ai/stories/pricing-writes-by-what-they-cost/): Engineering story

## Citation

Corey James. "The Safe Change Desk." coreyjames.ai, 2026. https://coreyjames.ai/agents/roles/safe-change-desk/

```bibtex
@misc{coreyjames-agent-role-safe-change-desk,
  author = {Corey James},
  title = {The Safe Change Desk},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/roles/safe-change-desk/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/safe-change-desk}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
