# The Speed Detective

**For a platform lead whose model responds slower than it should.**

Canonical: https://coreyjames.ai/agents/roles/speed-detective/  
Author: Corey James · Published: 2026-11-11 · Kind: agent role  

## The story

The agent profiles the engine, traces hardware events and breaks each response down into where the time went. It records the conditions of every run so results can be compared fairly. Each proposed fix is tested as an experiment, with a check that the answers stayed the same.

## Function

[AI and model teams](https://coreyjames.ai/agents/functions/ai-and-model-teams/): Launching, tuning and supervising models and the agents that use them.

## The crew

The specialists behind this role, grouped by the kind of work they do.

### Does the work

- [AI Experiment Runner](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/ai-experiment-runner) · [page](https://coreyjames.ai/agents/specialists/ai-experiment-runner/): This agent runs each experiment the same way: it sets up a baseline, packages the experiment, runs it on the GPUs with measurement attached and compares the result with the baseline.

### Keeps knowledge

- [Run Conditions Recorder](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/run-conditions-recorder) · [page](https://coreyjames.ai/agents/specialists/run-conditions-recorder/): This agent records GPU memory and machine load around every run so results are read against the conditions they ran in.

### Runs infrastructure

- [AI Speed Investigator](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/ai-speed-investigator) · [page](https://coreyjames.ai/agents/specialists/ai-speed-investigator/): This agent finds where the time goes in each AI response, from the full request down to waiting, copying and the slowest steps, and compares serving modes side by side.
- [GPU Profiler](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/gpu-profiler) · [page](https://coreyjames.ai/agents/specialists/gpu-profiler/): This agent profiles the AI engine at system, chip and memory level, finds idle time under steady load and records GPU use.
- [Hardware Event Tracer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/hardware-event-tracer) · [page](https://coreyjames.ai/agents/specialists/hardware-event-tracer/): This agent records low-level hardware events and queue activity and attributes each delay to its cause.
- [Serving Capacity Tuner](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/serving-capacity-tuner) · [page](https://coreyjames.ai/agents/specialists/serving-capacity-tuner/): Sets how much GPU memory holds conversations in progress and when new requests wait, then measures how many run at once.

### Audits and guards

- [AI Answer Accuracy Checker](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/ai-answer-accuracy-checker) · [page](https://coreyjames.ai/agents/specialists/ai-answer-accuracy-checker/): This agent checks whether a change alters the model's answers, finds where any difference starts and gives a clear yes or no.
- [AI Service Load Tester](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/ai-service-load-tester) · [page](https://coreyjames.ai/agents/specialists/ai-service-load-tester/): This agent runs the model under realistic traffic against a standard setup, checks each memory-saving path and compares runs.

## The engineering behind this role

- [High-throughput batch inference and embeddings](https://coreyjames.ai/capabilities/high-throughput-batch-inference/): Capability
- [Measure the instrument](https://coreyjames.ai/ideas/measure-the-instrument/): Idea
- [The observer that changed the answer](https://coreyjames.ai/stories/the-observer-that-changed-the-answer/): Engineering story
- [The thirteen percent that was never missing](https://coreyjames.ai/stories/the-thirteen-percent-that-was-never-missing/): Engineering story
- [From 44K to 163K tokens per second](https://coreyjames.ai/stories/from-44k-to-163k-tokens-per-second/): Engineering story

## Citation

Corey James. "The Speed Detective." coreyjames.ai, 2026. https://coreyjames.ai/agents/roles/speed-detective/

```bibtex
@misc{coreyjames-agent-role-speed-detective,
  author = {Corey James},
  title = {The Speed Detective},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/roles/speed-detective/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/speed-detective}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
