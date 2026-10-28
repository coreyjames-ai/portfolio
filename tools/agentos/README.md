# AgentOS work tools



Canonical: https://coreyjames.ai/tools/agentos/  
Author: Corey James · Published: 2026-10-28 · Kind: tool group  
Systems: [AgentOS](https://github.com/coreyjames-ai/agentos) · [Agent Swarm](https://github.com/coreyjames-ai/agent-swarm) · [FAFOHive](https://github.com/coreyjames-ai/fafohive)  

## What was built

[AgentOS](https://coreyjames.ai/systems/agentos) runs teams of AI agents against governed work orders, and the agents in those teams need a way to act inside that governance without being able to bend it. I gave them a deliberately narrow set of tools. The caller's identity fixes which work order, team and role it is acting for, so an agent cannot name a different work order or claim a different seat. Most actions take the path of a file the agent has written, so large plans and reviews stay on disk and the tool call stays small. Many of the tools answer with a receipt and deliver the final outcome to the team lead's mailbox, because the work they start keeps going after the call returns.

## Authoring and running work orders

`mcp_wo_author` turns a planning conversation into a finished work order without starting it.

- `render_author_packet` renders the authoring instructions for a project and objective, anchored to the planning marker and workspace.
- `validate_author_plan` checks the plan, proof and source files the authoring model wrote to disk.
- `apply_author_plan` finalizes the work order from those files.

`agentos_work_order_execution` starts and stops work at the level of whole work orders.

- `start` launches a finalized work order. AgentOS derives the team, personas, models, accounts and grounding from the work order itself, and the caller cannot override them. The launch can bring up the full roster or the team lead first.
- `continue` resumes an interrupted execution from its stored state.
- `archive_work_orders` archives work orders the operator has explicitly approved for archiving.

`agentos_work_order_amendment` adds work discovered after a piece of the plan has closed, without rewriting history. The amendment produces one new work package that runs through the normal machinery, and everything already done stays as it was.

- `start_amendment` opens an amendment for one distinct discovery.
- `submit_amendment_role_output` submits the architect's or another role's written contribution.
- `author_amend_request` writes the formal amendment request.
- `authorize_amendment` authorizes the new work package.
- `revise_amendment` corrects a still-open amended package through the same amendment.

`agentos_work_order_progression` moves governed work forward.

- `apply_continuation` lets the team lead apply a continuation that AgentOS delivered.
- `submit_qa_fix_claim` lets a developer submit a claim that a QA finding is fixed, which releases the developer while AgentOS handles the rest.

## Running the team

`agentos_team_management` manages the team frozen into the work order.

- `preview_create_team` checks a complete authored roster without changing anything.
- `create_team` registers and launches that roster once.
- `list_running_work_orders` lists every running execution and which of them can be stopped.
- `list_team_members` shows the roster.
- `member_status` inspects one member.
- `launch_member` fills an authored seat that is empty.
- `replace_member` replaces a stalled member in the same seat.
- `terminate_member` stops one member with no replacement.
- `terminate_team` stands down one exact execution.

`agentos_participant` is how teammates talk.

- `list_team_members` returns the current roster, so messages go to real seats.
- `send_message` sends a durable message or file-path handoff to one teammate. Messages wait in the recipient's mailbox while it is busy.
- `list_messages` reads the member's own mailbox.

`agentos_operational_task` handles operational work that sits outside the plan, submitted by the team lead as a saved contract.

- `create`, `list`, `assign`, `complete` and `cancel` each submit the contract for that step and return a receipt. The outcome arrives in the team lead's mailbox.

`agentos_qa` carries independent QA.

- `get_template` returns the template for a QA request or a QA result.
- `submit_review` submits the team lead's QA request for a work package.
- `submit_result` submits the assigned QA seat's result.
- `status` reads the durable QA state.

## Wiring the outside world in

`agentos_event_source` lets any seat connect an outside system to the work order. Every event lands in the team lead's mailbox, and incoming data never changes the work order's scope.

- `register` creates a source and returns its intake address and credential once.
- `list` and `get` show the work order's sources.
- `update` changes a source's description, event types or enabled state.
- `rotate_credential` issues a new credential when the old one is lost.

## Support for the platform itself

`agentos_harness_support` is a dedicated line between a team lead and the operator for defects in the platform machinery, kept separate from ordinary team traffic.

- `send_message` reports a blocking machinery defect, and carries the operator's diagnosis and retry instructions back.
- `list_messages` reads that line.
- `channel_status` shows where the line is routed.
- `close_channel` closes it.

`agentos_helpdesk_registration` registers the operator's support session as the helpdesk for work orders.

- `register` submits the registration as a small typed job.
- `status` confirms whether the registration took effect.

The narrowness is the design. An agent can coordinate, report, ask for QA and pull in events, and every one of those paths ends in state that AgentOS owns.

## What was verified

Each line is a claim the canonical page supports, with the figure as the page states it.

- Agent orchestration tools: 11 tools that let governed agents author, validate and start work orders and act inside their team without being able to name another work order or seat.
- Identity-scoped agent actions: the caller's identity fixes its work order, team and role; actions take file paths and return receipts, with outcomes delivered to the team lead's mailbox.

## Related

- System: [AgentOS](https://github.com/coreyjames-ai/agentos)
- System: [Agent Swarm](https://github.com/coreyjames-ai/agent-swarm)
- System: [FAFOHive](https://github.com/coreyjames-ai/fafohive)

## Citation

Corey James. "AgentOS work tools." coreyjames.ai, 2026. https://coreyjames.ai/tools/agentos/

```bibtex
@misc{coreyjames-agentos,
  author = {Corey James},
  title = {AgentOS work tools},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/tools/agentos/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/tools/agentos}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
