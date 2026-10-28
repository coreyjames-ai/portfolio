# LLM quantization (FP8, INT8, 4-bit)

Pages on coreyjames.ai that demonstrate this skill, decided at build time against every page (highest first).

Canonical: https://coreyjames.ai/llms.txt  
Author: Corey James · Published: 2026-10-28 · Kind: skill index  

| Page | Result | Kind |
| --- | --- | --- |
| [Model quantization](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/model-quantization) · [page](https://coreyjames.ai/technologies/model-quantization/) | A published 4-bit-weight quantization that fits a 27B model on one 32 GB card for 36 percent more throughput at 3 percent perplexity cost, an INT8 compressed history tier for ActiveKV, and FP8 serving on NVIDIA. | technology |
| [Model families and types](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/model-families-and-types) · [page](https://coreyjames.ai/technologies/model-families-and-types/) | I pick a model for the job and the hardware it has to run on, then I change it until it fits. | technology |
| [Hugging Face Hub](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/hugging-face-hub) · [page](https://coreyjames.ai/technologies/hugging-face-hub/) | I published a 4-bit quantization of a 27-billion-parameter model with its card, provenance and measured trade-off. | technology |
| [Bigger models and longer context on fixed GPU memory](https://github.com/coreyjames-ai/portfolio/tree/main/research/capabilities/longer-context-on-the-gpus-you-own) · [page](https://coreyjames.ai/capabilities/longer-context-on-the-gpus-you-own/) | When GPU memory, not the workload, is the limit | capability |
| [A 27B model on one 32 GB Intel card](https://github.com/coreyjames-ai/capabilities-model/tree/main/stories/a-27b-model-on-one-32gb-intel-card) · [page](https://coreyjames.ai/stories/a-27b-model-on-one-32gb-intel-card/) | A measured, attributed and published 4-bit quantization of a 27-billion-parameter hybrid recurrent-attention open-weight model for an Intel Arc Pro GPU | story |
| [Reading a file format by correlation](https://github.com/coreyjames-ai/capabilities-model/tree/main/stories/reading-a-file-format-by-correlation) · [page](https://coreyjames.ai/stories/reading-a-file-format-by-correlation/) | The four-bit weight format's layout was established by correlating candidate decodings against the known weights before a kernel was written, 0.9955 against 0.0018, and four-bit was positioned as a footprint win rather than a speed win | story |
| [vLLM](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/vllm) · [page](https://coreyjames.ai/technologies/vllm/) | vLLM is the engine ActiveKV lives inside, patched at the scheduler, worker and attention backend, and the server under my local open-source models. | technology |
| [Intel Arc GPUs](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/intel-arc-gpus) · [page](https://coreyjames.ai/technologies/intel-arc-gpus/) | An Intel Arc Pro GPU is ActiveKV's home: a 27B model serving 128,000-token histories on one 32 GB card, kernel patches on a new architecture, and a published quantization built for it. | technology |
| [GPU inference engine engineering](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/gpu-inference-engine-engineering) · [page](https://coreyjames.ai/technologies/gpu-inference-engine-engineering/) | I built a batched continuous-decode engine with paged key-value memory, admission control, canary-gated binding and typed refusals, and I tried the vendor's industrial stack first and closed it on measurements. | technology |
| [oneDNN](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/onednn) · [page](https://coreyjames.ai/technologies/onednn/) | Patches to Intel's math library for a GPU architecture the ecosystem had not caught up with, each one held to bit-identical output. | technology |
| [SYCL](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/sycl) · [page](https://coreyjames.ai/technologies/sycl/) | ActiveKV's attention operators and its kernel patches on Intel Xe2 are SYCL, each gated on bit-identical outputs. | technology |
| [Engines for the card you have](https://github.com/coreyjames-ai/inference-fabric/tree/main/stories/engines-for-the-card-you-have) · [page](https://coreyjames.ai/stories/engines-for-the-card-you-have/) | One calibrated FP8 checkpoint, a dozen inference engines sized to two consumer Blackwell GPUs, and the benchmarks that decided what the tiers would be | story |
| [Half the bytes, exactly merged](https://github.com/coreyjames-ai/activekv/tree/main/stories/half-the-bytes-exactly-merged) · [page](https://coreyjames.ai/stories/half-the-bytes-exactly-merged/) | The INT8 history format and the SYCL attention kernels that halve ActiveKV's bus traffic, and the log-sum-exp merge that keeps the result exact | story |

## Citation

Corey James. "LLM quantization (FP8, INT8, 4-bit): evidence on coreyjames.ai." 2026. https://coreyjames.ai/llms.txt
