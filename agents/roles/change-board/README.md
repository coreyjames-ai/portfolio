# The Change Board

**For a manager about to approve a risky change.**

Canonical: https://coreyjames.ai/agents/roles/change-board/  
Author: Corey James · Published: 2026-11-11 · Kind: agent role  

## The story

Before the change goes in, the agent maps everything that calls the code being touched and everything it calls. It pulls the history of that area, including what broke the last time someone changed it. The manager reads one page: what the change reaches, what could fail and what to test.

## Function

[Engineering](https://coreyjames.ai/agents/functions/engineering/): Planning, building, reviewing and releasing software, with the reasoning kept.

## The crew

The specialists behind this role, grouped by the kind of work they do.

### Does the work

- [Scope Change Manager](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/scope-change-manager) · [page](https://coreyjames.ai/agents/specialists/scope-change-manager/): Handles a mid-project change from proposal to approval: it maps what the change touches, gets an architect's proposal, an independent ruling and a hostile second look, then folds the approved change into the live plan.

### Challenges decisions

- [Change Risk Reviewer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/change-risk-reviewer) · [page](https://coreyjames.ai/agents/specialists/change-risk-reviewer/): Before a change goes in, this agent works out how risky it is from what it touches, maps everything that depends on it and asks for the matching level of checking.
- [Change Impact Reviewer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/change-impact-reviewer) · [page](https://coreyjames.ai/agents/specialists/change-impact-reviewer/): Maps everything a proposed change touches before anyone approves it and posts the impact summary on the merge request.
- [Independent Review Clerk](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/independent-review-clerk) · [page](https://coreyjames.ai/agents/specialists/independent-review-clerk/): It matches the verdict to the review that was requested and releases or holds the project exactly once.
- [Performance Reviewer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/performance-reviewer) · [page](https://coreyjames.ai/agents/specialists/performance-reviewer/): Reads a change for slow paths and wasted work and reports them on the ticket with the lines concerned.

### Keeps knowledge

- [Code Impact Analyst](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/code-impact-analyst) · [page](https://coreyjames.ai/agents/specialists/code-impact-analyst/): For every function or type a change touches, it lists what calls it and what it calls up to three steps out.
- [Code Flow Explainer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/code-flow-explainer) · [page](https://coreyjames.ai/agents/specialists/code-flow-explainer/): Takes a starting point (a file and line, a function name or a plain question), traces how the work flows through the code, and explains it in plain language.
- [Regression Historian](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/regression-historian) · [page](https://coreyjames.ai/agents/specialists/regression-historian/): Given a broken function or an error, works out which pieces of work touched that area and in what order, who calls it now, and how the failure travels through the code.
- [System Historian](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/system-historian) · [page](https://coreyjames.ai/agents/specialists/system-historian/): Reconstructs a system's story, covering the decisions that shaped it, the changes made, the problems hit and how each was fixed, and the trade-offs accepted, in time order.

## Routes

- [A complaint becomes a release](https://github.com/coreyjames-ai/portfolio/tree/main/agents/routes#a-complaint-becomes-a-release) · [page](https://coreyjames.ai/agents/routes/#a-complaint-becomes-a-release): The Support Desk finds a defect and files it. The Ticket Clearer fixes it, the Change Board clears it, and the Training Department remakes the help video. The Support Desk tells the customer it shipped.
- [A vendor notice becomes a finished upgrade](https://github.com/coreyjames-ai/portfolio/tree/main/agents/routes#a-vendor-notice-becomes-a-finished-upgrade) · [page](https://coreyjames.ai/agents/routes/#a-vendor-notice-becomes-a-finished-upgrade): The Migration Planner sizes the change and the Planning Room settles the approach. The Software Department builds it and the Change Board clears it.

## The engineering behind this role

- [Memory and code intelligence for agents](https://coreyjames.ai/capabilities/memory-and-code-intelligence-for-agents/): Capability
- [Compute first, narrate second](https://coreyjames.ai/ideas/compute-first-narrate-second/): Idea
- [A code explainer that is not allowed to invent](https://coreyjames.ai/stories/a-code-explainer-that-is-not-allowed-to-invent/): Engineering story

## Citation

Corey James. "The Change Board." coreyjames.ai, 2026. https://coreyjames.ai/agents/roles/change-board/

```bibtex
@misc{coreyjames-agent-role-change-board,
  author = {Corey James},
  title = {The Change Board},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/roles/change-board/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/change-board}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
