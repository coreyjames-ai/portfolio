# The Review Panel

**For a tech lead who wants every change read by more than one specialist.**

Canonical: https://coreyjames.ai/agents/roles/review-panel/  
Author: Corey James · Published: 2026-11-11 · Kind: agent role  

## The story

Each change is read four times, for design, speed, documentation and tests. Every reviewer writes its findings on the ticket with the lines concerned. When the reviewers disagree and cannot settle it, the ticket is marked for a person, with the disagreement summarised. The lead also hears when a tracked ticket gets a new comment, label or due date.

## Function

[Engineering](https://coreyjames.ai/agents/functions/engineering/): Planning, building, reviewing and releasing software, with the reasoning kept.

## The crew

The specialists behind this role, grouped by the kind of work they do.

### Does the work

- [Issue Change Watcher](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/issue-change-watcher) · [page](https://coreyjames.ai/agents/specialists/issue-change-watcher/): It reports what changed since the last check.

### Supervises other agents

- [Quality Fix Coordinator](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/quality-fix-coordinator) · [page](https://coreyjames.ai/agents/specialists/quality-fix-coordinator/): It records what must be fixed against each failed criterion, assigns the fix, and sends the work back for review.

### Challenges decisions

- [Architecture Reviewer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/architecture-reviewer) · [page](https://coreyjames.ai/agents/specialists/architecture-reviewer/): Reads a proposed change for how it fits the existing design and writes its findings on the ticket.
- [Performance Reviewer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/performance-reviewer) · [page](https://coreyjames.ai/agents/specialists/performance-reviewer/): Reads a change for slow paths and wasted work and reports them on the ticket with the lines concerned.
- [Documentation Reviewer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/documentation-reviewer) · [page](https://coreyjames.ai/agents/specialists/documentation-reviewer/): Checks that the documentation for a change matches what the code now does and lists what is missing.
- [Test Coverage Reviewer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/test-coverage-reviewer) · [page](https://coreyjames.ai/agents/specialists/test-coverage-reviewer/): Checks whether a change comes with tests for the cases that matter and names the cases left untested.
- [Code-Grounded Reviewer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/code-grounded-reviewer) · [page](https://coreyjames.ai/agents/specialists/code-grounded-reviewer/): Reviews a team's claims about finished work with search access limited to that system's code, so every finding points to a file and line.

### Audits and guards

- [Human Escalation Flagger](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/human-escalation-flagger) · [page](https://coreyjames.ai/agents/specialists/human-escalation-flagger/): Marks a ticket as needing a person when the AI reviewers cannot settle it, with a summary of the disagreement.

## The engineering behind this role

- [Governed autonomous engineering](https://coreyjames.ai/capabilities/governed-autonomous-engineering/): Capability
- [Role contracts, with vendors as data](https://coreyjames.ai/ideas/role-contracts-not-vendors/): Idea

## Citation

Corey James. "The Review Panel." coreyjames.ai, 2026. https://coreyjames.ai/agents/roles/review-panel/

```bibtex
@misc{coreyjames-agent-role-review-panel,
  author = {Corey James},
  title = {The Review Panel},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/roles/review-panel/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/review-panel}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
