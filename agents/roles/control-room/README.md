# The Control Room

**For an AI operations lead with agents running on many machines.**

Canonical: https://coreyjames.ai/agents/roles/control-room/  
Author: Corey James · Published: 2026-11-11 · Kind: agent role  

## The story

The agent knows which agents are alive, which have gone silent and who asked whom for what. Work held by a silent agent is taken back and reassigned. Large jobs are split into small ones and handed to short-lived workers. What the agents did becomes searchable notes, so an error turns into a lesson and an approval into a recorded decision. A digest arrives every day.

## Function

[AI and model teams](https://coreyjames.ai/agents/functions/ai-and-model-teams/): Launching, tuning and supervising models and the agents that use them.

## The crew

The specialists behind this role, grouped by the kind of work they do.

### Speaks to people

- [Platform Help Desk](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/platform-help-desk) · [page](https://coreyjames.ai/agents/specialists/platform-help-desk/): Registers itself before any restart, watches progress every fifteen minutes, answers the team lead's questions on a private support channel, logs real defects and ships the smallest fix when something blocks the team.

### Supervises other agents

- [AI Fleet Supervisor](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/ai-fleet-supervisor) · [page](https://coreyjames.ai/agents/specialists/ai-fleet-supervisor/): Watches every running agent across every machine: who is alive, which tool versions they run, and who asked whom for what.
- [Agent Fleet Operator](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/agent-fleet-operator) · [page](https://coreyjames.ai/agents/specialists/agent-fleet-operator/): Keeps the agent fleet healthy: who is online, who stopped heart-beating, which machines run old tool catalogs, and where a conversation between agents got stuck.
- [Agent Fleet Health Monitor](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/agent-fleet-health-monitor) · [page](https://coreyjames.ai/agents/specialists/agent-fleet-health-monitor/): It removes silent agents from the roster, updates the list of available machines, and reports fleet status.
- [Agent Coordination Dispatcher](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/agent-coordination-dispatcher) · [page](https://coreyjames.ai/agents/specialists/agent-coordination-dispatcher/): It acts on the request, starts a child job when the work needs another specialist, and replies to the sender.
- [AI Session Supervisor](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/ai-session-supervisor) · [page](https://coreyjames.ai/agents/specialists/ai-session-supervisor/): Keeps interactive assistant sessions running on the right machine, delivers team messages to them, and accounts for every transcript and every unit of usage, without giving a session access to the database.
- [Rate Limit Recovery Agent](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/rate-limit-recovery-agent) · [page](https://coreyjames.ai/agents/specialists/rate-limit-recovery-agent/): It prompts the stalled session to retry its last step so the work continues without a person stepping in.

### Keeps knowledge

- [Agent Activity Historian](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/agent-activity-historian) · [page](https://coreyjames.ai/agents/specialists/agent-activity-historian/): Turns what agents did into searchable notes, so that tool errors become lessons and approvals become recorded decisions.
- [Decision History Keeper](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/decision-history-keeper) · [page](https://coreyjames.ai/agents/specialists/decision-history-keeper/): It turns notable actions into entries in the searchable decision history.
- [Long-Session Memory Keeper](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/long-session-memory-keeper) · [page](https://coreyjames.ai/agents/specialists/long-session-memory-keeper/): Keeps a long session within its memory budget by shrinking older tool output in stages and leaving a pointer that brings the full text back on request.

### Runs infrastructure

- [Background Job Orchestrator](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/background-job-orchestrator) · [page](https://coreyjames.ai/agents/specialists/background-job-orchestrator/): Splits a job into child jobs, hands them to short-lived workers, tracks each one and collects the results.

### Audits and guards

- [Tool Version Checker](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/tool-version-checker) · [page](https://coreyjames.ai/agents/specialists/tool-version-checker/): Compares the tool list on every machine in the fleet and names any machine running an older version.

## Routes

- [A new function becomes a staffed desk](https://github.com/coreyjames-ai/portfolio/tree/main/agents/routes#a-new-function-becomes-a-staffed-desk) · [page](https://coreyjames.ai/agents/routes/#a-new-function-becomes-a-staffed-desk): The Team Architect designs the specialists and the Operations Desk puts them on call. The Control Room watches them and the Spend Controller caps what they cost.

## The engineering behind this role

- [Governed autonomous engineering](https://coreyjames.ai/capabilities/governed-autonomous-engineering/): Capability
- [Memory and code intelligence for agents](https://coreyjames.ai/capabilities/memory-and-code-intelligence-for-agents/): Capability

## Citation

Corey James. "The Control Room." coreyjames.ai, 2026. https://coreyjames.ai/agents/roles/control-room/

```bibtex
@misc{coreyjames-agent-role-control-room,
  author = {Corey James},
  title = {The Control Room},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/roles/control-room/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/control-room}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
