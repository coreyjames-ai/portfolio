# The Migration Planner

**For an engineering lead who just read a vendor's deprecation notice.**

Canonical: https://coreyjames.ai/agents/roles/migration-planner/  
Author: Corey James · Published: 2026-11-11 · Kind: agent role  

## The story

The agent reads the documentation for the new version and finds every place the old interface is used. It sizes the change and maps what depends on each piece. Where the new version needs a different technique, it studies how a reference library does it and writes up the method for the team to implement. The result is a task plan in the order the work should happen.

## Function

[Engineering](https://coreyjames.ai/agents/functions/engineering/): Planning, building, reviewing and releasing software, with the reasoning kept.

## The crew

The specialists behind this role, grouped by the kind of work they do.

### Does the work

- [API Upgrade Planner](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/api-upgrade-planner) · [page](https://coreyjames.ai/agents/specialists/api-upgrade-planner/): Reads the documentation for the new version, finds every place the old interface is used, sizes the change, and drafts the task plan for the upgrade.
- [Legacy System Migration Planner](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/legacy-system-migration-planner) · [page](https://coreyjames.ai/agents/specialists/legacy-system-migration-planner/): This agent maps every step of the old system, compares it with the new design and produces the list of pieces to rebuild and in what order.
- [Project Planning Clerk](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/project-planning-clerk) · [page](https://coreyjames.ai/agents/specialists/project-planning-clerk/): It turns what you want done into a fully specified plan grounded in the real code and project, checks it before anyone begins, records the facts it relied on with two independent checks, and handles approved changes to a plan already under way.

### Challenges decisions

- [Plan Deliberation Panel](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/plan-deliberation-panel) · [page](https://coreyjames.ai/agents/specialists/plan-deliberation-panel/): Puts several models from different vendors in one structured debate that works through numbered plan revisions and ends only when all agree, then hands over a plan ready to execute.
- [Change Impact Reviewer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/change-impact-reviewer) · [page](https://coreyjames.ai/agents/specialists/change-impact-reviewer/): Maps everything a proposed change touches before anyone approves it and posts the impact summary on the merge request.
- [Platform Capability Reviewer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/platform-capability-reviewer) · [page](https://coreyjames.ai/agents/specialists/platform-capability-reviewer/): This agent compares what the platform's control layer and GPU servers can actually do with what the plans say, and closes each build stage with a written review.

### Keeps knowledge

- [Documentation Site Harvester](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/documentation-site-harvester) · [page](https://coreyjames.ai/agents/specialists/documentation-site-harvester/): Crawls a documentation website inside set domain and path boundaries, cleans each page into readable text, splits it into sections, writes a summary, keywords and a quality score for each section, and makes the whole site searchable.
- [Code Impact Analyst](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/code-impact-analyst) · [page](https://coreyjames.ai/agents/specialists/code-impact-analyst/): For every function or type a change touches, it lists what calls it and what it calls up to three steps out.
- [Porting Pattern Scout](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/porting-pattern-scout) · [page](https://coreyjames.ai/agents/specialists/porting-pattern-scout/): Finds how a reference library or specification solves a problem and where the team's own code would host the equivalent.

## Routes

- [A vendor notice becomes a finished upgrade](https://github.com/coreyjames-ai/portfolio/tree/main/agents/routes#a-vendor-notice-becomes-a-finished-upgrade) · [page](https://coreyjames.ai/agents/routes/#a-vendor-notice-becomes-a-finished-upgrade): The Migration Planner sizes the change and the Planning Room settles the approach. The Software Department builds it and the Change Board clears it.

## The engineering behind this role

- [Memory and code intelligence for agents](https://coreyjames.ai/capabilities/memory-and-code-intelligence-for-agents/): Capability

## Citation

Corey James. "The Migration Planner." coreyjames.ai, 2026. https://coreyjames.ai/agents/roles/migration-planner/

```bibtex
@misc{coreyjames-agent-role-migration-planner,
  author = {Corey James},
  title = {The Migration Planner},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/roles/migration-planner/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/migration-planner}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
