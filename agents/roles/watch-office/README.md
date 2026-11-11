# The Watch Office

**For an operations lead who wants one screen and alerts that mean something.**

Canonical: https://coreyjames.ai/agents/roles/watch-office/  
Author: Corey James · Published: 2026-11-11 · Kind: agent role  

## The story

The agent builds the dashboards from the numbers the services already report. It tests every alert rule and its route to a phone from start to finish. Anyone on the team can ask in plain words what is running on which machine, what today has cost or which machine is free.

## Function

[Infrastructure and operations](https://coreyjames.ai/agents/functions/infrastructure-and-operations/): Machines, queues, databases and spend, watched through the night.

## The crew

The specialists behind this role, grouped by the kind of work they do.

### Does the work

- [Operations Dashboard Builder](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/operations-dashboard-builder) · [page](https://coreyjames.ai/agents/specialists/operations-dashboard-builder/): This agent builds the dashboards for jobs, queues, mining and system resources from the numbers the services already report, and checks that they load.

### Speaks to people

- [Fleet Help Desk](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/fleet-help-desk) · [page](https://coreyjames.ai/agents/specialists/fleet-help-desk/): Answers plain questions such as "what is running on which GPU", "what has today cost" or "which machine is free" by picking the right fleet tools for the question.
- [On-call Pager](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/on-call-pager) · [page](https://coreyjames.ai/agents/specialists/on-call-pager/): It turns each alert into a short text message on the on-call phone.
- [Live Operations Announcer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/live-operations-announcer) · [page](https://coreyjames.ai/agents/specialists/live-operations-announcer/): It posts each event to the team in plain words as it happens.

### Supervises other agents

- [Agent Fleet Health Monitor](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/agent-fleet-health-monitor) · [page](https://coreyjames.ai/agents/specialists/agent-fleet-health-monitor/): It removes silent agents from the roster, updates the list of available machines, and reports fleet status.

### Runs infrastructure

- [Alert Tuner](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/alert-tuner) · [page](https://coreyjames.ai/agents/specialists/alert-tuner/): This agent keeps alert rules and text-message delivery working by testing each rule and its route from start to finish.
- [GPU Capacity Inventory Clerk](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/gpu-capacity-inventory-clerk) · [page](https://coreyjames.ai/agents/specialists/gpu-capacity-inventory-clerk/): This agent takes stock of memory, model weights and idle capacity on each machine and rolls it up into one picture for planning.
- [Memory Service Operator](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/memory-service-operator) · [page](https://coreyjames.ai/agents/specialists/memory-service-operator/): Looks after the service day to day.
- [Night-Shift Fleet Watch](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/night-shift-fleet-watch) · [page](https://coreyjames.ai/agents/specialists/night-shift-fleet-watch/): Watches machines, GPUs and services overnight, texts your phone only for what matters, runs the standard health checks before waking you, and has a summary ready in the morning.

### Audits and guards

- [Index Stall Watchdog](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/index-stall-watchdog) · [page](https://coreyjames.ai/agents/specialists/index-stall-watchdog/): Resets the stuck job so scheduled indexing carries on, and records the reset.

## Citation

Corey James. "The Watch Office." coreyjames.ai, 2026. https://coreyjames.ai/agents/roles/watch-office/

```bibtex
@misc{coreyjames-agent-role-watch-office,
  author = {Corey James},
  title = {The Watch Office},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/roles/watch-office/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/watch-office}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
