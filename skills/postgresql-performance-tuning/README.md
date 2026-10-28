# PostgreSQL performance tuning

Pages on coreyjames.ai that demonstrate this skill, decided at build time against every page (highest first).

Canonical: https://coreyjames.ai/llms.txt  
Author: Corey James · Published: 2026-10-28 · Kind: skill index  

| Page | Result | Kind |
| --- | --- | --- |
| [Database performance diagnosis](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/database-performance-diagnosis) · [page](https://coreyjames.ai/technologies/database-performance-diagnosis/) | I diagnose database performance from the database's own statistics, one change at a time. | technology |
| [PostgreSQL bulk-update engineering](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/postgresql-bulk-update-engineering) · [page](https://coreyjames.ai/technologies/postgresql-bulk-update-engineering/) | Statement shape, batch width and index cost, each judged by what the database actually does with a write. | technology |
| [196 deadlocks to zero](https://github.com/coreyjames-ai/fafo-core/tree/main/stories/196-deadlocks-to-zero) · [page](https://coreyjames.ai/stories/196-deadlocks-to-zero/) | Measuring a write path from the database itself, and finding that one index was the whole problem | story |
| [Twenty thousand rows a second](https://github.com/coreyjames-ai/postgresql-fabric/tree/main/stories/twenty-thousand-rows-a-second) · [page](https://coreyjames.ai/stories/twenty-thousand-rows-a-second/) | A batch update that took twenty-five seconds became a third of a second: one SQL rewrite that makes parameter count independent of row count, and nearly 400 GB of indexes that nobody had ever read | story |
| [PostgreSQL Fabric](https://github.com/coreyjames-ai/postgresql-fabric) · [page](https://coreyjames.ai/systems/postgresql-fabric/) | One governed write path for a GPU-scale estate: batches sized from the database's own limits, workers that follow the queue, admission that reads the database's pressure, and the heavy work run inside the database next to its indexes | system |
| [A write path that sizes itself](https://github.com/coreyjames-ai/postgresql-fabric/tree/main/stories/a-write-path-that-sizes-itself) · [page](https://coreyjames.ai/stories/a-write-path-that-sizes-itself/) | Batches sized from the payload's own width under PostgreSQL's parameter limit, writer workers that follow queue demand, and the batch-size knobs deliberately taken away from operators | story |
| [SQL](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/sql) · [page](https://coreyjames.ai/technologies/sql/) | SQL is how I query the stores everything else projects from: work graphs, tuple statistics, retrieval tables, cost ledgers. | technology |
| [Performance engineering and benchmarking](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/performance-engineering-and-benchmarking) · [page](https://coreyjames.ai/technologies/performance-engineering-and-benchmarking/) | Fixed model, one variable at a time, negatives beside positives, and an intake screen that rejects gains tuned to the test fixture. | technology |
| [Write-behind persistence](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/write-behind-persistence) · [page](https://coreyjames.ai/technologies/write-behind-persistence/) | Writes in my substrate go through a write-behind queue and a batching writer, so producers never block on the database. | technology |
| [Rebuild only what moved](https://github.com/coreyjames-ai/inference-fabric/tree/main/stories/rebuild-only-what-moved) · [page](https://coreyjames.ai/stories/rebuild-only-what-moved/) | Column-scoped change capture, a rule that chooses a full or a delta rebuild from the size of the change and never from its age, and a segment merge whose output is byte-identical to a full rebuild | story |
| [Lease-based work claiming](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/lease-based-work-claiming) · [page](https://coreyjames.ai/technologies/lease-based-work-claiming/) | Parallel workers claim work by lease, designed against the dead-tuple behaviour of PostgreSQL's concurrency model, so two workers never process the same item and nothing is lost on a crash. | technology |
| [FAISS](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/faiss) · [page](https://coreyjames.ai/technologies/faiss/) | FAISS is a reference and a bake-off participant in my vector work; my own GPU store builds deterministic indexes and reports their health. | technology |

## Citation

Corey James. "PostgreSQL performance tuning: evidence on coreyjames.ai." 2026. https://coreyjames.ai/llms.txt
