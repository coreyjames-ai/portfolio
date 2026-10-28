# database admission control

Pages on coreyjames.ai that demonstrate this skill, decided at build time against every page (highest first).

Canonical: https://coreyjames.ai/llms.txt  
Author: Corey James · Published: 2026-10-28 · Kind: skill index  

| Page | Result | Kind |
| --- | --- | --- |
| [Pricing writes by what they cost the database](https://github.com/coreyjames-ai/postgresql-fabric/tree/main/stories/pricing-writes-by-what-they-cost) · [page](https://coreyjames.ai/stories/pricing-writes-by-what-they-cost/) | An admission controller that reads the database's own pressure, write-ahead-log rate, active writers and lock waits, and admits work only as fast as the database can take it | story |
| [Admission control and rate limiting](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/admission-control-and-rate-limiting) · [page](https://coreyjames.ai/technologies/admission-control-and-rate-limiting/) | Every surface I expose has a stated limit and a typed refusal. | technology |
| [PostgreSQL Fabric](https://github.com/coreyjames-ai/postgresql-fabric) · [page](https://coreyjames.ai/systems/postgresql-fabric/) | One governed write path for a GPU-scale estate: batches sized from the database's own limits, workers that follow the queue, admission that reads the database's pressure, and the heavy work run inside the database next to its indexes | system |
| [Policy-as-code enforcement](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/policy-as-code-enforcement) · [page](https://coreyjames.ai/technologies/policy-as-code-enforcement/) | Policy in my governance platform is enforced by hooks, not remembered by prompts: a lead cannot edit an artifact, work cannot dispatch before its evidence exists, a hook may never report an operation that did not happen. | technology |
| [Storage that refuses to become a coordinator](https://github.com/coreyjames-ai/inference-fabric/tree/main/stories/storage-that-refuses-to-become-a-coordinator) · [page](https://coreyjames.ai/stories/storage-that-refuses-to-become-a-coordinator/) | A tensor store that appends, returns a stable address and knows nothing about its consumers; the coordinator tables it once had were removed and the boundary is enforced by checks in the build | story |

## Citation

Corey James. "database admission control: evidence on coreyjames.ai." 2026. https://coreyjames.ai/llms.txt
