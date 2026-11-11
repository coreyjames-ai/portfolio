# The Bulk Run Manager

**For a team with millions of prompts to process.**

Canonical: https://coreyjames.ai/agents/roles/bulk-run-manager/  
Author: Corey James · Published: 2026-11-11 · Kind: agent role  

## The story

The agent estimates the job, rents the processors it needs within the budget and spreads the work across them. Machines that fail are replaced and their work is picked up. The results arrive with a cost report.

## Function

[AI and model teams](https://coreyjames.ai/agents/functions/ai-and-model-teams/): Launching, tuning and supervising models and the agents that use them.

## The crew

The specialists behind this role, grouped by the kind of work they do.

### Runs infrastructure

- [Capacity Planner](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/capacity-planner) · [page](https://coreyjames.ai/agents/specialists/capacity-planner/): Reads how fast each card runs, how full the queues and the database are, what is running now and what spot GPUs cost, then proposes where the next workload should go and whether renting is worth it.
- [Cloud GPU Buyer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/cloud-gpu-buyer) · [page](https://coreyjames.ai/agents/specialists/cloud-gpu-buyer/): Rents cloud GPUs only when the day's budget allows, prefers the cheapest current spot price, connects them back to your private network over an outbound link, and hands them back as soon as the work is done or the money runs out.
- [Bulk Inference Run Manager](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/bulk-inference-run-manager) · [page](https://coreyjames.ai/agents/specialists/bulk-inference-run-manager/): Takes a very large pile of prompts, packs them so every GPU stays busy, collects the answers after the submitting programs have gone home, and writes the results back with every item accounted for.
- [Failed Machine Recovery Specialist](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/failed-machine-recovery-specialist) · [page](https://coreyjames.ai/agents/specialists/failed-machine-recovery-specialist/): Notices when a GPU worker gets sick or goes silent, then moves its work: to a free local card first, then to the same provider at today's price, then to another provider, and otherwise into a waiting line.
- [Compute Cost Reporter](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/compute-cost-reporter) · [page](https://coreyjames.ai/agents/specialists/compute-cost-reporter/): Reports what compute and AI usage cost, broken down by machine, by dataset, by team role and by model, with today's projection and storage costs alongside.
- [Failed Item Replayer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/failed-item-replayer) · [page](https://coreyjames.ai/agents/specialists/failed-item-replayer/): Sends only the failed items of a large run back through, cancels a run that should stop, and refuses to start a duplicate of a run already in progress.
- [GPU Fleet Manager](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/gpu-fleet-manager) · [page](https://coreyjames.ai/agents/specialists/gpu-fleet-manager/): Starts a GPU worker on whichever machine you name, tells you what is running where, and shuts down idle workers with their final cost.
- [Cloud Price Watcher](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/cloud-price-watcher) · [page](https://coreyjames.ai/agents/specialists/cloud-price-watcher/): It compares the new price with the ceiling the owner set, then moves the work or holds it.
- [Recovery Policy Setter](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/recovery-policy-setter) · [page](https://coreyjames.ai/agents/specialists/recovery-policy-setter/): Sets for each job whether a lost machine is replaced automatically, moved to owned hardware, paused for a decision or allowed to fail, and how much extra price is acceptable.

### Audits and guards

- [Compute Budget Guardian](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/compute-budget-guardian) · [page](https://coreyjames.ai/agents/specialists/compute-budget-guardian/): Holds the line on the daily spend that only you set: it refuses any start the budget cannot cover and says why, warns you as spend climbs, and stops paid machines at the cap.
- [Run Verification Clerk](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/run-verification-clerk) · [page](https://coreyjames.ai/agents/specialists/run-verification-clerk/): Checks a finished run against its original request and reports whether every item is present, without running anything again.
- [Database Overload Guard](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/database-overload-guard) · [page](https://coreyjames.ai/agents/specialists/database-overload-guard/): This agent lets bulk loads into the database only as fast as the database can take them, frees stuck jobs and recommends capacity changes.

## The engineering behind this role

- [High-throughput batch inference and embeddings](https://coreyjames.ai/capabilities/high-throughput-batch-inference/): Capability
- [Budgets and refusals](https://coreyjames.ai/ideas/budgets-and-refusals/): Idea
- [One call to a GPU anywhere](https://coreyjames.ai/stories/one-call-to-a-gpu-anywhere/): Engineering story
- [Recovery that trusts only what happened](https://coreyjames.ai/stories/recovery-that-trusts-only-what-happened/): Engineering story

## Citation

Corey James. "The Bulk Run Manager." coreyjames.ai, 2026. https://coreyjames.ai/agents/roles/bulk-run-manager/

```bibtex
@misc{coreyjames-agent-role-bulk-run-manager,
  author = {Corey James},
  title = {The Bulk Run Manager},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/roles/bulk-run-manager/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/bulk-run-manager}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
