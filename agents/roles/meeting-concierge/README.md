# The Meeting Concierge

**For a team lead whose meetings end with "someone should look into that".**

Canonical: https://coreyjames.ai/agents/roles/meeting-concierge/  
Author: Corey James · Published: 2026-11-11 · Kind: agent role  

## The story

The agent books the meeting with an agenda and makes sure it is recorded. During the call someone asks for a number or a document. The agent starts a worker on the request while the meeting continues and posts the result in the meeting chat before people leave. Afterwards a panel reconciles what was decided and what is still open, and the minutes go out as a document.

## Function

[Running the company](https://coreyjames.ai/agents/functions/running-the-company/): The owner's side of the business: meetings, decisions, briefings and the work that follows them.

## The crew

The specialists behind this role, grouped by the kind of work they do.

### Does the work

- [Meeting Follow-through Agent](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/meeting-follow-through-agent) · [page](https://coreyjames.ai/agents/specialists/meeting-follow-through-agent/): It takes the request, runs the work on a worker while the meeting continues, posts the result in the meeting chat, and records the item in the minutes.
- [Teams Work Request Runner](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/teams-work-request-runner) · [page](https://coreyjames.ai/agents/specialists/teams-work-request-runner/): It starts a worker on a local machine or in the cloud, keeps the requester informed of progress, returns the results and files, and shuts the worker down when idle.
- [Background Task Worker](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/background-task-worker) · [page](https://coreyjames.ai/agents/specialists/background-task-worker/): Takes a task from chat or voice, does the file or code work in its own isolated workspace, reports back, picks the same thread up later, and shuts itself down when idle so it costs nothing.
- [Meeting Follow-up Engineer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/meeting-follow-up-engineer) · [page](https://coreyjames.ai/agents/specialists/meeting-follow-up-engineer/): Takes the meeting transcript and pulls out the engineering action items.

### Speaks to people

- [Meeting Scheduler](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/meeting-scheduler) · [page](https://coreyjames.ai/agents/specialists/meeting-scheduler/): Books the meeting with a clear purpose and agenda, makes sure it will be recorded and transcribed, and shows up when it starts.
- [Meeting Recap Producer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/meeting-recap-producer) · [page](https://coreyjames.ai/agents/specialists/meeting-recap-producer/): Joins a meeting as its own participant, keeps the transcript, and after the call returns a short narrated recap video with captions, posting the link in the meeting chat.
- [Action-Item Chaser](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/action-item-chaser) · [page](https://coreyjames.ai/agents/specialists/action-item-chaser/): Pulls every promise made in a meeting into a list with owners and due dates, then nudges each owner by chat until the item is done.

### Keeps knowledge

- [Meeting Decision Recorder](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/meeting-decision-recorder) · [page](https://coreyjames.ai/agents/specialists/meeting-decision-recorder/): After the meeting it takes the transcript, has a panel reconcile what was decided and what is still open, records each decision in the project's memory, and posts the minutes as a document.
- [Meeting Minute-Taker](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/meeting-minute-taker) · [page](https://coreyjames.ai/agents/specialists/meeting-minute-taker/): Takes the minutes after every meeting from the recording and transcript, and sends everyone the same version, updating it when someone points out a correction.

## The engineering behind this role

- [AI teammates inside Microsoft Teams and team chat](https://coreyjames.ai/capabilities/ai-teammates-in-teams-and-chat/): Capability
- [A meeting attendee that will not fake it](https://coreyjames.ai/stories/a-meeting-attendee-that-will-not-fake-it/): Engineering story

## Citation

Corey James. "The Meeting Concierge." coreyjames.ai, 2026. https://coreyjames.ai/agents/roles/meeting-concierge/

```bibtex
@misc{coreyjames-agent-role-meeting-concierge,
  author = {Corey James},
  title = {The Meeting Concierge},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/roles/meeting-concierge/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/meeting-concierge}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
