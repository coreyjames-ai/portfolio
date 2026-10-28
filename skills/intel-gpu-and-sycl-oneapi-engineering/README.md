# Intel GPU and SYCL/oneAPI engineering

Pages on coreyjames.ai that demonstrate this skill, decided at build time against every page (highest first).

Canonical: https://coreyjames.ai/llms.txt  
Author: Corey James · Published: 2026-10-28 · Kind: skill index  

| Page | Result | Kind |
| --- | --- | --- |
| [Intel oneAPI](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/intel-oneapi) · [page](https://coreyjames.ai/technologies/intel-oneapi/) | Intel's oneAPI stack is what ActiveKV's native engine and its kernel patches are built against, inside the vendor's own toolchain for ABI match. | technology |
| [oneDNN](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/onednn) · [page](https://coreyjames.ai/technologies/onednn/) | Patches to Intel's math library for a GPU architecture the ecosystem had not caught up with, each one held to bit-identical output. | technology |
| [CUTLASS](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/cutlass) · [page](https://coreyjames.ai/technologies/cutlass/) | CUTLASS-for-SYCL is part of the kernel stack I patched on Intel's Xe2 architecture for ActiveKV's attention. | technology |
| [Bringing a serving stack up on new silicon](https://github.com/coreyjames-ai/activekv/tree/main/stories/bringing-a-serving-stack-up-on-new-silicon) · [page](https://coreyjames.ai/stories/bringing-a-serving-stack-up-on-new-silicon/) | Patching Intel's Xe2 kernel stack where it had gaps, with outputs that stayed identical | story |
| [SYCL](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/sycl) · [page](https://coreyjames.ai/technologies/sycl/) | ActiveKV's attention operators and its kernel patches on Intel Xe2 are SYCL, each gated on bit-identical outputs. | technology |
| [Intel Arc GPUs](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/intel-arc-gpus) · [page](https://coreyjames.ai/technologies/intel-arc-gpus/) | An Intel Arc Pro GPU is ActiveKV's home: a 27B model serving 128,000-token histories on one 32 GB card, kernel patches on a new architecture, and a published quantization built for it. | technology |
| [ActiveKV](https://github.com/coreyjames-ai/activekv) · [page](https://coreyjames.ai/systems/activekv/) | An inference-memory layer for vLLM: the conversation's history in host RAM, the GPU as a bounded working set | system |
| [Context beyond VRAM](https://github.com/coreyjames-ai/activekv/tree/main/stories/context-beyond-vram) · [page](https://coreyjames.ai/stories/context-beyond-vram/) | Making a 27-billion-parameter model hold more conversation than its GPU can, exactly, on one card | story |
| [Bigger models and longer context on fixed GPU memory](https://github.com/coreyjames-ai/portfolio/tree/main/research/capabilities/longer-context-on-the-gpus-you-own) · [page](https://coreyjames.ai/capabilities/longer-context-on-the-gpus-you-own/) | When GPU memory, not the workload, is the limit | capability |
| [The observer that changed the answer](https://github.com/coreyjames-ai/activekv/tree/main/stories/the-observer-that-changed-the-answer) · [page](https://coreyjames.ai/stories/the-observer-that-changed-the-answer/) | Discovering that my own profiler caused the serialisation it reported, and retracting a verdict I had already acted on | story |
| [LD_PRELOAD symbol interposition](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/ld-preload-symbol-interposition) · [page](https://coreyjames.ai/technologies/ld-preload-symbol-interposition/) | Symbol interposition let me intercept runtime calls directly when the vendor's tracing path was itself distorting measurements. | technology |
| [Half the bytes, exactly merged](https://github.com/coreyjames-ai/activekv/tree/main/stories/half-the-bytes-exactly-merged) · [page](https://coreyjames.ai/stories/half-the-bytes-exactly-merged/) | The INT8 history format and the SYCL attention kernels that halve ActiveKV's bus traffic, and the log-sum-exp merge that keeps the result exact | story |
| [Ghost bytes in a zero-copy ring](https://github.com/coreyjames-ai/inference-fabric/tree/main/stories/ghost-bytes-in-a-zero-copy-ring) · [page](https://coreyjames.ai/stories/ghost-bytes-in-a-zero-copy-ring/) | A pinned-memory ring deadlocked with the GPU idle and hundreds of thousands of items in flight, because wrap-around padding was never freed; and a GPU worker that registered twice was starved as dead | story |
| [The 128-lane wall](https://github.com/coreyjames-ai/inference-fabric/tree/main/stories/the-128-lane-wall) · [page](https://coreyjames.ai/stories/the-128-lane-wall/) | Padding waste ran under one percent until every shape used all of its 128 lanes, then climbed past 95 percent on a 22-million-item load test; the fix was structural | story |
| [GPU profiling and tracing](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/gpu-profiling-and-tracing) · [page](https://coreyjames.ai/technologies/gpu-profiling-and-tracing/) | I instrument ActiveKV down to the runtime call level and I measure the instrument: a profiler that serialised the copy engine it was observing got its verdict retracted in the plan. | technology |
| [Millions of queued items that were not there](https://github.com/coreyjames-ai/inference-fabric/tree/main/stories/millions-of-queued-items-that-were-not-there) · [page](https://coreyjames.ai/stories/millions-of-queued-items-that-were-not-there/) | Fixing what 'done' meant in a GPU work broker until the token ledger balanced to zero | story |

## Citation

Corey James. "Intel GPU and SYCL/oneAPI engineering: evidence on coreyjames.ai." 2026. https://coreyjames.ai/llms.txt
