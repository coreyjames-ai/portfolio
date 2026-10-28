# Agent365



Canonical: https://coreyjames.ai/tools/agent365/  
Author: Corey James · Published: 2026-10-28 · Kind: tool group  
Systems: [Helix](https://github.com/coreyjames-ai/helix) · [FAFOHive](https://github.com/coreyjames-ai/fafohive)  

## What was built

My digital employees work inside Microsoft Teams as colleagues with their own identities, and an AI model needs tools to do that: join the meeting, speak up in chat, raise a hand, put a deck on screen, write a document and remember what was decided. This server gives it those tools. Every action names the exact digital employee it acts as, and the server resolves that employee's identity itself. Microsoft stays the authority on what the employee may do, so the server adds capability without adding a second permission system. The employees and their voice are described on the [Helix](https://coreyjames.ai/systems/helix) page, and [a self-hosted colleague in a Teams call](https://coreyjames.ai/stories/a-self-hosted-colleague-in-a-teams-call) tells the story.

## Identity

`agent365_employees` lists the digital employees with their names, personas, addresses and identities. An agent calls it first to get the identifier every other tool needs.

## Meetings and chat

`teams_meeting_join` brings an employee into a Teams meeting from its invitation link, as its own participant.

`teams_meeting_leave` takes the employee out of the meeting and ends any sharing or presentation it was running.

`teams_chat_send` posts a message or an approved link in the meeting chat.

`teams_hand_raise` is a typed refusal: the server will not raise the employee's own hand until Microsoft's authority to do so on the employee's behalf is proven, and it says so rather than pretending.

`teams_hand_lower` lowers one attendee's hand, so a facilitator can clear a request to speak that has been handled.

## Presenting

`teams_presentation_start` presents one of the employee's approved PowerPoint decks on the meeting stage.

`teams_presentation_next` moves the deck forward one slide.

`teams_presentation_previous` moves it back one slide.

`teams_presentation_show` jumps to a numbered slide.

`teams_presentation_stop` ends the presentation and leaves the employee in the call.

## Screen sharing

`teams_screen_share_start` shares a live desktop, browser or terminal from the employee's own workspace into the meeting, opening a chosen page or showing chosen content.

`teams_screen_share_update` changes the live share in place: another surface, another page, or new terminal content.

`teams_screen_share_stop` ends the screen share and leaves the employee in the meeting. A running presentation can carry on.

## Documents

Documents are Markdown files the employee publishes into its conversation in Mattermost, with every version kept.

`markdown_create` publishes a new Markdown document into the current conversation.

`markdown_create_version` publishes a full new version of an existing document. A revision check stops an edit based on an out-of-date copy.

`markdown_read` reads the current text of a Markdown document in the conversation.

`document_versions` lists a document's version history.

`document_delete` deletes a document and all of its versions, with the same revision check.

`workspace_files` finds files already attached to the conversation, with their type, indexing state and version details.

## Grounding

Grounding is the employee's working memory, organised in scopes from a whole system down to one work order, participant or private conversation.

`grounding_read` loads a bounded briefing for a scope: its ancestry, recent activity, durable records and which sources are ready.

`grounding_search` searches the sources available to a scope, optionally including its parents or children, and can narrow to decisions, code, references, files or activity.

`grounding_record` stores a decision, constraint, discovery, question, checkpoint or outcome in a scope. A stable key stops a retry from storing it twice.

`grounding_system_create` creates the grounding scope for a new workspace and its working folder, linking existing code indexes, the chat team and the work-order system when they are given.

The judgment in this server is restraint. It gives an AI colleague the same handful of things a person does in a meeting, and lets Microsoft's identity model decide who that colleague is allowed to be.

## What was verified

Each line is a claim the canonical page supports, with the figure as the page states it.

- Microsoft Teams agent tooling: 24 tools that let a digital employee join a Teams meeting as its own participant, speak in chat, present a deck, write documents and remember decisions.
- Identity for AI agents in Microsoft 365: every action names the exact digital employee it acts as, the server resolves its Entra identity, and Microsoft stays the authority on what it may do.

## Related

- [A self-hosted colleague in a Teams call](https://github.com/coreyjames-ai/helix/tree/main/stories/a-self-hosted-colleague-in-a-teams-call) · https://coreyjames.ai/stories/a-self-hosted-colleague-in-a-teams-call/
- System: [Helix](https://github.com/coreyjames-ai/helix)
- System: [FAFOHive](https://github.com/coreyjames-ai/fafohive)

## Citation

Corey James. "Agent365." coreyjames.ai, 2026. https://coreyjames.ai/tools/agent365/

```bibtex
@misc{coreyjames-agent365,
  author = {Corey James},
  title = {Agent365},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/tools/agent365/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/tools/agent365}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
