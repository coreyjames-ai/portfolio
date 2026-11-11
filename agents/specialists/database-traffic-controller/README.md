# Database Traffic Controller

**Keeps heavy bulk writes from flattening the database: it prices each write by its expected load, lets cheap work through, holds heavy work until there is room, and tunes the write workers.**

Canonical: https://coreyjames.ai/agents/specialists/database-traffic-controller/  
Author: Corey James · Published: 2026-11-11 · Kind: agent specialist  

## What it does

Keeps heavy bulk writes from flattening the database: it prices each write by its expected load, lets cheap work through, holds heavy work until there is room, and tunes the write workers. You can run it in watch-only mode first and switch to enforcing when you trust the numbers.

For a database administrator.

Kind: [Runs infrastructure](https://coreyjames.ai/agents/specialists/?kind=runs-infrastructure). Keeps machines, queues and data moving.

Group: Machines, data and operations.

## Roles it serves

- [The Database Guard](https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/database-guard) · [page](https://coreyjames.ai/agents/roles/database-guard/): For a team whose database takes writes from many directions.
- [The Pipeline Foreman](https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/pipeline-foreman) · [page](https://coreyjames.ai/agents/roles/pipeline-foreman/): For a data team lead who needs a new processing job by Thursday.

## Citation

Corey James. "Database Traffic Controller." coreyjames.ai, 2026. https://coreyjames.ai/agents/specialists/database-traffic-controller/

```bibtex
@misc{coreyjames-agent-specialist-database-traffic-controller,
  author = {Corey James},
  title = {Database Traffic Controller},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/specialists/database-traffic-controller/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/database-traffic-controller}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
