# The Code Guide

**For anyone with a question about the code.**

Canonical: https://coreyjames.ai/agents/roles/code-guide/  
Author: Corey James · Published: 2026-11-11 · Kind: agent role  

## The story

A product manager asks whether the product already does something. The agent searches the code by meaning, follows the calls from end to end and answers in plain language with the file and line. Every path it describes exists in the code.

## Function

[Knowledge and memory](https://coreyjames.ai/agents/functions/knowledge-and-memory/): What the team learned, kept searchable and handed to every new worker.

## The crew

The specialists behind this role, grouped by the kind of work they do.

### Speaks to people

- [Codebase Onboarding Guide](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/codebase-onboarding-guide) · [page](https://coreyjames.ai/agents/specialists/codebase-onboarding-guide/): Answers a newcomer's questions about how the code works with the exact files and lines involved, plus the reference documents and past decisions behind them.

### Keeps knowledge

- [Codebase Answer Desk](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/codebase-answer-desk) · [page](https://coreyjames.ai/agents/specialists/codebase-answer-desk/): Answers plain-language questions about the team's own code, such as "where do we handle refunds" or "what calls this function", and returns the exact files and lines.
- [Code Flow Explainer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/code-flow-explainer) · [page](https://coreyjames.ai/agents/specialists/code-flow-explainer/): Takes a starting point (a file and line, a function name or a plain question), traces how the work flows through the code, and explains it in plain language.
- [Code Impact Analyst](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/code-impact-analyst) · [page](https://coreyjames.ai/agents/specialists/code-impact-analyst/): For every function or type a change touches, it lists what calls it and what it calls up to three steps out.
- [Reference Researcher](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/reference-researcher) · [page](https://coreyjames.ai/agents/specialists/reference-researcher/): Before anyone writes code, finds how the specification, the vendor manual, a library's source or a documentation website handles the problem, and returns cited sections with page numbers or file paths.
- [Grounding Coach](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/grounding-coach) · [page](https://coreyjames.ai/agents/specialists/grounding-coach/): Checks whether the task troubleshoots or spans several files and, if so, asks for a file and line reference from code search before work starts.

### Runs infrastructure

- [Commit-Triggered Re-Indexer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/commit-triggered-re-indexer) · [page](https://coreyjames.ai/agents/specialists/commit-triggered-re-indexer/): Starts a re-index of the affected codebase as soon as new code lands and reports progress to the team lead's inbox.

### Audits and guards

- [Existing-Capability Checker](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/existing-capability-checker) · [page](https://coreyjames.ai/agents/specialists/existing-capability-checker/): Searches the codebase for something people believe is missing and reports whether any candidate code exists, then checks whether a past decision already settled the question.

## The engineering behind this role

- [Memory and code intelligence for agents](https://coreyjames.ai/capabilities/memory-and-code-intelligence-for-agents/): Capability
- [Compute first, narrate second](https://coreyjames.ai/ideas/compute-first-narrate-second/): Idea
- [A code explainer that is not allowed to invent](https://coreyjames.ai/stories/a-code-explainer-that-is-not-allowed-to-invent/): Engineering story

## Citation

Corey James. "The Code Guide." coreyjames.ai, 2026. https://coreyjames.ai/agents/roles/code-guide/

```bibtex
@misc{coreyjames-agent-role-code-guide,
  author = {Corey James},
  title = {The Code Guide},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/roles/code-guide/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/code-guide}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
