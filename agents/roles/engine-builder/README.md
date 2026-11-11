# The Engine Builder

**For an engineering lead shipping an AI engine to more than one kind of graphics processor.**

Canonical: https://coreyjames.ai/agents/roles/engine-builder/  
Author: Corey James · Published: 2026-11-11 · Kind: agent role  

## The story

The agent takes stock of each machine: memory, model files and idle capacity. It builds the engine for each processor type, runs the tests and measures throughput with the results saved. Where a small helper model shares a card with a large one, it lets requests in only when there is measured room and tells the rest when to try again.

## Function

[AI and model teams](https://coreyjames.ai/agents/functions/ai-and-model-teams/): Launching, tuning and supervising models and the agents that use them.

## The crew

The specialists behind this role, grouped by the kind of work they do.

### Does the work

- [Release Engineer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/release-engineer) · [page](https://coreyjames.ai/agents/specialists/release-engineer/): Screens each candidate change for benchmark gaming, builds release images from pinned inputs, checks every hash, compares the candidate with the current baseline and promotes it, then tells the other teams to rebase.

### Keeps knowledge

- [Porting Pattern Scout](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/porting-pattern-scout) · [page](https://coreyjames.ai/agents/specialists/porting-pattern-scout/): Finds how a reference library or specification solves a problem and where the team's own code would host the equivalent.

### Runs infrastructure

- [GPU Capacity Inventory Clerk](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/gpu-capacity-inventory-clerk) · [page](https://coreyjames.ai/agents/specialists/gpu-capacity-inventory-clerk/): This agent takes stock of memory, model weights and idle capacity on each machine and rolls it up into one picture for planning.
- [AI Engine Build and Benchmark Agent](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/ai-engine-build-and-benchmark-agent) · [page](https://coreyjames.ai/agents/specialists/ai-engine-build-and-benchmark-agent/): This agent builds the engine for each GPU type, runs its tests and measures throughput with saved results.
- [Performance Benchmark Analyst](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/performance-benchmark-analyst) · [page](https://coreyjames.ai/agents/specialists/performance-benchmark-analyst/): Runs the same fixed benchmark set on every change, reports the same four numbers each time, ramps concurrent users until a stop condition is hit, and says plainly whether the change helped.
- [Shared GPU Traffic Warden](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/shared-gpu-traffic-warden) · [page](https://coreyjames.ai/agents/specialists/shared-gpu-traffic-warden/): Lets requests into the small model only when the card has measured free memory, and otherwise answers "busy, try again in this many seconds" instead of crashing the large model.
- [Model Serving Engineer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/model-serving-engineer) · [page](https://coreyjames.ai/agents/specialists/model-serving-engineer/): Builds a version of the model sized for each GPU card you own, measures how fast each card runs it, sets each card's limits for the scheduler, and copies the right build to every machine.
- [GPU Server Onboarder](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/gpu-server-onboarder) · [page](https://coreyjames.ai/agents/specialists/gpu-server-onboarder/): This agent prepares a newly built AI engine to take work from the shared queue by writing and checking the settings files it needs.
- [GPU Profiler](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/gpu-profiler) · [page](https://coreyjames.ai/agents/specialists/gpu-profiler/): This agent profiles the AI engine at system, chip and memory level, finds idle time under steady load and records GPU use.
- [Model Courier](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/model-courier) · [page](https://coreyjames.ai/agents/specialists/model-courier/): Copies each new model build to the remote machines that serve it and confirms every copy arrived complete.

## The engineering behind this role

- [Custom small models for tool calling and routing](https://coreyjames.ai/capabilities/small-models-for-tool-calling-and-routing/): Capability
- [Budgets and refusals](https://coreyjames.ai/ideas/budgets-and-refusals/): Idea
- [A router beside a production model](https://coreyjames.ai/stories/a-router-beside-a-production-model/): Engineering story
- [Bringing a serving stack up on new silicon](https://coreyjames.ai/stories/bringing-a-serving-stack-up-on-new-silicon/): Engineering story
- [Engines for the card you have](https://coreyjames.ai/stories/engines-for-the-card-you-have/): Engineering story

## Citation

Corey James. "The Engine Builder." coreyjames.ai, 2026. https://coreyjames.ai/agents/roles/engine-builder/

```bibtex
@misc{coreyjames-agent-role-engine-builder,
  author = {Corey James},
  title = {The Engine Builder},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/roles/engine-builder/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/engine-builder}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
