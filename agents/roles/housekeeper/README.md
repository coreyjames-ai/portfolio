# The Housekeeper

**For an operations lead whose systems collect clutter.**

Canonical: https://coreyjames.ai/agents/roles/housekeeper/  
Author: Corey James · Published: 2026-11-11 · Kind: agent role  

## The story

Dead jobs leave locks behind, and stalled workers stay attached to their queues. The agent finds both, shows what it would remove and clears them once the lead agrees. It sets how worker time is shared between quick updates and bulk loads. A retired machine is taken out of the fleet and its certificates are revoked. The lead also gets the trend in job run times, with the slowest step named.

## Function

[Infrastructure and operations](https://coreyjames.ai/agents/functions/infrastructure-and-operations/): Machines, queues, databases and spend, watched through the night.

## The crew

The specialists behind this role, grouped by the kind of work they do.

### Does the work

- [Automation Library Caretaker](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/automation-library-caretaker) · [page](https://coreyjames.ai/agents/specialists/automation-library-caretaker/): This agent keeps the team's library of automated jobs up to date.

### Keeps knowledge

- [Job Performance Historian](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/job-performance-historian) · [page](https://coreyjames.ai/agents/specialists/job-performance-historian/): Keeps the run history of every job and reports the trend over the last hour, day, week or month, with the slowest step named.
- [Deleted Code Cleaner](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/deleted-code-cleaner) · [page](https://coreyjames.ai/agents/specialists/deleted-code-cleaner/): Deletes the search entries and dependency links for code that no longer exists, without holding up the scan.

### Runs infrastructure

- [Stuck Job Unblocker](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/stuck-job-unblocker) · [page](https://coreyjames.ai/agents/specialists/stuck-job-unblocker/): Finds the locks left behind by dead jobs, confirms nothing live depends on them and releases them so the queue moves again.
- [Stale Worker Sweeper](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/stale-worker-sweeper) · [page](https://coreyjames.ai/agents/specialists/stale-worker-sweeper/): Lists the workers that have sat idle past a set time, shows what would be removed as a dry run and clears them.
- [Queue Priority Balancer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/queue-priority-balancer) · [page](https://coreyjames.ai/agents/specialists/queue-priority-balancer/): Sets how worker time is shared between quick updates and bulk loads, and switches either line off during maintenance.
- [Machine Decommissioner](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/machine-decommissioner) · [page](https://coreyjames.ai/agents/specialists/machine-decommissioner/): Takes a retired machine out of the fleet, revokes its certificates and confirms nothing still routes work to it.
- [Index Upkeep Operator](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/index-upkeep-operator) · [page](https://coreyjames.ai/agents/specialists/index-upkeep-operator/): Keeps every index matching its source.
- [Storage Space Reclaimer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/storage-space-reclaimer) · [page](https://coreyjames.ai/agents/specialists/storage-space-reclaimer/): Lists the old stored versions, confirms which one is active and clears the ones no longer needed.
- [Service Caretaker](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/service-caretaker) · [page](https://coreyjames.ai/agents/specialists/service-caretaker/): This agent watches the status, memory and logs of every core service and restarts only the services it is allowed to restart.

## The engineering behind this role

- [Rules that never ran](https://coreyjames.ai/stories/rules-that-never-ran/): Engineering story

## Citation

Corey James. "The Housekeeper." coreyjames.ai, 2026. https://coreyjames.ai/agents/roles/housekeeper/

```bibtex
@misc{coreyjames-agent-role-housekeeper,
  author = {Corey James},
  title = {The Housekeeper},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/roles/housekeeper/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/housekeeper}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
