# observability and alerting

Pages on coreyjames.ai that demonstrate this skill, decided at build time against every page (highest first).

Canonical: https://coreyjames.ai/llms.txt  
Author: Corey James · Published: 2026-10-28 · Kind: skill index  

| Page | Result | Kind |
| --- | --- | --- |
| [Site reliability engineering](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/site-reliability-engineering) · [page](https://coreyjames.ai/technologies/site-reliability-engineering/) | A declared systemd fleet, tunnelled ingress, a documented Redis topology and written runbooks keep my estate recoverable. | technology |
| [Observability and alerting](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/observability-and-alerting) · [page](https://coreyjames.ai/technologies/observability-and-alerting/) | SMS alerting is wired to the service fleet, with a metrics stack and dashboards beside it, and a status dashboard that says plainly what each service is doing. | technology |
| [Prometheus](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/prometheus) · [page](https://coreyjames.ai/technologies/prometheus/) | Prometheus carries the numbers that decide whether GPUs earn their keep, follows a fleet that changes under it, and pages one operator's phone. | technology |
| [Grafana](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/grafana) · [page](https://coreyjames.ai/technologies/grafana/) | Dashboards are how I captured the numbers on this site. | technology |
| [Shapes have a lifecycle](https://github.com/coreyjames-ai/inference-fabric/tree/main/stories/shapes-have-a-lifecycle) · [page](https://coreyjames.ai/stories/shapes-have-a-lifecycle/) | Every switch of prompt shape costs a GPU its prefix cache, so the broker stages a shape until it is worth running, warms the next one before the current one drains, and alarms when a shape ran too briefly | story |
| [Millions of queued items that were not there](https://github.com/coreyjames-ai/inference-fabric/tree/main/stories/millions-of-queued-items-that-were-not-there) · [page](https://coreyjames.ai/stories/millions-of-queued-items-that-were-not-there/) | Fixing what 'done' meant in a GPU work broker until the token ledger balanced to zero | story |
| [Rules that never ran](https://github.com/coreyjames-ai/postgresql-fabric/tree/main/stories/rules-that-never-ran) · [page](https://coreyjames.ai/stories/rules-that-never-ran/) | The writer's batch-release rules had been silently unused, workers were grabbing whatever arrived, and 145 of 153 stream consumers were ghosts; how the write path was found out and rebuilt | story |
| [ActiveKV](https://github.com/coreyjames-ai/activekv) · [page](https://coreyjames.ai/systems/activekv/) | An inference-memory layer for vLLM: the conversation's history in host RAM, the GPU as a bounded working set | system |
| [Catalog versioning and drift detection](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/catalog-versioning-and-drift-detection) · [page](https://coreyjames.ai/technologies/catalog-versioning-and-drift-detection/) | Every host in my agent fleet runs the same approved tool catalog, verified by content hash, with drift detection that falls back from notifications to polling under measured thresholds and never flaps. | technology |

## Citation

Corey James. "observability and alerting: evidence on coreyjames.ai." 2026. https://coreyjames.ai/llms.txt
