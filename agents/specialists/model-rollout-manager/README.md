# Model Rollout Manager

**Moves a new model version into service: builds it, sends a harmless test job through, benchmarks it against the current version, brings up new workers, drains the old ones, and puts the old version back if the new one is worse.**

Canonical: https://coreyjames.ai/agents/specialists/model-rollout-manager/  
Author: Corey James · Published: 2026-11-11 · Kind: agent specialist  

## What it does

Moves a new model version into service: builds it, sends a harmless test job through, benchmarks it against the current version, brings up new workers, drains the old ones, and puts the old version back if the new one is worse.

For an ML platform lead shipping a new model version.

Kind: [Runs infrastructure](https://coreyjames.ai/agents/specialists/?kind=runs-infrastructure). Keeps machines, queues and data moving.

Group: AI models and performance.

## Roles it serves

- [The Model Launch Manager](https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/model-launch-manager) · [page](https://coreyjames.ai/agents/roles/model-launch-manager/): For a platform lead shipping a new model version.
- [The Model Shrinker](https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/model-shrinker) · [page](https://coreyjames.ai/agents/roles/model-shrinker/): For an AI team that needs a large model on a smaller card.

## Routes it travels

- [A new model becomes a story](https://github.com/coreyjames-ai/portfolio/tree/main/agents/routes#a-new-model-becomes-a-story) · [page](https://coreyjames.ai/agents/routes/#a-new-model-becomes-a-story): The Model Shrinker compresses it, the Model Launch Manager rolls it out under the Spend Controller's limit, and the Newsroom writes about it from the engineering record.

## Citation

Corey James. "Model Rollout Manager." coreyjames.ai, 2026. https://coreyjames.ai/agents/specialists/model-rollout-manager/

```bibtex
@misc{coreyjames-agent-specialist-model-rollout-manager,
  author = {Corey James},
  title = {Model Rollout Manager},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/specialists/model-rollout-manager/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/model-rollout-manager}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
