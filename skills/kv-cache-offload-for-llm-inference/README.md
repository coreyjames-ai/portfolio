# KV-cache offload for LLM inference

Pages on coreyjames.ai that demonstrate this skill, decided at build time against every page (highest first).

Canonical: https://coreyjames.ai/llms.txt  
Author: Corey James · Published: 2026-10-28 · Kind: skill index  

| Page | Result | Kind |
| --- | --- | --- |
| [KV-cache engineering](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/kv-cache-engineering) · [page](https://coreyjames.ai/technologies/kv-cache-engineering/) | The key-value cache is the largest thing on the card after the weights. I moved it to the host in ActiveKV, kept it hot in the Inference Fabric's broker, and in both cases measured the bus. | technology |
| [Context beyond VRAM](https://github.com/coreyjames-ai/activekv/tree/main/stories/context-beyond-vram) · [page](https://coreyjames.ai/stories/context-beyond-vram/) | Making a 27-billion-parameter model hold more conversation than its GPU can, exactly, on one card | story |
| [vLLM](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/vllm) · [page](https://coreyjames.ai/technologies/vllm/) | vLLM is the engine ActiveKV lives inside, patched at the scheduler, worker and attention backend, and the server under my local open-source models. | technology |
| [The copy of record lives off the accelerator](https://github.com/coreyjames-ai/portfolio/tree/main/research/ideas/the-copy-of-record-lives-off-the-accelerator) · [page](https://coreyjames.ai/ideas/the-copy-of-record-lives-off-the-accelerator/) | Host memory or the database holds the truth; the GPU or the model holds a bounded working set | idea |
| [GPU memory management](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/gpu-memory-management) · [page](https://coreyjames.ai/technologies/gpu-memory-management/) | ActiveKV inverts who owns memory: history in pinned host RAM, the GPU a budgeted working set. | technology |
| [Half the bytes, exactly merged](https://github.com/coreyjames-ai/activekv/tree/main/stories/half-the-bytes-exactly-merged) · [page](https://coreyjames.ai/stories/half-the-bytes-exactly-merged/) | The INT8 history format and the SYCL attention kernels that halve ActiveKV's bus traffic, and the log-sum-exp merge that keeps the result exact | story |
| [Bigger models and longer context on fixed GPU memory](https://github.com/coreyjames-ai/portfolio/tree/main/research/capabilities/longer-context-on-the-gpus-you-own) · [page](https://coreyjames.ai/capabilities/longer-context-on-the-gpus-you-own/) | When GPU memory, not the workload, is the limit | capability |
| [ActiveKV](https://github.com/coreyjames-ai/activekv) · [page](https://coreyjames.ai/systems/activekv/) | An inference-memory layer for vLLM: the conversation's history in host RAM, the GPU as a bounded working set | system |
| [Judge a representation by the bytes it stops moving](https://github.com/coreyjames-ai/activekv/tree/main/stories/judge-a-representation-by-the-bytes-it-stops-moving) · [page](https://coreyjames.ai/stories/judge-a-representation-by-the-bytes-it-stops-moving/) | Rewriting an acceptance gate that kept rejecting good compression, and what it bought at 128K tokens | story |
| [NVIDIA Nsight Systems](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/nvidia-nsight-systems) · [page](https://coreyjames.ai/technologies/nvidia-nsight-systems/) | Nsight traces are where I found what the engine was actually doing, and where I learned to check that the trace was not itself the cause. | technology |
| [Engines for the card you have](https://github.com/coreyjames-ai/inference-fabric/tree/main/stories/engines-for-the-card-you-have) · [page](https://coreyjames.ai/stories/engines-for-the-card-you-have/) | One calibrated FP8 checkpoint, a dozen inference engines sized to two consumer Blackwell GPUs, and the benchmarks that decided what the tiers would be | story |
| [Model quantization](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/model-quantization) · [page](https://coreyjames.ai/technologies/model-quantization/) | A published 4-bit-weight quantization that fits a 27B model on one 32 GB card for 36 percent more throughput at 3 percent perplexity cost, an INT8 compressed history tier for ActiveKV, and FP8 serving on NVIDIA. | technology |

## Citation

Corey James. "KV-cache offload for LLM inference: evidence on coreyjames.ai." 2026. https://coreyjames.ai/llms.txt
