# append-only log design

Pages on coreyjames.ai that demonstrate this skill, decided at build time against every page (highest first).

Canonical: https://coreyjames.ai/llms.txt  
Author: Corey James · Published: 2026-10-28 · Kind: skill index  

| Page | Result | Kind |
| --- | --- | --- |
| [Append-only log and journal design](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/append-only-log-and-journal-design) · [page](https://coreyjames.ai/technologies/append-only-log-and-journal-design/) | The Inference Fabric's broker is an append-only, memory-mapped log on NVMe whose unit is the token. | technology |
| [Append-only, with tombstones and lineage](https://github.com/coreyjames-ai/portfolio/tree/main/research/ideas/append-only-with-lineage) · [page](https://coreyjames.ai/ideas/append-only-with-lineage/) | Durable logs are only ever appended, deletion is a mark, and every derived artefact can prove where it came from | idea |
| [Storage that refuses to become a coordinator](https://github.com/coreyjames-ai/inference-fabric/tree/main/stories/storage-that-refuses-to-become-a-coordinator) · [page](https://coreyjames.ai/stories/storage-that-refuses-to-become-a-coordinator/) | A tensor store that appends, returns a stable address and knows nothing about its consumers; the coordinator tables it once had were removed and the boundary is enforced by checks in the build | story |
| [Done means delivered](https://github.com/coreyjames-ai/inference-fabric/tree/main/stories/done-means-delivered) · [page](https://coreyjames.ai/stories/done-means-delivered/) | A result counts as delivered only after it has been written to the receiver's socket, and polling a job costs what is ready rather than what is pending | story |
| [Inference Fabric](https://github.com/coreyjames-ai/inference-fabric) · [page](https://coreyjames.ai/systems/inference-fabric/) | A throughput-first GPU inference pipeline on consumer NVIDIA hardware: broker, saturated runtime, completion, vector store | system |
| [NVMe (cold-tier storage)](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/nvme-cold-tier-storage) · [page](https://coreyjames.ai/technologies/nvme-cold-tier-storage/) | The broker's cold tier is NVMe: billions of queued tokens survive a restart in shape-pure order. | technology |
| [Git](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/git) · [page](https://coreyjames.ai/technologies/git/) | My governance platform reads git as evidence: witness, task and decision commits, authorship trailers, and the rule that every commit is pushed and nothing is rewritten. | technology |
| [MessagePack](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/messagepack) · [page](https://coreyjames.ai/technologies/messagepack/) | Compact binary serialisation on the agent runtime's message bus and the broker's internal entries. | technology |
| [Meta Graph API](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/meta-graph-api) · [page](https://coreyjames.ai/technologies/meta-graph-api/) | An in-house integration with Meta's Graph API, with usage telemetry, a ledger of everything the app created, and signature-checked webhooks. | technology |
| [X API](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/x-api) · [page](https://coreyjames.ai/technologies/x-api/) | An in-house X integration where one service owns the rate limit, the monthly budget and the send log, and never re-sends an action whose outcome is unknown. | technology |

## Citation

Corey James. "append-only log design: evidence on coreyjames.ai." 2026. https://coreyjames.ai/llms.txt
