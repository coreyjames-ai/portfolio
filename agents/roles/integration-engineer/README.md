# The Integration Engineer

**For an IT lead who keeps being asked to connect another service.**

Canonical: https://coreyjames.ai/agents/roles/integration-engineer/  
Author: Corey James · Published: 2026-11-11 · Kind: agent role  

## The story

The agent reads the other service's documentation, generates the tools to use it and tries them with harmless read-only calls. It stores the credentials, runs the standard checks and only then lets the connection go live. From then on it receives that service's notifications, checks that each one is genuine, drops duplicates and routes it to the team that should act. When a fault sits on the supplier's side, it raises the case and follows it.

## Function

[Engineering](https://coreyjames.ai/agents/functions/engineering/): Planning, building, reviewing and releasing software, with the reasoning kept.

## The crew

The specialists behind this role, grouped by the kind of work they do.

### Does the work

- [API Upgrade Planner](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/api-upgrade-planner) · [page](https://coreyjames.ai/agents/specialists/api-upgrade-planner/): Reads the documentation for the new version, finds every place the old interface is used, sizes the change, and drafts the task plan for the upgrade.

### Speaks to people

- [Supplier Support Liaison](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/supplier-support-liaison) · [page](https://coreyjames.ai/agents/specialists/supplier-support-liaison/): Writes up the unexplained problem with its evidence, raises it with the supplier's support, follows the case and reports the answer.

### Keeps knowledge

- [Third-Party Integration Researcher](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/third-party-integration-researcher) · [page](https://coreyjames.ai/agents/specialists/third-party-integration-researcher/): Reads the outside platform's documentation and development-kit source, compares it with the current code and writes down the facts the developers will build on.
- [Documentation Site Harvester](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/documentation-site-harvester) · [page](https://coreyjames.ai/agents/specialists/documentation-site-harvester/): Crawls a documentation website inside set domain and path boundaries, cleans each page into readable text, splits it into sections, writes a summary, keywords and a quality score for each section, and makes the whole site searchable.

### Runs infrastructure

- [Integration Wiring Engineer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/integration-wiring-engineer) · [page](https://coreyjames.ai/agents/specialists/integration-wiring-engineer/): Registers each incoming feed, wires the website, email route and provider inbox to the right project, checks that events arrive and reach the lead, and rotates credentials on schedule.
- [Systems Connection Specialist](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/systems-connection-specialist) · [page](https://coreyjames.ai/agents/specialists/systems-connection-specialist/): It sets up the connection, issues and rotates its access key, configures the sending system, confirms events arrive, and switches the connection off when it is no longer needed.
- [Business Event Switchboard](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/business-event-switchboard) · [page](https://coreyjames.ai/agents/specialists/business-event-switchboard/): It connects payments, email, social activity, inbound mail and the website so every customer signal lands in one team inbox, where it can become a task.
- [New App Integration Engineer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/new-app-integration-engineer) · [page](https://coreyjames.ai/agents/specialists/new-app-integration-engineer/): This agent reads a new app's API documentation, generates the tools to use it, tries it with safe read-only test calls, writes the connection settings, stores the credentials and runs the standard checks before the app goes live.
- [Tool Onboarding Specialist](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/tool-onboarding-specialist) · [page](https://coreyjames.ai/agents/specialists/tool-onboarding-specialist/): Qualifies each new tool with normal and hostile test cases, rebuilds the tool index the agents search, and confirms agents can find the new tool.
- [Event Feed Manager](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/event-feed-manager) · [page](https://coreyjames.ai/agents/specialists/event-feed-manager/): It decides which email, SMS, inbound mail, social and payment events the business wants told about, points them at the right receiver, and checks that they keep arriving.

### Audits and guards

- [Event Delivery Watchdog](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/event-delivery-watchdog) · [page](https://coreyjames.ai/agents/specialists/event-delivery-watchdog/): It checks that social, email and payment notifications are still arriving and that usage allowances are not running out, and it alerts the team when something drops.
- [Integration Health Checker](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/integration-health-checker) · [page](https://coreyjames.ai/agents/specialists/integration-health-checker/): This agent runs the standard checks across the integration platform so a broken connection is found before a user finds it.

## The engineering behind this role

- [Business systems as safe agent tools](https://coreyjames.ai/capabilities/business-systems-as-safe-agent-tools/): Capability
- [Tools are the platform](https://coreyjames.ai/ideas/tools-are-the-platform/): Idea
- [Agents that react to the world](https://coreyjames.ai/ideas/agents-that-react-to-the-world/): Idea
- [Agents with real tools and no keys](https://coreyjames.ai/stories/agents-with-real-tools-and-no-keys/): Engineering story

## Citation

Corey James. "The Integration Engineer." coreyjames.ai, 2026. https://coreyjames.ai/agents/roles/integration-engineer/

```bibtex
@misc{coreyjames-agent-role-integration-engineer,
  author = {Corey James},
  title = {The Integration Engineer},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/roles/integration-engineer/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/integration-engineer}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
