# The Software Department

**For a founder with a large build and a small team.**

Canonical: https://coreyjames.ai/agents/roles/software-department/  
Author: Corey James · Published: 2026-11-11 · Kind: agent role  

## The story

Someone types a feature request into chat. A planner turns it into a plan, a panel of different models argues the design until they agree, and developers who can search the whole codebase and see what a change will break build it. A reviewer checks the result against the plan, a red team tries to break it and a spend guard refuses any compute past the limit the owner set. The requester gets working software and a record of why each decision was made.

## Function

[Engineering](https://coreyjames.ai/agents/functions/engineering/): Planning, building, reviewing and releasing software, with the reasoning kept.

## The crew

The specialists behind this role, grouped by the kind of work they do.

### Does the work

- [Software Delivery Crew](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/software-delivery-crew) · [page](https://coreyjames.ai/agents/specialists/software-delivery-crew/): This crew of five takes a plan and turns it into working code: a planner writes the tasks, a builder writes the code, a reviewer reads every critical path, a researcher answers "what else does this touch", and an inspector checks the finished work before it is accepted.
- [Project Planner](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/project-planner) · [page](https://coreyjames.ai/agents/specialists/project-planner/): Turns a goal into a scoped project plan with acceptance criteria, a task breakdown, who may change which files and a staffed team, and hands it back for one yes or no.
- [Software Developer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/software-developer) · [page](https://coreyjames.ai/agents/specialists/software-developer/): Takes one assigned task, reads the brief and the code around it, writes and tests the change inside its allowed folders, submits evidence for each acceptance point and fixes what reviewers send back.
- [Release Engineer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/release-engineer) · [page](https://coreyjames.ai/agents/specialists/release-engineer/): Screens each candidate change for benchmark gaming, builds release images from pinned inputs, checks every hash, compares the candidate with the current baseline and promotes it, then tells the other teams to rebase.
- [Project Closer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/project-closer) · [page](https://coreyjames.ai/agents/specialists/project-closer/): Closes a project, phase or program only when every required item carries a current sign-off, writes the closing summary with cost, archives the team and retires everything it opened.

### Challenges decisions

- [Plan Deliberation Panel](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/plan-deliberation-panel) · [page](https://coreyjames.ai/agents/specialists/plan-deliberation-panel/): Puts several models from different vendors in one structured debate that works through numbered plan revisions and ends only when all agree, then hands over a plan ready to execute.
- [Code Reviewer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/code-reviewer) · [page](https://coreyjames.ai/agents/specialists/code-reviewer/): Reviews finished code and reports against the plan, lists what is missing, extra or wrong with file and line, freezes the list after the first pass and then checks only the fixes.
- [Red Team Reviewer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/red-team-reviewer) · [page](https://coreyjames.ai/agents/specialists/red-team-reviewer/): Attacks every major decision and every change of scope from a different model family than the builders, looking for the assumption that breaks, and holds approval until it has answered.

### Keeps knowledge

- [Code Impact Analyst](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/code-impact-analyst) · [page](https://coreyjames.ai/agents/specialists/code-impact-analyst/): For every function or type a change touches, it lists what calls it and what it calls up to three steps out.
- [Decision Recorder](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/decision-recorder) · [page](https://coreyjames.ai/agents/specialists/decision-recorder/): Watches the team's decisions log and working notes folder.

### Audits and guards

- [Acceptance Checker](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/acceptance-checker) · [page](https://coreyjames.ai/agents/specialists/acceptance-checker/): Checks the facts of the finished work against each acceptance point, refuses claims that are only narrative, and either signs the item off or returns a precise fix list.
- [Compute Budget Guardian](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/compute-budget-guardian) · [page](https://coreyjames.ai/agents/specialists/compute-budget-guardian/): Holds the line on the daily spend that only you set: it refuses any start the budget cannot cover and says why, warns you as spend climbs, and stops paid machines at the cap.

## Routes

- [A meeting becomes shipped software](https://github.com/coreyjames-ai/portfolio/tree/main/agents/routes#a-meeting-becomes-shipped-software) · [page](https://coreyjames.ai/agents/routes/#a-meeting-becomes-shipped-software): The Chief of Staff's minutes contain a feature request. The Software Department builds it, and the Presenter demonstrates it at the next meeting.
- [A vendor notice becomes a finished upgrade](https://github.com/coreyjames-ai/portfolio/tree/main/agents/routes#a-vendor-notice-becomes-a-finished-upgrade) · [page](https://coreyjames.ai/agents/routes/#a-vendor-notice-becomes-a-finished-upgrade): The Migration Planner sizes the change and the Planning Room settles the approach. The Software Department builds it and the Change Board clears it.

## The engineering behind this role

- [Governed autonomous engineering](https://coreyjames.ai/capabilities/governed-autonomous-engineering/): Capability
- [AI subscriptions as governed workers](https://coreyjames.ai/capabilities/use-the-ai-subscriptions-you-already-have/): Capability
- [Role contracts, with vendors as data](https://coreyjames.ai/ideas/role-contracts-not-vendors/): Idea
- [Budgets and refusals](https://coreyjames.ai/ideas/budgets-and-refusals/): Idea
- [Separation of duties for AI work](https://coreyjames.ai/stories/separation-of-duties-for-ai-work/): Engineering story
- [Directing AI coding agents at program scale](https://coreyjames.ai/stories/directing-ai-coding-agents-at-program-scale/): Engineering story

## Citation

Corey James. "The Software Department." coreyjames.ai, 2026. https://coreyjames.ai/agents/roles/software-department/

```bibtex
@misc{coreyjames-agent-role-software-department,
  author = {Corey James},
  title = {The Software Department},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/roles/software-department/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/software-department}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
