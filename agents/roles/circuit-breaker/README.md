# The Circuit Breaker

**For an AI operations lead who needs a stop button and a paper trail.**

Canonical: https://coreyjames.ai/agents/roles/circuit-breaker/  
Author: Corey James · Published: 2026-11-11 · Kind: agent role  

## The story

A new agent is inspected before it joins: identity, access and workspace. While the team works, every start, failure and recovery is announced in the team chat. When one agent says another never answered, the agent follows that message hop by hop and names where it stopped. If a role misbehaves, every agent in that role is stopped at once, and the record shows what each one did.

## Function

[AI and model teams](https://coreyjames.ai/agents/functions/ai-and-model-teams/): Launching, tuning and supervising models and the agents that use them.

## The crew

The specialists behind this role, grouped by the kind of work they do.

### Speaks to people

- [Live Operations Announcer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/live-operations-announcer) · [page](https://coreyjames.ai/agents/specialists/live-operations-announcer/): It posts each event to the team in plain words as it happens.

### Supervises other agents

- [Lost Message Tracer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/lost-message-tracer) · [page](https://coreyjames.ai/agents/specialists/lost-message-tracer/): Follows a single message from agent to agent by its reference, shows each hop and how long it took, and names where it stopped.
- [Emergency Stop Officer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/emergency-stop-officer) · [page](https://coreyjames.ai/agents/specialists/emergency-stop-officer/): Stops one agent or every agent in a given role at once, records what was running and confirms nothing is left.
- [Pause and Resume Controller](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/pause-and-resume-controller) · [page](https://coreyjames.ai/agents/specialists/pause-and-resume-controller/): Pauses a single AI worker without losing its place and resumes it when the blocker clears.
- [Project Recovery Specialist](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/project-recovery-specialist) · [page](https://coreyjames.ai/agents/specialists/project-recovery-specialist/): Winds a team down cleanly, takes a checkpoint, and later re-reads the saved state and the real code to restart the work under a fresh resume, relaunching any reviewer whose session broke.
- [AI Fleet Supervisor](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/ai-fleet-supervisor) · [page](https://coreyjames.ai/agents/specialists/ai-fleet-supervisor/): Watches every running agent across every machine: who is alive, which tool versions they run, and who asked whom for what.

### Audits and guards

- [New Agent Pre-flight Inspector](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/new-agent-pre-flight-inspector) · [page](https://coreyjames.ai/agents/specialists/new-agent-pre-flight-inspector/): Checks a new agent's identity, access and workspace before it joins the team, and refuses the start when something does not match.
- [Agent Activity Auditor](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/agent-activity-auditor) · [page](https://coreyjames.ai/agents/specialists/agent-activity-auditor/): Reconstructs what any agent did in a time window: its raw actions, the conversations it took part in and the money it spent, in one audit report.
- [Scope Escalation Sentinel](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/scope-escalation-sentinel) · [page](https://coreyjames.ai/agents/specialists/scope-escalation-sentinel/): It warns that this label needs an independent review first and blocks the shortcut until that review exists.
- [Operations Audit Clerk](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/operations-audit-clerk) · [page](https://coreyjames.ai/agents/specialists/operations-audit-clerk/): Keeps the trail of every pause, resume, scale and stop, and answers who did what to which job and when.

## The engineering behind this role

- [Governed autonomous engineering](https://coreyjames.ai/capabilities/governed-autonomous-engineering/): Capability
- [Authority outside the model](https://coreyjames.ai/ideas/authority-outside-the-model/): Idea

## Citation

Corey James. "The Circuit Breaker." coreyjames.ai, 2026. https://coreyjames.ai/agents/roles/circuit-breaker/

```bibtex
@misc{coreyjames-agent-role-circuit-breaker,
  author = {Corey James},
  title = {The Circuit Breaker},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/roles/circuit-breaker/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/circuit-breaker}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
