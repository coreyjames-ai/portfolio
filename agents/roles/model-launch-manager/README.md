# The Model Launch Manager

**For a platform lead shipping a new model version.**

Canonical: https://coreyjames.ai/agents/roles/model-launch-manager/  
Author: Corey James · Published: 2026-11-11 · Kind: agent role  

## The story

The agent serves the candidate next to the current model and puts both through the same hidden test set. It load-tests the candidate, checks that answers have stayed the same where they should and reports where each version fails. A candidate that clears the bar rolls out in stages.

## Function

[AI and model teams](https://coreyjames.ai/agents/functions/ai-and-model-teams/): Launching, tuning and supervising models and the agents that use them.

## The crew

The specialists behind this role, grouped by the kind of work they do.

### Challenges decisions

- [Release Readiness Reviewer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/release-readiness-reviewer) · [page](https://coreyjames.ai/agents/specialists/release-readiness-reviewer/): This agent pulls together the regression results, accuracy checks, load tests and package review for a new version and writes one go or no-go summary.

### Keeps knowledge

- [AI Model Librarian](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/ai-model-librarian) · [page](https://coreyjames.ai/agents/specialists/ai-model-librarian/): Brings a requested AI model in from its exact source, checks access and the licence question with the owner first, installs it, checks the files are intact and keeps the catalogue of every model and where it came from.

### Runs infrastructure

- [Model Serving Engineer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/model-serving-engineer) · [page](https://coreyjames.ai/agents/specialists/model-serving-engineer/): Builds a version of the model sized for each GPU card you own, measures how fast each card runs it, sets each card's limits for the scheduler, and copies the right build to every machine.
- [Model Comparison Evaluator](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/model-comparison-evaluator) · [page](https://coreyjames.ai/agents/specialists/model-comparison-evaluator/): This agent puts two or three model versions through the same hidden test set, runs any generated code safely, scores the answers strictly and explains where each version fails.
- [Model Rollout Manager](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/model-rollout-manager) · [page](https://coreyjames.ai/agents/specialists/model-rollout-manager/): Moves a new model version into service: builds it, sends a harmless test job through, benchmarks it against the current version, brings up new workers, drains the old ones, and puts the old version back if the new one is worse.
- [Serving Capacity Tuner](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/serving-capacity-tuner) · [page](https://coreyjames.ai/agents/specialists/serving-capacity-tuner/): Sets how much GPU memory holds conversations in progress and when new requests wait, then measures how many run at once.
- [Answer Consistency Setter](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/answer-consistency-setter) · [page](https://coreyjames.ai/agents/specialists/answer-consistency-setter/): Sets how predictable or varied a model's answers are, from fully repeatable to more varied, for each deployment.
- [AI Speed Investigator](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/ai-speed-investigator) · [page](https://coreyjames.ai/agents/specialists/ai-speed-investigator/): This agent finds where the time goes in each AI response, from the full request down to waiting, copying and the slowest steps, and compares serving modes side by side.
- [Capacity Planner](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/capacity-planner) · [page](https://coreyjames.ai/agents/specialists/capacity-planner/): Reads how fast each card runs, how full the queues and the database are, what is running now and what spot GPUs cost, then proposes where the next workload should go and whether renting is worth it.

### Audits and guards

- [AI Service Load Tester](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/ai-service-load-tester) · [page](https://coreyjames.ai/agents/specialists/ai-service-load-tester/): This agent runs the model under realistic traffic against a standard setup, checks each memory-saving path and compares runs.
- [AI Answer Accuracy Checker](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/ai-answer-accuracy-checker) · [page](https://coreyjames.ai/agents/specialists/ai-answer-accuracy-checker/): This agent checks whether a change alters the model's answers, finds where any difference starts and gives a clear yes or no.

## Routes

- [A new model becomes a story](https://github.com/coreyjames-ai/portfolio/tree/main/agents/routes#a-new-model-becomes-a-story) · [page](https://coreyjames.ai/agents/routes/#a-new-model-becomes-a-story): The Model Shrinker compresses it, the Model Launch Manager rolls it out under the Spend Controller's limit, and the Newsroom writes about it from the engineering record.

## The engineering behind this role

- [Bigger models and longer context on fixed GPU memory](https://coreyjames.ai/capabilities/longer-context-on-the-gpus-you-own/): Capability
- [Measure the instrument](https://coreyjames.ai/ideas/measure-the-instrument/): Idea
- [Proving a rewrite is the same system](https://coreyjames.ai/stories/proving-a-rewrite-is-the-same-system/): Engineering story

## Citation

Corey James. "The Model Launch Manager." coreyjames.ai, 2026. https://coreyjames.ai/agents/roles/model-launch-manager/

```bibtex
@misc{coreyjames-agent-role-model-launch-manager,
  author = {Corey James},
  title = {The Model Launch Manager},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/roles/model-launch-manager/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/model-launch-manager}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
