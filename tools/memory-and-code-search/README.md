# Memory and code search



Canonical: https://coreyjames.ai/tools/memory-and-code-search/  
Author: Corey James · Published: 2026-10-28 · Kind: tool group  
Systems: [FAFOHive](https://github.com/coreyjames-ai/fafohive)  

## What was built

Agents waste most of their effort rediscovering things: where a behaviour lives in the code, why a decision was made, what went wrong last week. I gave every agent in my estate the same memory, served by [FAFOHive](https://coreyjames.ai/systems/fafohive). These eight tools are how an agent asks it questions. Code is indexed by syntax tree, so a search returns whole functions and types with file and line. The code graph answers structural questions without a model. Decisions and fixes are kept as observations, so the reasoning behind a change outlives the session that made it.

## The tools

`list_indexes` lists the code and reference collections that exist and how much each holds. Its names are the scope every search uses.

`search_code` finds the implementation behind a behaviour in an indexed codebase and returns ranked code chunks with file paths and lines. A search can cover the whole codebase, one directory, or a chosen set of files that work together, and it has an exact-symbol mode for named functions.

`search_references` searches external material: documents, library source and crawled documentation. It is where an agent looks for a reference implementation or a specification before writing its own.

`trace_symbol_dependencies` walks the code graph around a function, type or trait to show callers, callees, imports and implementations, with a chosen direction and depth. No model is involved, so it answers fast and it cannot make an edge up.

`explain_code_path` turns a path through the code graph into a readable explanation of how execution or data flows between two points. The narrative is built only from edges the graph contains, which is the subject of [a code explainer that is not allowed to invent](https://coreyjames.ai/stories/a-code-explainer-that-is-not-allowed-to-invent).

`search_observations` searches recorded decisions, discoveries and fixes by meaning, by keyword or by both, with project and date filters.

`create_observation` records a decision, fix or discovery with a title, a narrative of what happened and why, and optional tags and affected files.

`search_agent_history` reads the raw activity log of agent runs with exact filters on job, trace, event, model and time. It reconstructs one particular run, where observation search finds lessons across many.

Eight tools is a small surface on purpose. Every agent connects to it, and the less it has to learn, the more often it uses memory before it guesses.

## What was verified

Each line is a claim the canonical page supports, with the figure as the page states it.

- Memory for AI agents: 8 tools let an agent search code by syntax tree, search reference material, recall past decisions and fixes, and record new observations.
- Code intelligence for AI agents: code-graph tools answer callers, callees and dependency questions without a model, returning file paths and lines.

## Related

- [A code explainer that is not allowed to invent](https://github.com/coreyjames-ai/fafohive/tree/main/stories/a-code-explainer-that-is-not-allowed-to-invent) · https://coreyjames.ai/stories/a-code-explainer-that-is-not-allowed-to-invent/
- System: [FAFOHive](https://github.com/coreyjames-ai/fafohive)

## Citation

Corey James. "Memory and code search." coreyjames.ai, 2026. https://coreyjames.ai/tools/memory-and-code-search/

```bibtex
@misc{coreyjames-memory-and-code-search,
  author = {Corey James},
  title = {Memory and code search},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/tools/memory-and-code-search/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/tools/memory-and-code-search}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
