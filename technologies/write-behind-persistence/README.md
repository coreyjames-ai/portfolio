# Write-behind persistence

**Writes in my substrate go through a write-behind queue and a batching writer, so producers never block on the database.**

Canonical: https://coreyjames.ai/technologies/write-behind-persistence/  
Author: Corey James · Published: 2026-10-28 · Kind: technology  
Systems: [PostgreSQL Fabric](https://github.com/coreyjames-ai/postgresql-fabric) · [FAFO Core and Function Forge](https://github.com/coreyjames-ai/fafo-core) · [Inference Fabric](https://github.com/coreyjames-ai/inference-fabric)  
Skills: [PostgreSQL performance tuning](https://github.com/coreyjames-ai/portfolio/tree/main/skills/postgresql-performance-tuning) · [Rust systems engineering](https://github.com/coreyjames-ai/portfolio/tree/main/skills/rust-systems-engineering) · [tool synthesis and governed API integration](https://github.com/coreyjames-ai/portfolio/tree/main/skills/tool-synthesis-and-governed-api-integration)  

![Write-behind persistence](figures/hero.png)

## Result

| Figure | What it measures |
| --- | --- |
| **196 → 0** | deadlocks, before and after one schema change on the shared path |
| **2 s** | the slowest batches before that change |

## What was built

### One governed write path

[FAFO Core and Function Forge](https://coreyjames.ai/systems/fafo-core) runs functions that fan out to many GPU workers on several machines, each producing results in bursts. If every worker wrote to PostgreSQL itself, the database would see as many writers as there are workers, each holding connections and locks while it waits on a GPU. I made a house rule.

![Figure 1](figures/fig-01.png)

Workers hand off results and move on, and the writer, not the workers, sets the database's write load. Schema validation lives on that single path and nowhere else, so a malformed row is rejected in one place for every function. A function that writes to several related tables hands off the set together, so related rows land as a unit.

![Every worker writes for itself](figures/fig-02.png)

### Results for producers that walked away

[Inference Fabric](https://coreyjames.ai/systems/inference-fabric) feeds the same path. Producers there submit inference work and exit, sometimes hours before results exist. I built a completion service that receives results from the GPUs and dispatches them per function into the governed write path, so a producer that walked away still gets its results stored.

![Submit and exit, stored anyway](figures/fig-03.png)

### Judged by rows committed

When a bulk update workload slowed that shared write path to a crawl, with frequent deadlocks, I measured from the database's own statistics, because the queue in front of it counts intake and the database counts committed rows. Comparing runs before and after a single schema change ended the deadlocks. See [196 deadlocks to zero](https://coreyjames.ai/stories/196-deadlocks-to-zero).

![Figure 4](figures/fig-04.png)

> Functions read from PostgreSQL directly, and every write leaves the function as a message that one governed writer applies.

## What was verified

Each line is a claim the canonical page supports, with the figure as the page states it.

- Write-behind persistence: every write from GPU-scale workers leaves as a message one governed writer applies, so the database takes writes at a rate it can sustain.
- PostgreSQL performance tuning: deadlocks on the shared write path went 196 → 0 after one schema change, measured from committed rows rather than queue intake.

## Related

- [196 deadlocks to zero](https://github.com/coreyjames-ai/fafo-core/tree/main/stories/196-deadlocks-to-zero) · https://coreyjames.ai/stories/196-deadlocks-to-zero/
- System: [PostgreSQL Fabric](https://github.com/coreyjames-ai/postgresql-fabric)
- System: [FAFO Core and Function Forge](https://github.com/coreyjames-ai/fafo-core)
- System: [Inference Fabric](https://github.com/coreyjames-ai/inference-fabric)

## Citation

Corey James. "Write-behind persistence." coreyjames.ai, 2026. https://coreyjames.ai/technologies/write-behind-persistence/

```bibtex
@misc{coreyjames-write-behind-persistence,
  author = {Corey James},
  title = {Write-behind persistence},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/technologies/write-behind-persistence/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/technologies/write-behind-persistence}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
