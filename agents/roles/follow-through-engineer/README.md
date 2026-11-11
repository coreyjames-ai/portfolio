# The Follow-Through Engineer

**For an engineering manager walking out of a design meeting.**

Canonical: https://coreyjames.ai/agents/roles/follow-through-engineer/  
Author: Corey James · Published: 2026-11-11 · Kind: agent role  

## The story

The agent takes the meeting transcript and pulls out the engineering action items. For each one it finds where in the code the work would land and how far it reaches. It drafts the task plan and will not let a task start without a file and line reference behind it.

## Function

[Engineering](https://coreyjames.ai/agents/functions/engineering/): Planning, building, reviewing and releasing software, with the reasoning kept.

## The crew

The specialists behind this role, grouped by the kind of work they do.

### Does the work

- [Meeting Follow-up Engineer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/meeting-follow-up-engineer) · [page](https://coreyjames.ai/agents/specialists/meeting-follow-up-engineer/): Takes the meeting transcript and pulls out the engineering action items.
- [Project Planning Clerk](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/project-planning-clerk) · [page](https://coreyjames.ai/agents/specialists/project-planning-clerk/): It turns what you want done into a fully specified plan grounded in the real code and project, checks it before anyone begins, records the facts it relied on with two independent checks, and handles approved changes to a plan already under way.
- [Teams Work Request Runner](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/teams-work-request-runner) · [page](https://coreyjames.ai/agents/specialists/teams-work-request-runner/): It starts a worker on a local machine or in the cloud, keeps the requester informed of progress, returns the results and files, and shuts the worker down when idle.
- [Meeting Follow-through Agent](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/meeting-follow-through-agent) · [page](https://coreyjames.ai/agents/specialists/meeting-follow-through-agent/): It takes the request, runs the work on a worker while the meeting continues, posts the result in the meeting chat, and records the item in the minutes.

### Keeps knowledge

- [Meeting Minute-Taker](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/meeting-minute-taker) · [page](https://coreyjames.ai/agents/specialists/meeting-minute-taker/): Takes the minutes after every meeting from the recording and transcript, and sends everyone the same version, updating it when someone points out a correction.
- [Code Impact Analyst](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/code-impact-analyst) · [page](https://coreyjames.ai/agents/specialists/code-impact-analyst/): For every function or type a change touches, it lists what calls it and what it calls up to three steps out.
- [Grounding Coach](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/grounding-coach) · [page](https://coreyjames.ai/agents/specialists/grounding-coach/): Checks whether the task troubleshoots or spans several files and, if so, asks for a file and line reference from code search before work starts.

## The engineering behind this role

- [Memory and code intelligence for agents](https://coreyjames.ai/capabilities/memory-and-code-intelligence-for-agents/): Capability
- [Compute first, narrate second](https://coreyjames.ai/ideas/compute-first-narrate-second/): Idea

## Citation

Corey James. "The Follow-Through Engineer." coreyjames.ai, 2026. https://coreyjames.ai/agents/roles/follow-through-engineer/

```bibtex
@misc{coreyjames-agent-role-follow-through-engineer,
  author = {Corey James},
  title = {The Follow-Through Engineer},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/roles/follow-through-engineer/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/follow-through-engineer}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
