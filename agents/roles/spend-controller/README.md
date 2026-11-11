# The Spend Controller

**For whoever signs off on compute spend.**

Canonical: https://coreyjames.ai/agents/roles/spend-controller/  
Author: Corey James · Published: 2026-11-11 · Kind: agent role  

## The story

The owner sets a daily limit, and only the owner can change it. Every request to start a machine or an AI worker passes the agent first. A request that would break the limit is refused with the reason and the numbers. The finance lead gets a cost report by project.

## Function

[Infrastructure and operations](https://coreyjames.ai/agents/functions/infrastructure-and-operations/): Machines, queues, databases and spend, watched through the night.

## The crew

The specialists behind this role, grouped by the kind of work they do.

### Supervises other agents

- [Work Budget Setter](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/work-budget-setter) · [page](https://coreyjames.ai/agents/specialists/work-budget-setter/): Sets a limit on the number of steps an AI worker may take and reports when the worker reaches it.

### Keeps knowledge

- [AI Spend Recorder](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/ai-spend-recorder) · [page](https://coreyjames.ai/agents/specialists/ai-spend-recorder/): It reads the model usage from the session, removes duplicates, and records the cost against the task it belongs to.

### Runs infrastructure

- [Cloud Compute Dispatcher](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/cloud-compute-dispatcher) · [page](https://coreyjames.ai/agents/specialists/cloud-compute-dispatcher/): This agent picks an image, checks the container settings, runs the job on local or rented GPUs, keeps an eye on it and shuts the container down when it is done.
- [Storage Spend Reconciler](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/storage-spend-reconciler) · [page](https://coreyjames.ai/agents/specialists/storage-spend-reconciler/): It syncs the day's storage cost into the daily budget so tomorrow's limit reflects real spend.
- [Compute Cost Reporter](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/compute-cost-reporter) · [page](https://coreyjames.ai/agents/specialists/compute-cost-reporter/): Reports what compute and AI usage cost, broken down by machine, by dataset, by team role and by model, with today's projection and storage costs alongside.
- [Idle Machine Drainer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/idle-machine-drainer) · [page](https://coreyjames.ai/agents/specialists/idle-machine-drainer/): Sets how long a machine may sit idle, empties its queues when the time is up and shuts it down.
- [Cloud Price Watcher](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/cloud-price-watcher) · [page](https://coreyjames.ai/agents/specialists/cloud-price-watcher/): It compares the new price with the ceiling the owner set, then moves the work or holds it.
- [Recovery Policy Setter](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/recovery-policy-setter) · [page](https://coreyjames.ai/agents/specialists/recovery-policy-setter/): Sets for each job whether a lost machine is replaced automatically, moved to owned hardware, paused for a decision or allowed to fail, and how much extra price is acceptable.
- [AI Provider Switchboard](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/ai-provider-switchboard) · [page](https://coreyjames.ai/agents/specialists/ai-provider-switchboard/): Sends every agent's model calls to an approved provider, keeps each provider inside its rate limit, steps down to a cheaper tier when a quota runs out, and blocks traffic that a provider's terms do not allow.

### Audits and guards

- [Compute Budget Guardian](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/compute-budget-guardian) · [page](https://coreyjames.ai/agents/specialists/compute-budget-guardian/): Holds the line on the daily spend that only you set: it refuses any start the budget cannot cover and says why, warns you as spend climbs, and stops paid machines at the cap.
- [Engineering Cost Analyst](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/engineering-cost-analyst) · [page](https://coreyjames.ai/agents/specialists/engineering-cost-analyst/): Attributes every model call to the task, role and phase that spent it and turns the totals into cost and human-equivalent effort hours per project.
- [GPU Spend and Power Guard](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/gpu-spend-and-power-guard) · [page](https://coreyjames.ai/agents/specialists/gpu-spend-and-power-guard/): Keeps rendering inside the daily spend limit and the office's power limit: no job starts without budget, and only one graphics card runs flat out at a time.

## Routes

- [A new model becomes a story](https://github.com/coreyjames-ai/portfolio/tree/main/agents/routes#a-new-model-becomes-a-story) · [page](https://coreyjames.ai/agents/routes/#a-new-model-becomes-a-story): The Model Shrinker compresses it, the Model Launch Manager rolls it out under the Spend Controller's limit, and the Newsroom writes about it from the engineering record.
- [A new function becomes a staffed desk](https://github.com/coreyjames-ai/portfolio/tree/main/agents/routes#a-new-function-becomes-a-staffed-desk) · [page](https://coreyjames.ai/agents/routes/#a-new-function-becomes-a-staffed-desk): The Team Architect designs the specialists and the Operations Desk puts them on call. The Control Room watches them and the Spend Controller caps what they cost.

## The engineering behind this role

- [AI subscriptions as governed workers](https://coreyjames.ai/capabilities/use-the-ai-subscriptions-you-already-have/): Capability
- [Budgets and refusals](https://coreyjames.ai/ideas/budgets-and-refusals/): Idea
- [One call to a GPU anywhere](https://coreyjames.ai/stories/one-call-to-a-gpu-anywhere/): Engineering story
- [What the work cost, to the penny](https://coreyjames.ai/stories/what-the-work-cost/): Engineering story

## Citation

Corey James. "The Spend Controller." coreyjames.ai, 2026. https://coreyjames.ai/agents/roles/spend-controller/

```bibtex
@misc{coreyjames-agent-role-spend-controller,
  author = {Corey James},
  title = {The Spend Controller},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/roles/spend-controller/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/spend-controller}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
