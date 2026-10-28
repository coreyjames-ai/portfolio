# GPU profiling (Nsight)

Pages on coreyjames.ai that demonstrate this skill, decided at build time against every page (highest first).

Canonical: https://coreyjames.ai/llms.txt  
Author: Corey James · Published: 2026-10-28 · Kind: skill index  

| Page | Result | Kind |
| --- | --- | --- |
| [NVIDIA Nsight Systems](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/nvidia-nsight-systems) · [page](https://coreyjames.ai/technologies/nvidia-nsight-systems/) | Nsight traces are where I found what the engine was actually doing, and where I learned to check that the trace was not itself the cause. | technology |
| [The thirteen percent that was never missing](https://github.com/coreyjames-ai/inference-fabric/tree/main/stories/the-thirteen-percent-that-was-never-missing) · [page](https://coreyjames.ai/stories/the-thirteen-percent-that-was-never-missing/) | A profile said thirteen percent of the GPU was idle; it was the share of time in non-matrix kernels. Reading what each metric measured before optimising found utilisation at 98.7 percent | story |
| [Inference Fabric](https://github.com/coreyjames-ai/inference-fabric) · [page](https://coreyjames.ai/systems/inference-fabric/) | A throughput-first GPU inference pipeline on consumer NVIDIA hardware: broker, saturated runtime, completion, vector store | system |
| [Machinery I built and then did not need](https://github.com/coreyjames-ai/inference-fabric/tree/main/stories/machinery-i-built-and-then-did-not-need) · [page](https://coreyjames.ai/stories/machinery-i-built-and-then-did-not-need/) | Fixed-size epochs and dense slots were built so decode steps could be captured as CUDA graphs; profiling showed the vendor's executor already does it. What I kept, what I stopped relying on, and the rule I took from it | story |

## Citation

Corey James. "GPU profiling (Nsight): evidence on coreyjames.ai." 2026. https://coreyjames.ai/llms.txt
