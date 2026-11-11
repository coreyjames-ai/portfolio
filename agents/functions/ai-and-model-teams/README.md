# AI and model teams

**Launching, tuning and supervising models and the agents that use them.**

Canonical: https://coreyjames.ai/agents/functions/ai-and-model-teams/  
Author: Corey James · Published: 2026-11-11 · Kind: agent function  

## The roles

- [The AI Workforce Manager](https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/ai-workforce-manager) · [page](https://coreyjames.ai/agents/roles/ai-workforce-manager/): For a manager running a team of AI agents.
- [The Model Launch Manager](https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/model-launch-manager) · [page](https://coreyjames.ai/agents/roles/model-launch-manager/): For a platform lead shipping a new model version.
- [The Model Shrinker](https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/model-shrinker) · [page](https://coreyjames.ai/agents/roles/model-shrinker/): For an AI team that needs a large model on a smaller card.
- [The Speed Detective](https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/speed-detective) · [page](https://coreyjames.ai/agents/roles/speed-detective/): For a platform lead whose model responds slower than it should.
- [The Bulk Run Manager](https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/bulk-run-manager) · [page](https://coreyjames.ai/agents/roles/bulk-run-manager/): For a team with millions of prompts to process.
- [The Model Interviewer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/model-interviewer) · [page](https://coreyjames.ai/agents/roles/model-interviewer/): For a research lead who wants what a model knows in a form people can search.
- [The Model Broker](https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/model-broker) · [page](https://coreyjames.ai/agents/roles/model-broker/): For an AI team lead paying several model providers.
- [The Research Lab](https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/research-lab) · [page](https://coreyjames.ai/agents/roles/research-lab/): For a research director running an AI program with several lines of work.
- [The Engine Builder](https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/engine-builder) · [page](https://coreyjames.ai/agents/roles/engine-builder/): For an engineering lead shipping an AI engine to more than one kind of graphics processor.
- [The Team Architect](https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/team-architect) · [page](https://coreyjames.ai/agents/roles/team-architect/): For a founder who wants a set of specialist assistants built around the company's own material.
- [The Control Room](https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/control-room) · [page](https://coreyjames.ai/agents/roles/control-room/): For an AI operations lead with agents running on many machines.
- [The Circuit Breaker](https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/circuit-breaker) · [page](https://coreyjames.ai/agents/roles/circuit-breaker/): For an AI operations lead who needs a stop button and a paper trail.
- [The Archive Keeper](https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/archive-keeper) · [page](https://coreyjames.ai/agents/roles/archive-keeper/): For a research lead whose results must still be readable next year.

## Specialists these roles share

- [AI Answer Accuracy Checker](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/ai-answer-accuracy-checker) · [page](https://coreyjames.ai/agents/specialists/ai-answer-accuracy-checker/): This agent checks whether a change alters the model's answers, finds where any difference starts and gives a clear yes or no.
- [AI Experiment Runner](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/ai-experiment-runner) · [page](https://coreyjames.ai/agents/specialists/ai-experiment-runner/): This agent runs each experiment the same way: it sets up a baseline, packages the experiment, runs it on the GPUs with measurement attached and compares the result with the baseline.
- [AI Fleet Supervisor](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/ai-fleet-supervisor) · [page](https://coreyjames.ai/agents/specialists/ai-fleet-supervisor/): Watches every running agent across every machine: who is alive, which tool versions they run, and who asked whom for what.
- [AI Service Load Tester](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/ai-service-load-tester) · [page](https://coreyjames.ai/agents/specialists/ai-service-load-tester/): This agent runs the model under realistic traffic against a standard setup, checks each memory-saving path and compares runs.
- [AI Session Supervisor](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/ai-session-supervisor) · [page](https://coreyjames.ai/agents/specialists/ai-session-supervisor/): Keeps interactive assistant sessions running on the right machine, delivers team messages to them, and accounts for every transcript and every unit of usage, without giving a session access to the database.
- [AI Speed Investigator](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/ai-speed-investigator) · [page](https://coreyjames.ai/agents/specialists/ai-speed-investigator/): This agent finds where the time goes in each AI response, from the full request down to waiting, copying and the slowest steps, and compares serving modes side by side.
- [AI Spend Recorder](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/ai-spend-recorder) · [page](https://coreyjames.ai/agents/specialists/ai-spend-recorder/): It reads the model usage from the session, removes duplicates, and records the cost against the task it belongs to.
- [Agent Activity Auditor](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/agent-activity-auditor) · [page](https://coreyjames.ai/agents/specialists/agent-activity-auditor/): Reconstructs what any agent did in a time window: its raw actions, the conversations it took part in and the money it spent, in one audit report.
- [Bulk Inference Run Manager](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/bulk-inference-run-manager) · [page](https://coreyjames.ai/agents/specialists/bulk-inference-run-manager/): Takes a very large pile of prompts, packs them so every GPU stays busy, collects the answers after the submitting programs have gone home, and writes the results back with every item accounted for.
- [Capacity Planner](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/capacity-planner) · [page](https://coreyjames.ai/agents/specialists/capacity-planner/): Reads how fast each card runs, how full the queues and the database are, what is running now and what spot GPUs cost, then proposes where the next workload should go and whether renting is worth it.
- [Failed Item Replayer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/failed-item-replayer) · [page](https://coreyjames.ai/agents/specialists/failed-item-replayer/): Sends only the failed items of a large run back through, cancels a run that should stop, and refuses to start a duplicate of a run already in progress.
- [GPU Profiler](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/gpu-profiler) · [page](https://coreyjames.ai/agents/specialists/gpu-profiler/): This agent profiles the AI engine at system, chip and memory level, finds idle time under steady load and records GPU use.
- [Memory Compression Researcher](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/memory-compression-researcher) · [page](https://coreyjames.ai/agents/specialists/memory-compression-researcher/): This agent tests ways to compress what the model keeps in memory, measures how much accuracy each costs and picks the best candidates.
- [Model Comparison Evaluator](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/model-comparison-evaluator) · [page](https://coreyjames.ai/agents/specialists/model-comparison-evaluator/): This agent puts two or three model versions through the same hidden test set, runs any generated code safely, scores the answers strictly and explains where each version fails.
- [Model Evaluation Analyst](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/model-evaluation-analyst) · [page](https://coreyjames.ai/agents/specialists/model-evaluation-analyst/): It compares compressed variants of a model against the original on fixed prompts and scored tasks, and it checks that a new model endpoint calls tools correctly before anyone relies on it.
- [Model Insight Extractor](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/model-insight-extractor) · [page](https://coreyjames.ai/agents/specialists/model-insight-extractor/): Generates a large set of test prompts, runs them through the model, captures the model's internal state for each prompt, and re-runs any that failed.
- [Model Rollout Manager](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/model-rollout-manager) · [page](https://coreyjames.ai/agents/specialists/model-rollout-manager/): Moves a new model version into service: builds it, sends a harmless test job through, benchmarks it against the current version, brings up new workers, drains the old ones, and puts the old version back if the new one is worse.
- [Model Serving Engineer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/model-serving-engineer) · [page](https://coreyjames.ai/agents/specialists/model-serving-engineer/): Builds a version of the model sized for each GPU card you own, measures how fast each card runs it, sets each card's limits for the scheduler, and copies the right build to every machine.
- [New Agent Pre-flight Inspector](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/new-agent-pre-flight-inspector) · [page](https://coreyjames.ai/agents/specialists/new-agent-pre-flight-inspector/): Checks a new agent's identity, access and workspace before it joins the team, and refuses the start when something does not match.
- [Performance Benchmark Analyst](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/performance-benchmark-analyst) · [page](https://coreyjames.ai/agents/specialists/performance-benchmark-analyst/): Runs the same fixed benchmark set on every change, reports the same four numbers each time, ramps concurrent users until a stop condition is hit, and says plainly whether the change helped.
- [Rate Limit Recovery Agent](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/rate-limit-recovery-agent) · [page](https://coreyjames.ai/agents/specialists/rate-limit-recovery-agent/): It prompts the stalled session to retry its last step so the work continues without a person stepping in.
- [Release Readiness Reviewer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/release-readiness-reviewer) · [page](https://coreyjames.ai/agents/specialists/release-readiness-reviewer/): This agent pulls together the regression results, accuracy checks, load tests and package review for a new version and writes one go or no-go summary.
- [Research Data Archivist](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/research-data-archivist) · [page](https://coreyjames.ai/agents/specialists/research-data-archivist/): This agent manages stored research data by version: it lists what is stored, closes and activates versions, releases checkpoints and clears out old versions.
- [Run Conditions Recorder](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/run-conditions-recorder) · [page](https://coreyjames.ai/agents/specialists/run-conditions-recorder/): This agent records GPU memory and machine load around every run so results are read against the conditions they ran in.
- [Run Verification Clerk](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/run-verification-clerk) · [page](https://coreyjames.ai/agents/specialists/run-verification-clerk/): Checks a finished run against its original request and reports whether every item is present, without running anything again.
- [Scope Escalation Sentinel](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/scope-escalation-sentinel) · [page](https://coreyjames.ai/agents/specialists/scope-escalation-sentinel/): It warns that this label needs an independent review first and blocks the shortcut until that review exists.
- [Serving Capacity Tuner](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/serving-capacity-tuner) · [page](https://coreyjames.ai/agents/specialists/serving-capacity-tuner/): Sets how much GPU memory holds conversations in progress and when new requests wait, then measures how many run at once.
- [Storage Incident Handler](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/storage-incident-handler) · [page](https://coreyjames.ai/agents/specialists/storage-incident-handler/): When storage reports a problem, this agent reads the recovery report, runs a consistency check, sends lost items back for reprocessing and records the sign-off.
- [Team Staffing Coordinator](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/team-staffing-coordinator) · [page](https://coreyjames.ai/agents/specialists/team-staffing-coordinator/): Assembles a mixed team from different model families, gives each role its tool access, replaces anyone who drops out with their history intact and winds the team down at the end.
- [Tool Concierge](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/tool-concierge) · [page](https://coreyjames.ai/agents/specialists/tool-concierge/): Takes a plain-language need and returns the best-matching tools from a catalog of hundreds in one answer.
- [Training Data Producer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/training-data-producer) · [page](https://coreyjames.ai/agents/specialists/training-data-producer/): It writes prompts designed to draw out a model's behaviour, runs resumable collection jobs across graphics servers, and stores what it collects for training, with status and replay.

## The engineering behind these roles

- [AI subscriptions as governed workers](https://coreyjames.ai/capabilities/use-the-ai-subscriptions-you-already-have/): Capability
- [Bigger models and longer context on fixed GPU memory](https://coreyjames.ai/capabilities/longer-context-on-the-gpus-you-own/): Capability
- [High-throughput batch inference and embeddings](https://coreyjames.ai/capabilities/high-throughput-batch-inference/): Capability
- [What the work cost, to the penny](https://coreyjames.ai/stories/what-the-work-cost/): Engineering story
- [A router beside a production model](https://coreyjames.ai/stories/a-router-beside-a-production-model/): Engineering story
- [The observer that changed the answer](https://coreyjames.ai/stories/the-observer-that-changed-the-answer/): Engineering story

## Citation

Corey James. "AI and model teams." coreyjames.ai, 2026. https://coreyjames.ai/agents/functions/ai-and-model-teams/

```bibtex
@misc{coreyjames-agent-function-ai-and-model-teams,
  author = {Corey James},
  title = {AI and model teams},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/functions/ai-and-model-teams/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/functions/ai-and-model-teams}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
