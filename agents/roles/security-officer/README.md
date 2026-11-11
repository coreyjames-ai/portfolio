# The Security Officer

**For a security lead.**

Canonical: https://coreyjames.ai/agents/roles/security-officer/  
Author: Corey James · Published: 2026-11-11 · Kind: agent role  

## The story

The agent issues and rotates certificates and secrets, registers each application that wants access and manages sign-in tokens. It hunts the sign-in records for takeover attempts. When a new advisory lands, it checks whether the company is exposed. It also attacks the company's own AI tools to find what an agent could be tricked into running.

## Function

[Infrastructure and operations](https://coreyjames.ai/agents/functions/infrastructure-and-operations/): Machines, queues, databases and spend, watched through the night.

## The crew

The specialists behind this role, grouped by the kind of work they do.

### Supervises other agents

- [Emergency Stop Officer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/emergency-stop-officer) · [page](https://coreyjames.ai/agents/specialists/emergency-stop-officer/): Stops one agent or every agent in a given role at once, records what was running and confirms nothing is left.

### Runs infrastructure

- [Remote Machine Rebuilder](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/remote-machine-rebuilder) · [page](https://coreyjames.ai/agents/specialists/remote-machine-rebuilder/): Removes a remote machine, rejoins it from a clean state with the standard images and setup, starts the agents it should host, and has an independent reviewer check the result against a checklist.
- [Machine Decommissioner](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/machine-decommissioner) · [page](https://coreyjames.ai/agents/specialists/machine-decommissioner/): Takes a retired machine out of the fleet, revokes its certificates and confirms nothing still routes work to it.

### Audits and guards

- [Secrets and Certificates Officer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/secrets-and-certificates-officer) · [page](https://coreyjames.ai/agents/specialists/secrets-and-certificates-officer/): Keeps every credential and certificate in one locked store.
- [App Access Registrar](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/app-access-registrar) · [page](https://coreyjames.ai/agents/specialists/app-access-registrar/): This agent signs up new client apps, issues their credentials, enrols passkeys and manages registrations afterwards, keeping an audit trail of every step.
- [Sign-in and Token Manager](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/sign-in-and-token-manager) · [page](https://coreyjames.ai/agents/specialists/sign-in-and-token-manager/): This agent handles sign-in codes, access tokens and refresh tokens end to end and keeps the site's security certificate renewed.
- [Sign-in Threat Hunter](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/sign-in-threat-hunter) · [page](https://coreyjames.ai/agents/specialists/sign-in-threat-hunter/): This agent watches sign-in traffic for attacks, recognises devices, slows or blocks suspicious sources, keeps a tamper-evident audit trail and raises alerts with a security dashboard.
- [Vulnerability Triage Analyst](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/vulnerability-triage-analyst) · [page](https://coreyjames.ai/agents/specialists/vulnerability-triage-analyst/): This agent checks a new advisory against what is actually installed and configured, writes a plain verdict on exposure and texts the on-call person if action is needed.
- [Security Attack Tester](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/security-attack-tester) · [page](https://coreyjames.ai/agents/specialists/security-attack-tester/): Throws command injection, path traversal, header injection, forbidden schemes, forged identities and runaway tool chains at every tool and fails the build if any attack gets through.
- [Secret Access Auditor](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/secret-access-auditor) · [page](https://coreyjames.ai/agents/specialists/secret-access-auditor/): Lists every stored credential with the roles and machines allowed to use it.
- [Credential Rotation Clerk](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/credential-rotation-clerk) · [page](https://coreyjames.ai/agents/specialists/credential-rotation-clerk/): Replaces a stored credential in one step, sends the new one to each machine that needs it and removes the retired one.
- [AI Access Desk](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/ai-access-desk) · [page](https://coreyjames.ai/agents/specialists/ai-access-desk/): Registers each AI assistant as an app, holds every grant until a person approves it, accepts sign-in tokens from your own server and from your workplace platform, shows each assistant only the tools it is allowed, and ties every action to the assignment rather than to what the assistant claims.

## The engineering behind this role

- [Business systems as safe agent tools](https://coreyjames.ai/capabilities/business-systems-as-safe-agent-tools/): Capability
- [Identity from the caller, credentials on the server](https://coreyjames.ai/ideas/identity-from-the-caller/): Idea
- [The hardening fix that locked everyone out](https://coreyjames.ai/stories/the-hardening-fix-that-locked-everyone-out/): Engineering story

## Citation

Corey James. "The Security Officer." coreyjames.ai, 2026. https://coreyjames.ai/agents/roles/security-officer/

```bibtex
@misc{coreyjames-agent-role-security-officer,
  author = {Corey James},
  title = {The Security Officer},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/roles/security-officer/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/security-officer}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
