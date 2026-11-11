# The Incident Commander

**For an engineering manager in the middle of a messy incident.**

Canonical: https://coreyjames.ai/agents/roles/incident-commander/  
Author: Corey James · Published: 2026-11-11 · Kind: agent role  

## The story

An error alert arrives. The agent finds the code behind it and pulls what happened the last time that area broke. It gathers the evidence and asks a panel of several AI models to debate the fix. The agreed plan becomes tickets and a merge request for approval, and customers hear what is going on while the work is done.

## Function

[Engineering](https://coreyjames.ai/agents/functions/engineering/): Planning, building, reviewing and releasing software, with the reasoning kept.

## The crew

The specialists behind this role, grouped by the kind of work they do.

### Does the work

- [Incident Fix Planner](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/incident-fix-planner) · [page](https://coreyjames.ai/agents/specialists/incident-fix-planner/): This agent gathers the evidence for an incident, asks a panel of several AI models to debate the fix, and turns the agreed plan into tickets and a merge request for approval.
- [Ticket-to-Fix Engineer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/ticket-to-fix-engineer) · [page](https://coreyjames.ai/agents/specialists/ticket-to-fix-engineer/): This agent picks up a new ticket, makes the change, checks it, opens a merge request and leaves a note on the ticket so the requester knows it is ready for review.

### Speaks to people

- [Incident Communications Officer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/incident-communications-officer) · [page](https://coreyjames.ai/agents/specialists/incident-communications-officer/): During an outage it sends one factual update to affected customers by email and text, posts it on X and the Facebook Page, pins it, messages active website visitors, and sends the all-clear when service returns.
- [Supplier Support Liaison](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/supplier-support-liaison) · [page](https://coreyjames.ai/agents/specialists/supplier-support-liaison/): Writes up the unexplained problem with its evidence, raises it with the supplier's support, follows the case and reports the answer.

### Supervises other agents

- [Emergency Stop Officer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/emergency-stop-officer) · [page](https://coreyjames.ai/agents/specialists/emergency-stop-officer/): Stops one agent or every agent in a given role at once, records what was running and confirms nothing is left.
- [Lost Message Tracer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/lost-message-tracer) · [page](https://coreyjames.ai/agents/specialists/lost-message-tracer/): Follows a single message from agent to agent by its reference, shows each hop and how long it took, and names where it stopped.

### Challenges decisions

- [Issue Review Panel](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/issue-review-panel) · [page](https://coreyjames.ai/agents/specialists/issue-review-panel/): It assigns AI advisors distinct roles (mediator, technical expert, security auditor, devil's advocate, referee, pragmatist and innovator), has them review an issue together, and follows the issue for changes.

### Keeps knowledge

- [Incident Code Locator](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/incident-code-locator) · [page](https://coreyjames.ai/agents/specialists/incident-code-locator/): Finds the code that produced the error, traces what depends on it, explains the failure path, and leaves the finding in the team lead's inbox.
- [Regression Historian](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/regression-historian) · [page](https://coreyjames.ai/agents/specialists/regression-historian/): Given a broken function or an error, works out which pieces of work touched that area and in what order, who calls it now, and how the failure travels through the code.
- [Settings Change Keeper](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/settings-change-keeper) · [page](https://coreyjames.ai/agents/specialists/settings-change-keeper/): Compares the live settings with the saved ones, shows the history of changes, saves a known-good set and reloads it on request.

### Runs infrastructure

- [Incident Responder](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/incident-responder) · [page](https://coreyjames.ai/agents/specialists/incident-responder/): Reads the alert and the service logs, matches them to the written procedure, restarts the failing worker or service, rolls back a bad deployment if needed, and files the incident on the issue tracker.

### Audits and guards

- [Quarantine Officer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/quarantine-officer) · [page](https://coreyjames.ai/agents/specialists/quarantine-officer/): Isolates the misbehaving step so nothing sends it new work, keeps the rest running and releases it once it is fixed.

## Routes

- [An outage becomes a lesson](https://github.com/coreyjames-ai/portfolio/tree/main/agents/routes#an-outage-becomes-a-lesson) · [page](https://coreyjames.ai/agents/routes/#an-outage-becomes-a-lesson): The Night Shift contains it and the Incident Commander plans the fix. The Record Keeper files what happened and the Handbook Keeper updates the playbook.

## The engineering behind this role

- [Memory and code intelligence for agents](https://coreyjames.ai/capabilities/memory-and-code-intelligence-for-agents/): Capability
- [AI subscriptions as governed workers](https://coreyjames.ai/capabilities/use-the-ai-subscriptions-you-already-have/): Capability

## Citation

Corey James. "The Incident Commander." coreyjames.ai, 2026. https://coreyjames.ai/agents/roles/incident-commander/

```bibtex
@misc{coreyjames-agent-role-incident-commander,
  author = {Corey James},
  title = {The Incident Commander},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/roles/incident-commander/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/incident-commander}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
