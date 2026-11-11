# The Research Lab

**For a research director running an AI program with several lines of work.**

Canonical: https://coreyjames.ai/agents/roles/research-lab/  
Author: Corey James · Published: 2026-11-11 · Kind: agent role  

## The story

The agent splits the program among specialists who each own their files, and keeps processor time and final assembly to itself. One specialist captures what a model does internally across a large prompt set. Another tests ways to compress what the model holds in memory and measures what each costs in accuracy. Results are stored by version, and when storage reports a fault, lost items go back for reprocessing.

## Function

[AI and model teams](https://coreyjames.ai/agents/functions/ai-and-model-teams/): Launching, tuning and supervising models and the agents that use them.

## The crew

The specialists behind this role, grouped by the kind of work they do.

### Does the work

- [Model Insight Extractor](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/model-insight-extractor) · [page](https://coreyjames.ai/agents/specialists/model-insight-extractor/): Generates a large set of test prompts, runs them through the model, captures the model's internal state for each prompt, and re-runs any that failed.
- [Memory Compression Researcher](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/memory-compression-researcher) · [page](https://coreyjames.ai/agents/specialists/memory-compression-researcher/): This agent tests ways to compress what the model keeps in memory, measures how much accuracy each costs and picks the best candidates.
- [AI Experiment Runner](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/ai-experiment-runner) · [page](https://coreyjames.ai/agents/specialists/ai-experiment-runner/): This agent runs each experiment the same way: it sets up a baseline, packages the experiment, runs it on the GPUs with measurement attached and compares the result with the baseline.
- [Training Data Producer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/training-data-producer) · [page](https://coreyjames.ai/agents/specialists/training-data-producer/): It writes prompts designed to draw out a model's behaviour, runs resumable collection jobs across graphics servers, and stores what it collects for training, with status and replay.

### Supervises other agents

- [AI Research Team Lead](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/ai-research-team-lead) · [page](https://coreyjames.ai/agents/specialists/ai-research-team-lead/): This agent splits a research program among specialists who each own their own files, keeps GPU time and final assembly to itself, and keeps a tamper-evident record of decisions.

### Keeps knowledge

- [Research Data Archivist](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/research-data-archivist) · [page](https://coreyjames.ai/agents/specialists/research-data-archivist/): This agent manages stored research data by version: it lists what is stored, closes and activates versions, releases checkpoints and clears out old versions.

### Runs infrastructure

- [Model Evaluation Analyst](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/model-evaluation-analyst) · [page](https://coreyjames.ai/agents/specialists/model-evaluation-analyst/): It compares compressed variants of a model against the original on fixed prompts and scored tasks, and it checks that a new model endpoint calls tools correctly before anyone relies on it.
- [Storage Incident Handler](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/storage-incident-handler) · [page](https://coreyjames.ai/agents/specialists/storage-incident-handler/): When storage reports a problem, this agent reads the recovery report, runs a consistency check, sends lost items back for reprocessing and records the sign-off.
- [Failed Item Replayer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/failed-item-replayer) · [page](https://coreyjames.ai/agents/specialists/failed-item-replayer/): Sends only the failed items of a large run back through, cancels a run that should stop, and refuses to start a duplicate of a run already in progress.
- [Bulk Inference Run Manager](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/bulk-inference-run-manager) · [page](https://coreyjames.ai/agents/specialists/bulk-inference-run-manager/): Takes a very large pile of prompts, packs them so every GPU stays busy, collects the answers after the submitting programs have gone home, and writes the results back with every item accounted for.

## The engineering behind this role

- [High-throughput batch inference and embeddings](https://coreyjames.ai/capabilities/high-throughput-batch-inference/): Capability
- [Bigger models and longer context on fixed GPU memory](https://coreyjames.ai/capabilities/longer-context-on-the-gpus-you-own/): Capability
- [A detector for a silent corruption](https://coreyjames.ai/stories/a-detector-for-a-silent-corruption/): Engineering story
- [Judge a representation by the bytes it stops moving](https://coreyjames.ai/stories/judge-a-representation-by-the-bytes-it-stops-moving/): Engineering story

## Citation

Corey James. "The Research Lab." coreyjames.ai, 2026. https://coreyjames.ai/agents/roles/research-lab/

```bibtex
@misc{coreyjames-agent-role-research-lab,
  author = {Corey James},
  title = {The Research Lab},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/roles/research-lab/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/research-lab}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
