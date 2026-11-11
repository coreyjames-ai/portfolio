# The Second Opinion

**For a CTO who wants a critical system read by someone who did not build it.**

Canonical: https://coreyjames.ai/agents/roles/second-opinion/  
Author: Corey James · Published: 2026-11-11 · Kind: agent role  

## The story

Several reviewers from different AI model families read the system in parallel, and none of them may change anything. One works as an attacker. Their findings are merged, ranked by severity and handed over with the file and line for each.

## Function

[Engineering](https://coreyjames.ai/agents/functions/engineering/): Planning, building, reviewing and releasing software, with the reasoning kept.

## The crew

The specialists behind this role, grouped by the kind of work they do.

### Challenges decisions

- [Red Team Reviewer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/red-team-reviewer) · [page](https://coreyjames.ai/agents/specialists/red-team-reviewer/): Attacks every major decision and every change of scope from a different model family than the builders, looking for the assumption that breaks, and holds approval until it has answered.
- [Code-Grounded Reviewer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/code-grounded-reviewer) · [page](https://coreyjames.ai/agents/specialists/code-grounded-reviewer/): Reviews a team's claims about finished work with search access limited to that system's code, so every finding points to a file and line.
- [Independent Review Clerk](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/independent-review-clerk) · [page](https://coreyjames.ai/agents/specialists/independent-review-clerk/): It matches the verdict to the review that was requested and releases or holds the project exactly once.
- [Issue Review Panel](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/issue-review-panel) · [page](https://coreyjames.ai/agents/specialists/issue-review-panel/): It assigns AI advisors distinct roles (mediator, technical expert, security auditor, devil's advocate, referee, pragmatist and innovator), has them review an issue together, and follows the issue for changes.

### Audits and guards

- [Independent Code Auditor](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/independent-code-auditor) · [page](https://coreyjames.ai/agents/specialists/independent-code-auditor/): Audits a running system read-only in parallel tracks (interfaces, storage, runtime and deployment, test honesty) and reports every finding with file, line and severity against what the documentation claims.
- [Security Attack Tester](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/security-attack-tester) · [page](https://coreyjames.ai/agents/specialists/security-attack-tester/): Throws command injection, path traversal, header injection, forbidden schemes, forged identities and runaway tool chains at every tool and fails the build if any attack gets through.
- [Dead Code Finder](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/dead-code-finder) · [page](https://coreyjames.ai/agents/specialists/dead-code-finder/): Lists functions and types that nothing appears to call, as candidates for a person to review.

## Routes

- [An acquisition becomes a working team](https://github.com/coreyjames-ai/portfolio/tree/main/agents/routes#an-acquisition-becomes-a-working-team) · [page](https://coreyjames.ai/agents/routes/#an-acquisition-becomes-a-working-team): The Due-Diligence Analyst reads the codebase. The Second Opinion audits it, the Company Librarian files the documents and the Onboarding Buddy brings each engineer up to speed.

## The engineering behind this role

- [Governed autonomous engineering](https://coreyjames.ai/capabilities/governed-autonomous-engineering/): Capability
- [Role contracts, with vendors as data](https://coreyjames.ai/ideas/role-contracts-not-vendors/): Idea
- [Separation of duties for AI work](https://coreyjames.ai/stories/separation-of-duties-for-ai-work/): Engineering story

## Citation

Corey James. "The Second Opinion." coreyjames.ai, 2026. https://coreyjames.ai/agents/roles/second-opinion/

```bibtex
@misc{coreyjames-agent-role-second-opinion,
  author = {Corey James},
  title = {The Second Opinion},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/roles/second-opinion/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/second-opinion}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
