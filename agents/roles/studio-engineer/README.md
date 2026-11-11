# The Studio Engineer

**For a studio or IT lead with graphics machines.**

Canonical: https://coreyjames.ai/agents/roles/studio-engineer/  
Author: Corey James · Published: 2026-11-11 · Kind: agent role  

## The story

The agent keeps the library of AI models: where each file came from and whether it is intact. It starts and stops the render services, schedules the jobs so the power draw stays within what the building supplies and diagnoses a job that fails.

## Function

[Infrastructure and operations](https://coreyjames.ai/agents/functions/infrastructure-and-operations/): Machines, queues, databases and spend, watched through the night.

## The crew

The specialists behind this role, grouped by the kind of work they do.

### Does the work

- [Render Producer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/render-producer) · [page](https://coreyjames.ai/agents/specialists/render-producer/): It follows the job, confirms the finished file, moves it to the right destination, and hands it over or publishes it.
- [Production Planner](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/production-planner) · [page](https://coreyjames.ai/agents/specialists/production-planner/): Turns an approved storyboard into a signed-off production plan with the GPU budget it needs and a brief for each specialist, so production starts without back-and-forth.

### Speaks to people

- [Fleet Help Desk](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/fleet-help-desk) · [page](https://coreyjames.ai/agents/specialists/fleet-help-desk/): Answers plain questions such as "what is running on which GPU", "what has today cost" or "which machine is free" by picking the right fleet tools for the question.

### Keeps knowledge

- [AI Model Librarian](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/ai-model-librarian) · [page](https://coreyjames.ai/agents/specialists/ai-model-librarian/): Brings a requested AI model in from its exact source, checks access and the licence question with the owner first, installs it, checks the files are intact and keeps the catalogue of every model and where it came from.

### Runs infrastructure

- [Render Farm Operator](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/render-farm-operator) · [page](https://coreyjames.ai/agents/specialists/render-farm-operator/): Keeps the GPU image and video service running for the whole team: starts it only within the spend limit, watches health and logs, frees GPU memory between jobs and shuts it down when work is done.
- [Render Job Troubleshooter](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/render-job-troubleshooter) · [page](https://coreyjames.ai/agents/specialists/render-job-troubleshooter/): Steps in when an image or video job fails: reads the error and the service log, re-sends the finished file if only the hand-off failed, otherwise fixes the cause and runs the job again.
- [New Render Machine Setup Technician](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/new-render-machine-setup-technician) · [page](https://coreyjames.ai/agents/specialists/new-render-machine-setup-technician/): Brings a new graphics machine into service: confirms the GPU, starts the service, registers the models already on disk, runs a test image and a test video and shuts down.
- [Shared GPU Traffic Warden](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/shared-gpu-traffic-warden) · [page](https://coreyjames.ai/agents/specialists/shared-gpu-traffic-warden/): Lets requests into the small model only when the card has measured free memory, and otherwise answers "busy, try again in this many seconds" instead of crashing the large model.

### Audits and guards

- [GPU Spend and Power Guard](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/gpu-spend-and-power-guard) · [page](https://coreyjames.ai/agents/specialists/gpu-spend-and-power-guard/): Keeps rendering inside the daily spend limit and the office's power limit: no job starts without budget, and only one graphics card runs flat out at a time.

## The engineering behind this role

- [Budgets and refusals](https://coreyjames.ai/ideas/budgets-and-refusals/): Idea

## Citation

Corey James. "The Studio Engineer." coreyjames.ai, 2026. https://coreyjames.ai/agents/roles/studio-engineer/

```bibtex
@misc{coreyjames-agent-role-studio-engineer,
  author = {Corey James},
  title = {The Studio Engineer},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/roles/studio-engineer/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/studio-engineer}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
