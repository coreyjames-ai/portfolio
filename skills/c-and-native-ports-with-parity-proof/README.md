# C++ and native ports with parity proof

Pages on coreyjames.ai that demonstrate this skill, decided at build time against every page (highest first).

Canonical: https://coreyjames.ai/llms.txt  
Author: Corey James · Published: 2026-10-28 · Kind: skill index  

| Page | Result | Kind |
| --- | --- | --- |
| [Large-scale refactoring with parity proof](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/large-scale-refactoring-with-parity-proof) · [page](https://coreyjames.ai/technologies/large-scale-refactoring-with-parity-proof/) | Rewrite a system, prove it is the same system. My governance platform's own refactors carry parity proofs, and the largest example is a GPU runtime ported to C++ without changing a token. | technology |
| [pybind11](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/pybind11) · [page](https://coreyjames.ai/technologies/pybind11/) | pybind11 binds ActiveKV's C++ engine into vLLM and PyTorch; a line-by-line audit proves every remaining Python line is a framework contract. | technology |
| [C++](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/c-plus-plus) · [page](https://coreyjames.ai/technologies/c-plus-plus/) | ActiveKV's runtime is C++ throughout, ported from Python under bitwise-parity gates, and the Inference Fabric's TensorRT boundary is C++. | technology |
| [Directing AI coding agents at program scale](https://github.com/coreyjames-ai/agentos/tree/main/stories/directing-ai-coding-agents-at-program-scale) · [page](https://coreyjames.ai/stories/directing-ai-coding-agents-at-program-scale/) | How I run engineering programs with teams of frontier and open-source models, and why evidence, not the agents, decides | story |
| [Governed AI-assisted software engineering](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/governed-ai-assisted-software-engineering) · [page](https://coreyjames.ai/technologies/governed-ai-assisted-software-engineering/) | Written definitions of done, builders and reviewers from different model families, intake and promotion procedures, and evidence that decides. | technology |
| [Bigger models and longer context on fixed GPU memory](https://github.com/coreyjames-ai/portfolio/tree/main/research/capabilities/longer-context-on-the-gpus-you-own) · [page](https://coreyjames.ai/capabilities/longer-context-on-the-gpus-you-own/) | When GPU memory, not the workload, is the limit | capability |
| [ActiveKV](https://github.com/coreyjames-ai/activekv) · [page](https://coreyjames.ai/systems/activekv/) | An inference-memory layer for vLLM: the conversation's history in host RAM, the GPU as a bounded working set | system |
| [Rewriting an engine extension without changing a token](https://github.com/coreyjames-ai/activekv/tree/main/stories/rewriting-an-engine-extension-without-changing-a-token) · [page](https://coreyjames.ai/stories/rewriting-an-engine-extension-without-changing-a-token/) | Porting a GPU serving layer from Python to native C++ with bit-identical output, and proving every remaining line of Python was required | story |
| [Governed autonomous engineering](https://github.com/coreyjames-ai/portfolio/tree/main/research/capabilities/governed-autonomous-engineering) · [page](https://coreyjames.ai/capabilities/governed-autonomous-engineering/) | Programs of AI coding agents that finish, prove it, and can be trusted | capability |
| [vLLM](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/vllm) · [page](https://coreyjames.ai/technologies/vllm/) | vLLM is the engine ActiveKV lives inside, patched at the scheduler, worker and attention backend, and the server under my local open-source models. | technology |
| [PyTorch](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/pytorch) · [page](https://coreyjames.ai/technologies/pytorch/) | ActiveKV extends PyTorch's XPU backend and ATen from native code; the capabilities model is a PyTorch fine-tune. | technology |
| [Proving a rewrite is the same system](https://github.com/coreyjames-ai/activekv/tree/main/stories/proving-a-rewrite-is-the-same-system) · [page](https://coreyjames.ai/stories/proving-a-rewrite-is-the-same-system/) | Parity discipline for a GPU runtime, and the day I voided over a thousand passing trials | story |
| [Determinism and numerical reproducibility](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/determinism-and-numerical-reproducibility) · [page](https://coreyjames.ai/technologies/determinism-and-numerical-reproducibility/) | Bit-identical or nothing, wherever the reference is bitwise with itself. | technology |
| [CUTLASS](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/cutlass) · [page](https://coreyjames.ai/technologies/cutlass/) | CUTLASS-for-SYCL is part of the kernel stack I patched on Intel's Xe2 architecture for ActiveKV's attention. | technology |
| [Context beyond VRAM](https://github.com/coreyjames-ai/activekv/tree/main/stories/context-beyond-vram) · [page](https://coreyjames.ai/stories/context-beyond-vram/) | Making a 27-billion-parameter model hold more conversation than its GPU can, exactly, on one card | story |
| [oneDNN](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/onednn) · [page](https://coreyjames.ai/technologies/onednn/) | Patches to Intel's math library for a GPU architecture the ecosystem had not caught up with, each one held to bit-identical output. | technology |
| [Intel oneAPI](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/intel-oneapi) · [page](https://coreyjames.ai/technologies/intel-oneapi/) | Intel's oneAPI stack is what ActiveKV's native engine and its kernel patches are built against, inside the vendor's own toolchain for ABI match. | technology |

## Citation

Corey James. "C++ and native ports with parity proof: evidence on coreyjames.ai." 2026. https://coreyjames.ai/llms.txt
