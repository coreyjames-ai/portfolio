# The Contractor Pass

**For a team that wants outside or automated contributors without handing over the keys.**

Canonical: https://coreyjames.ai/agents/roles/contractor-pass/  
Author: Corey James · Published: 2026-11-11 · Kind: agent role  

## The story

A contributor agent clones the repository, makes its change on its own branch and runs the tests. It never holds the repository key. A trusted steward opens the merge request for it, a reviewer reads the change and an assistant keeps the tickets, branches and comments in order.

## Function

[Engineering](https://coreyjames.ai/agents/functions/engineering/): Planning, building, reviewing and releasing software, with the reasoning kept.

## The crew

The specialists behind this role, grouped by the kind of work they do.

### Does the work

- [Credential-Free Contributor](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/credential-free-contributor) · [page](https://coreyjames.ai/agents/specialists/credential-free-contributor/): Clones a repository, makes and tests a change on its own branch and asks a trusted steward to open the merge request, never holding the repository key itself.
- [Repository Steward](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/repository-steward) · [page](https://coreyjames.ai/agents/specialists/repository-steward/): Holds the repository keys, checks who is asking and what branch they offer, opens merge requests for human review and keeps issues, comments and labels in order.
- [Repository Assistant](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/repository-assistant) · [page](https://coreyjames.ai/agents/specialists/repository-assistant/): This agent keeps tickets, comments, branches and merge requests in order so developers spend their time on the code.
- [Build and Test Runner](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/build-and-test-runner) · [page](https://coreyjames.ai/agents/specialists/build-and-test-runner/): Runs a compile check and the test suite in order, stops at the first failure and checks the service health endpoint afterwards.

### Challenges decisions

- [Code Reviewer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/code-reviewer) · [page](https://coreyjames.ai/agents/specialists/code-reviewer/): Reviews finished code and reports against the plan, lists what is missing, extra or wrong with file and line, freezes the list after the first pass and then checks only the fixes.
- [Test Coverage Reviewer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/test-coverage-reviewer) · [page](https://coreyjames.ai/agents/specialists/test-coverage-reviewer/): Checks whether a change comes with tests for the cases that matter and names the cases left untested.

### Audits and guards

- [Acceptance Tester](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/acceptance-tester) · [page](https://coreyjames.ai/agents/specialists/acceptance-tester/): Before new code joins the product, this agent runs the acceptance checks and refuses anything that contains placeholder code or skipped steps.
- [Secrets and Certificates Officer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/secrets-and-certificates-officer) · [page](https://coreyjames.ai/agents/specialists/secrets-and-certificates-officer/): Keeps every credential and certificate in one locked store.
- [App Access Registrar](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/app-access-registrar) · [page](https://coreyjames.ai/agents/specialists/app-access-registrar/): This agent signs up new client apps, issues their credentials, enrols passkeys and manages registrations afterwards, keeping an audit trail of every step.

## The engineering behind this role

- [Governed autonomous engineering](https://coreyjames.ai/capabilities/governed-autonomous-engineering/): Capability
- [Identity from the caller, credentials on the server](https://coreyjames.ai/ideas/identity-from-the-caller/): Idea
- [A coding agent that never holds the keys](https://coreyjames.ai/stories/a-coding-agent-that-never-holds-the-keys/): Engineering story

## Citation

Corey James. "The Contractor Pass." coreyjames.ai, 2026. https://coreyjames.ai/agents/roles/contractor-pass/

```bibtex
@misc{coreyjames-agent-role-contractor-pass,
  author = {Corey James},
  title = {The Contractor Pass},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/roles/contractor-pass/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/contractor-pass}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
