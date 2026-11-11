# The Model Shrinker

**For an AI team that needs a large model on a smaller card.**

Canonical: https://coreyjames.ai/agents/roles/model-shrinker/  
Author: Corey James · Published: 2026-11-11 · Kind: agent role  

## The story

A team of specialist agents compresses the model, measures what the compression cost in accuracy and tunes until the trade is acceptable. The result ships with a benchmark against the original.

## Function

[AI and model teams](https://coreyjames.ai/agents/functions/ai-and-model-teams/): Launching, tuning and supervising models and the agents that use them.

## The crew

The specialists behind this role, grouped by the kind of work they do.

### Does the work

- [Model Compression Team](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/model-compression-team) · [page](https://coreyjames.ai/agents/specialists/model-compression-team/): A coordinated group of six agents: one reads the model and serving code, one designs and applies the compression recipe, one measures quality against the full-size model, one measures speed, one checks every claim against the measurements, and a coordinator pulls it together into a release you can publish.
- [Model Optimization Team](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/model-optimization-team) · [page](https://coreyjames.ai/agents/specialists/model-optimization-team/): Splits model compression into coordinated specialist jobs: reading the model's source, building compressed variants, serving and timing them, measuring quality against the original and reviewing the evidence independently.
- [Memory Compression Researcher](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/memory-compression-researcher) · [page](https://coreyjames.ai/agents/specialists/memory-compression-researcher/): This agent tests ways to compress what the model keeps in memory, measures how much accuracy each costs and picks the best candidates.

### Challenges decisions

- [Release Readiness Reviewer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/release-readiness-reviewer) · [page](https://coreyjames.ai/agents/specialists/release-readiness-reviewer/): This agent pulls together the regression results, accuracy checks, load tests and package review for a new version and writes one go or no-go summary.

### Runs infrastructure

- [Performance Benchmark Analyst](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/performance-benchmark-analyst) · [page](https://coreyjames.ai/agents/specialists/performance-benchmark-analyst/): Runs the same fixed benchmark set on every change, reports the same four numbers each time, ramps concurrent users until a stop condition is hit, and says plainly whether the change helped.
- [Model Rollout Manager](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/model-rollout-manager) · [page](https://coreyjames.ai/agents/specialists/model-rollout-manager/): Moves a new model version into service: builds it, sends a harmless test job through, benchmarks it against the current version, brings up new workers, drains the old ones, and puts the old version back if the new one is worse.
- [Model Evaluation Analyst](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/model-evaluation-analyst) · [page](https://coreyjames.ai/agents/specialists/model-evaluation-analyst/): It compares compressed variants of a model against the original on fixed prompts and scored tasks, and it checks that a new model endpoint calls tools correctly before anyone relies on it.

### Audits and guards

- [AI Answer Accuracy Checker](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/ai-answer-accuracy-checker) · [page](https://coreyjames.ai/agents/specialists/ai-answer-accuracy-checker/): This agent checks whether a change alters the model's answers, finds where any difference starts and gives a clear yes or no.

## Routes

- [A new model becomes a story](https://github.com/coreyjames-ai/portfolio/tree/main/agents/routes#a-new-model-becomes-a-story) · [page](https://coreyjames.ai/agents/routes/#a-new-model-becomes-a-story): The Model Shrinker compresses it, the Model Launch Manager rolls it out under the Spend Controller's limit, and the Newsroom writes about it from the engineering record.

## The engineering behind this role

- [Bigger models and longer context on fixed GPU memory](https://coreyjames.ai/capabilities/longer-context-on-the-gpus-you-own/): Capability
- [Measure the instrument](https://coreyjames.ai/ideas/measure-the-instrument/): Idea

## Citation

Corey James. "The Model Shrinker." coreyjames.ai, 2026. https://coreyjames.ai/agents/roles/model-shrinker/

```bibtex
@misc{coreyjames-agent-role-model-shrinker,
  author = {Corey James},
  title = {The Model Shrinker},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/roles/model-shrinker/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/model-shrinker}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
