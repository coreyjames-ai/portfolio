# The Ticket Clearer

**For an engineering manager with a queue of small tickets.**

Canonical: https://coreyjames.ai/agents/roles/ticket-clearer/  
Author: Corey James · Published: 2026-11-11 · Kind: agent role  

## The story

The agent takes a ticket, finds the code, makes the change and runs the build and tests. A second agent reviews the change against the ticket. The manager gets a merge request that is ready to approve, and the ticket is updated either way.

## Function

[Engineering](https://coreyjames.ai/agents/functions/engineering/): Planning, building, reviewing and releasing software, with the reasoning kept.

## The crew

The specialists behind this role, grouped by the kind of work they do.

### Does the work

- [Issue Triage Engineer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/issue-triage-engineer) · [page](https://coreyjames.ai/agents/specialists/issue-triage-engineer/): Reads each new issue, finds the code most likely at fault and comments the suspect file and line with a triage label so a developer starts in the right place.
- [Ticket-to-Fix Engineer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/ticket-to-fix-engineer) · [page](https://coreyjames.ai/agents/specialists/ticket-to-fix-engineer/): This agent picks up a new ticket, makes the change, checks it, opens a merge request and leaves a note on the ticket so the requester knows it is ready for review.
- [Build and Test Runner](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/build-and-test-runner) · [page](https://coreyjames.ai/agents/specialists/build-and-test-runner/): Runs a compile check and the test suite in order, stops at the first failure and checks the service health endpoint afterwards.
- [Repository Steward](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/repository-steward) · [page](https://coreyjames.ai/agents/specialists/repository-steward/): Holds the repository keys, checks who is asking and what branch they offer, opens merge requests for human review and keeps issues, comments and labels in order.
- [Credential-Free Contributor](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/credential-free-contributor) · [page](https://coreyjames.ai/agents/specialists/credential-free-contributor/): Clones a repository, makes and tests a change on its own branch and asks a trusted steward to open the merge request, never holding the repository key itself.
- [Repository Assistant](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/repository-assistant) · [page](https://coreyjames.ai/agents/specialists/repository-assistant/): This agent keeps tickets, comments, branches and merge requests in order so developers spend their time on the code.
- [Issue Change Watcher](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/issue-change-watcher) · [page](https://coreyjames.ai/agents/specialists/issue-change-watcher/): It reports what changed since the last check.

### Challenges decisions

- [Code Reviewer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/code-reviewer) · [page](https://coreyjames.ai/agents/specialists/code-reviewer/): Reviews finished code and reports against the plan, lists what is missing, extra or wrong with file and line, freezes the list after the first pass and then checks only the fixes.

### Audits and guards

- [Acceptance Checker](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/acceptance-checker) · [page](https://coreyjames.ai/agents/specialists/acceptance-checker/): Checks the facts of the finished work against each acceptance point, refuses claims that are only narrative, and either signs the item off or returns a precise fix list.
- [Vulnerability Triage Analyst](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/vulnerability-triage-analyst) · [page](https://coreyjames.ai/agents/specialists/vulnerability-triage-analyst/): This agent checks a new advisory against what is actually installed and configured, writes a plain verdict on exposure and texts the on-call person if action is needed.

## Routes

- [A complaint becomes a release](https://github.com/coreyjames-ai/portfolio/tree/main/agents/routes#a-complaint-becomes-a-release) · [page](https://coreyjames.ai/agents/routes/#a-complaint-becomes-a-release): The Support Desk finds a defect and files it. The Ticket Clearer fixes it, the Change Board clears it, and the Training Department remakes the help video. The Support Desk tells the customer it shipped.

## The engineering behind this role

- [Governed autonomous engineering](https://coreyjames.ai/capabilities/governed-autonomous-engineering/): Capability
- [A coding agent that never holds the keys](https://coreyjames.ai/stories/a-coding-agent-that-never-holds-the-keys/): Engineering story

## Citation

Corey James. "The Ticket Clearer." coreyjames.ai, 2026. https://coreyjames.ai/agents/roles/ticket-clearer/

```bibtex
@misc{coreyjames-agent-role-ticket-clearer,
  author = {Corey James},
  title = {The Ticket Clearer},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/roles/ticket-clearer/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/ticket-clearer}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
