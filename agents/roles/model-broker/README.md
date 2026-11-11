# The Model Broker

**For an AI team lead paying several model providers.**

Canonical: https://coreyjames.ai/agents/roles/model-broker/  
Author: Corey James · Published: 2026-11-11 · Kind: agent role  

## The story

Every model call from every agent passes through one switchboard. The agent sends each call to an approved provider, keeps each provider inside its rate limit and steps down to a cheaper tier when a quota runs out. Commercial AI assistants that want access are registered, and a person approves each grant. Every call is charged to the task that made it.

## Function

[AI and model teams](https://coreyjames.ai/agents/functions/ai-and-model-teams/): Launching, tuning and supervising models and the agents that use them.

## The crew

The specialists behind this role, grouped by the kind of work they do.

### Speaks to people

- [Tool Concierge](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/tool-concierge) · [page](https://coreyjames.ai/agents/specialists/tool-concierge/): Takes a plain-language need and returns the best-matching tools from a catalog of hundreds in one answer.

### Keeps knowledge

- [AI Spend Recorder](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/ai-spend-recorder) · [page](https://coreyjames.ai/agents/specialists/ai-spend-recorder/): It reads the model usage from the session, removes duplicates, and records the cost against the task it belongs to.
- [Memory Return-on-Investment Reporter](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/memory-return-on-investment-reporter) · [page](https://coreyjames.ai/agents/specialists/memory-return-on-investment-reporter/): Reports the tokens spent creating each note against the tokens saved each time a note is reused or compressed, priced per model provider on per-token or flat-fee plans, and shows project-level totals on a live dashboard.

### Runs infrastructure

- [AI Provider Switchboard](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/ai-provider-switchboard) · [page](https://coreyjames.ai/agents/specialists/ai-provider-switchboard/): Sends every agent's model calls to an approved provider, keeps each provider inside its rate limit, steps down to a cheaper tier when a quota runs out, and blocks traffic that a provider's terms do not allow.
- [Model Comparison Evaluator](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/model-comparison-evaluator) · [page](https://coreyjames.ai/agents/specialists/model-comparison-evaluator/): This agent puts two or three model versions through the same hidden test set, runs any generated code safely, scores the answers strictly and explains where each version fails.

### Audits and guards

- [AI Access Desk](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/ai-access-desk) · [page](https://coreyjames.ai/agents/specialists/ai-access-desk/): Registers each AI assistant as an app, holds every grant until a person approves it, accepts sign-in tokens from your own server and from your workplace platform, shows each assistant only the tools it is allowed, and ties every action to the assignment rather than to what the assistant claims.
- [Engineering Cost Analyst](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/engineering-cost-analyst) · [page](https://coreyjames.ai/agents/specialists/engineering-cost-analyst/): Attributes every model call to the task, role and phase that spent it and turns the totals into cost and human-equivalent effort hours per project.

## The engineering behind this role

- [AI subscriptions as governed workers](https://coreyjames.ai/capabilities/use-the-ai-subscriptions-you-already-have/): Capability
- [Role contracts, with vendors as data](https://coreyjames.ai/ideas/role-contracts-not-vendors/): Idea
- [What the work cost, to the penny](https://coreyjames.ai/stories/what-the-work-cost/): Engineering story

## Citation

Corey James. "The Model Broker." coreyjames.ai, 2026. https://coreyjames.ai/agents/roles/model-broker/

```bibtex
@misc{coreyjames-agent-role-model-broker,
  author = {Corey James},
  title = {The Model Broker},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/roles/model-broker/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/model-broker}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
