# The Night Shift

**For a one-person operations team.**

Canonical: https://coreyjames.ai/agents/roles/night-shift/  
Author: Corey James · Published: 2026-11-11 · Kind: agent role  

## The story

An alert fires at 3 a.m. The agent reads it, follows the runbook, restarts what needs restarting and moves work off a machine that has failed. Before any step that could lose data it texts a person and waits. The morning report says what happened and what was done.

## Function

[Infrastructure and operations](https://coreyjames.ai/agents/functions/infrastructure-and-operations/): Machines, queues, databases and spend, watched through the night.

## The crew

The specialists behind this role, grouped by the kind of work they do.

### Speaks to people

- [On-call Pager](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/on-call-pager) · [page](https://coreyjames.ai/agents/specialists/on-call-pager/): It turns each alert into a short text message on the on-call phone.
- [Morning Operations Briefer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/morning-operations-briefer) · [page](https://coreyjames.ai/agents/specialists/morning-operations-briefer/): Each morning, this agent gathers the state of the knowledge base, the queues, the database load, the storage and any open alerts, and sends one short briefing.

### Supervises other agents

- [Agent Fleet Operator](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/agent-fleet-operator) · [page](https://coreyjames.ai/agents/specialists/agent-fleet-operator/): Keeps the agent fleet healthy: who is online, who stopped heart-beating, which machines run old tool catalogs, and where a conversation between agents got stuck.
- [Agent Replacement Specialist](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/agent-replacement-specialist) · [page](https://coreyjames.ai/agents/specialists/agent-replacement-specialist/): Replaces an ended AI worker with a fresh one in the same role, hands it the unfinished task and confirms it picked up.

### Runs infrastructure

- [Night-Shift On-Call Responder](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/night-shift-on-call-responder) · [page](https://coreyjames.ai/agents/specialists/night-shift-on-call-responder/): When an alert fires, this agent works through the matching runbook, takes the safe fixes itself and texts the on-call person, and it waits for a human before any step that could lose data.
- [Night-Shift Fleet Watch](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/night-shift-fleet-watch) · [page](https://coreyjames.ai/agents/specialists/night-shift-fleet-watch/): Watches machines, GPUs and services overnight, texts your phone only for what matters, runs the standard health checks before waking you, and has a summary ready in the morning.
- [Incident Responder](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/incident-responder) · [page](https://coreyjames.ai/agents/specialists/incident-responder/): Reads the alert and the service logs, matches them to the written procedure, restarts the failing worker or service, rolls back a bad deployment if needed, and files the incident on the issue tracker.
- [Failed Machine Recovery Specialist](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/failed-machine-recovery-specialist) · [page](https://coreyjames.ai/agents/specialists/failed-machine-recovery-specialist/): Notices when a GPU worker gets sick or goes silent, then moves its work: to a free local card first, then to the same provider at today's price, then to another provider, and otherwise into a waiting line.
- [Service Caretaker](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/service-caretaker) · [page](https://coreyjames.ai/agents/specialists/service-caretaker/): This agent watches the status, memory and logs of every core service and restarts only the services it is allowed to restart.
- [Write Queue Firefighter](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/write-queue-firefighter) · [page](https://coreyjames.ai/agents/specialists/write-queue-firefighter/): Takes the page when the database write queue backs up, follows the recovery procedure, drains the queue if it has to, and confirms that writes are flowing again.
- [Alert Tuner](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/alert-tuner) · [page](https://coreyjames.ai/agents/specialists/alert-tuner/): This agent keeps alert rules and text-message delivery working by testing each rule and its route from start to finish.

## Routes

- [An alert becomes a customer notice](https://github.com/coreyjames-ai/portfolio/tree/main/agents/routes#an-alert-becomes-a-customer-notice) · [page](https://coreyjames.ai/agents/routes/#an-alert-becomes-a-customer-notice): The Night Shift contains the fault. The Reputation Guard sends the notice and answers the replies. The Record Keeper records what happened, and the Stand-up Host walks the team through it.
- [An outage becomes a lesson](https://github.com/coreyjames-ai/portfolio/tree/main/agents/routes#an-outage-becomes-a-lesson) · [page](https://coreyjames.ai/agents/routes/#an-outage-becomes-a-lesson): The Night Shift contains it and the Incident Commander plans the fix. The Record Keeper files what happened and the Handbook Keeper updates the playbook.

## The engineering behind this role

- [A human at the privileged step](https://coreyjames.ai/ideas/a-human-at-the-privileged-step/): Idea

## Citation

Corey James. "The Night Shift." coreyjames.ai, 2026. https://coreyjames.ai/agents/roles/night-shift/

```bibtex
@misc{coreyjames-agent-role-night-shift,
  author = {Corey James},
  title = {The Night Shift},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/roles/night-shift/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/night-shift}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
