# The Due-Diligence Analyst

**For a CTO inheriting or acquiring a codebase.**

Canonical: https://coreyjames.ai/agents/roles/due-diligence-analyst/  
Author: Corey James · Published: 2026-11-11 · Kind: agent role  

## The story

The agent takes the repository in, maps how it fits together and compares the documentation with what the code does. It lists what the system can do, what is dead and what would be expensive to change. The findings come as a written report and a briefing the agent presents in a meeting.

## Function

[Engineering](https://coreyjames.ai/agents/functions/engineering/): Planning, building, reviewing and releasing software, with the reasoning kept.

## The crew

The specialists behind this role, grouped by the kind of work they do.

### Speaks to people

- [Board Briefing Presenter](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/board-briefing-presenter) · [page](https://coreyjames.ai/agents/specialists/board-briefing-presenter/): It turns an agreed plan into a briefing deck, joins the video meeting as a named digital colleague, presents the deck slide by slide, and drops the plan link into the meeting chat.

### Challenges decisions

- [Platform Capability Reviewer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/platform-capability-reviewer) · [page](https://coreyjames.ai/agents/specialists/platform-capability-reviewer/): This agent compares what the platform's control layer and GPU servers can actually do with what the plans say, and closes each build stage with a written review.
- [Architecture Reviewer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/architecture-reviewer) · [page](https://coreyjames.ai/agents/specialists/architecture-reviewer/): Reads a proposed change for how it fits the existing design and writes its findings on the ticket.

### Keeps knowledge

- [Codebase Intake Engineer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/codebase-intake-engineer) · [page](https://coreyjames.ai/agents/specialists/codebase-intake-engineer/): Brings a codebase in from a local folder or straight from GitHub or GitLab, recommends which file types to include, splits the code along function and type boundaries for eight languages, and makes it searchable by meaning and by name.
- [Code Map Builder](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/code-map-builder) · [page](https://coreyjames.ai/agents/specialists/code-map-builder/): Builds and maintains the dependency map: calls, imports, implementations, references, definitions and re-exports.
- [Technical Due-diligence Researcher](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/technical-due-diligence-researcher) · [page](https://coreyjames.ai/agents/specialists/technical-due-diligence-researcher/): It surveys a large codebase without changing it and writes structured findings, a source list, open questions and an area report for each part of the estate.

### Audits and guards

- [Documentation Drift Auditor](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/documentation-drift-auditor) · [page](https://coreyjames.ai/agents/specialists/documentation-drift-auditor/): Compares what internal documents say with what the code actually does and lists each mismatch with the document section and the file and line.
- [Dead Code Finder](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/dead-code-finder) · [page](https://coreyjames.ai/agents/specialists/dead-code-finder/): Lists functions and types that nothing appears to call, as candidates for a person to review.
- [Independent Code Auditor](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/independent-code-auditor) · [page](https://coreyjames.ai/agents/specialists/independent-code-auditor/): Audits a running system read-only in parallel tracks (interfaces, storage, runtime and deployment, test honesty) and reports every finding with file, line and severity against what the documentation claims.

## Routes

- [An acquisition becomes a working team](https://github.com/coreyjames-ai/portfolio/tree/main/agents/routes#an-acquisition-becomes-a-working-team) · [page](https://coreyjames.ai/agents/routes/#an-acquisition-becomes-a-working-team): The Due-Diligence Analyst reads the codebase. The Second Opinion audits it, the Company Librarian files the documents and the Onboarding Buddy brings each engineer up to speed.

## The engineering behind this role

- [Memory and code intelligence for agents](https://coreyjames.ai/capabilities/memory-and-code-intelligence-for-agents/): Capability

## Citation

Corey James. "The Due-Diligence Analyst." coreyjames.ai, 2026. https://coreyjames.ai/agents/roles/due-diligence-analyst/

```bibtex
@misc{coreyjames-agent-role-due-diligence-analyst,
  author = {Corey James},
  title = {The Due-Diligence Analyst},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/roles/due-diligence-analyst/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/due-diligence-analyst}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
