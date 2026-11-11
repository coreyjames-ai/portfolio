# The AI Workforce Manager

**For a manager running a team of AI agents.**

Canonical: https://coreyjames.ai/agents/roles/ai-workforce-manager/  
Author: Corey James · Published: 2026-11-11 · Kind: agent role  

## The story

The agent staffs each project with the right mix of agents, starts them and stops them. It watches every session, restarts the ones that hit a limit and records what each task cost. If an agent steps outside its assignment, the manager hears about it. Any question about what an agent did has an answer on file.

## Function

[AI and model teams](https://coreyjames.ai/agents/functions/ai-and-model-teams/): Launching, tuning and supervising models and the agents that use them.

## The crew

The specialists behind this role, grouped by the kind of work they do.

### Supervises other agents

- [Team Staffing Coordinator](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/team-staffing-coordinator) · [page](https://coreyjames.ai/agents/specialists/team-staffing-coordinator/): Assembles a mixed team from different model families, gives each role its tool access, replaces anyone who drops out with their history intact and winds the team down at the end.
- [AI Team Dispatcher](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/ai-team-dispatcher) · [page](https://coreyjames.ai/agents/specialists/ai-team-dispatcher/): Starts an AI agent for each role you need, each with its own limited access, workspace and budget, on the machine you choose.
- [AI Session Supervisor](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/ai-session-supervisor) · [page](https://coreyjames.ai/agents/specialists/ai-session-supervisor/): Keeps interactive assistant sessions running on the right machine, delivers team messages to them, and accounts for every transcript and every unit of usage, without giving a session access to the database.
- [Rate Limit Recovery Agent](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/rate-limit-recovery-agent) · [page](https://coreyjames.ai/agents/specialists/rate-limit-recovery-agent/): It prompts the stalled session to retry its last step so the work continues without a person stepping in.
- [Agent Replacement Specialist](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/agent-replacement-specialist) · [page](https://coreyjames.ai/agents/specialists/agent-replacement-specialist/): Replaces an ended AI worker with a fresh one in the same role, hands it the unfinished task and confirms it picked up.
- [Work Budget Setter](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/work-budget-setter) · [page](https://coreyjames.ai/agents/specialists/work-budget-setter/): Sets a limit on the number of steps an AI worker may take and reports when the worker reaches it.
- [Role Catalogue Updater](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/role-catalogue-updater) · [page](https://coreyjames.ai/agents/specialists/role-catalogue-updater/): Loads new role descriptions and tool lists into the running system without a restart, so the next worker launched uses them.
- [Engineering Team Lead](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/engineering-team-lead) · [page](https://coreyjames.ai/agents/specialists/engineering-team-lead/): Runs the whole team through the project: hands out ready work, relays review findings, applies each next step and keeps everyone pointed at the finish line.

### Challenges decisions

- [Task Results Reviewer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/task-results-reviewer) · [page](https://coreyjames.ai/agents/specialists/task-results-reviewer/): It checks the result, marks the task complete or cancelled, and starts the next task in line.

### Keeps knowledge

- [AI Spend Recorder](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/ai-spend-recorder) · [page](https://coreyjames.ai/agents/specialists/ai-spend-recorder/): It reads the model usage from the session, removes duplicates, and records the cost against the task it belongs to.

### Audits and guards

- [Scope Escalation Sentinel](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/scope-escalation-sentinel) · [page](https://coreyjames.ai/agents/specialists/scope-escalation-sentinel/): It warns that this label needs an independent review first and blocks the shortcut until that review exists.
- [Agent Activity Auditor](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/agent-activity-auditor) · [page](https://coreyjames.ai/agents/specialists/agent-activity-auditor/): Reconstructs what any agent did in a time window: its raw actions, the conversations it took part in and the money it spent, in one audit report.

## Routes

- [A text becomes a finished project](https://github.com/coreyjames-ai/portfolio/tree/main/agents/routes#a-text-becomes-a-finished-project) · [page](https://coreyjames.ai/agents/routes/#a-text-becomes-a-finished-project): The owner texts the Pocket Operator. The Programme Office runs the work, the AI Workforce Manager staffs it, and the result returns to the owner's phone.

## The engineering behind this role

- [Governed autonomous engineering](https://coreyjames.ai/capabilities/governed-autonomous-engineering/): Capability
- [AI subscriptions as governed workers](https://coreyjames.ai/capabilities/use-the-ai-subscriptions-you-already-have/): Capability
- [What the work cost, to the penny](https://coreyjames.ai/stories/what-the-work-cost/): Engineering story
- [Directing AI coding agents at program scale](https://coreyjames.ai/stories/directing-ai-coding-agents-at-program-scale/): Engineering story

## Citation

Corey James. "The AI Workforce Manager." coreyjames.ai, 2026. https://coreyjames.ai/agents/roles/ai-workforce-manager/

```bibtex
@misc{coreyjames-agent-role-ai-workforce-manager,
  author = {Corey James},
  title = {The AI Workforce Manager},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/roles/ai-workforce-manager/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/ai-workforce-manager}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
