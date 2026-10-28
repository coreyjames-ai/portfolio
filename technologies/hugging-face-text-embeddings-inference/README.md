# Hugging Face Text Embeddings Inference

**A local text-embedding inference server serves the embedding model to the memory service, replacing an earlier in-process binding.**

Canonical: https://coreyjames.ai/technologies/hugging-face-text-embeddings-inference/  
Author: Corey James · Published: 2026-10-28 · Kind: technology  
Systems: [FAFOHive](https://github.com/coreyjames-ai/fafohive)  
Skills: [inference serving architecture](https://github.com/coreyjames-ai/portfolio/tree/main/skills/inference-serving-architecture) · [GPU inference optimisation](https://github.com/coreyjames-ai/portfolio/tree/main/skills/gpu-inference-optimisation) · [AI-assisted engineering methodology](https://github.com/coreyjames-ai/portfolio/tree/main/skills/ai-assisted-engineering-methodology)  

![Hugging Face Text Embeddings Inference](figures/hero.png)

## Result

| Figure | What it measures |
| --- | --- |
| **1,024** | dimensions per embedding |
| **~19,000** | files in the monorepo's code index |
| **~294,000** | structure-aware chunks embedded from them |

## What was built

### A model behind a service boundary

The memory capability in [FAFOHive](https://coreyjames.ai/systems/fafohive) searches code, reference documents and past decisions, and all of it depends on one multilingual embedding model. The first version ran that model in-process through a Python binding inside the Rust service. That put a Python runtime and a GPU model inside the Rust service, and every other service that needed embeddings would have loaded its own copy.

I moved the model behind a service boundary, so it is loaded once and shared. Hugging Face's Text Embeddings Inference server runs that model on a local GPU, and the memory service calls it over HTTP through a provider abstraction. I kept the service's existing embedding interface fixed while the backend changed underneath it, so no caller had to change.

![Before](figures/fig-01.png)

![Figure 2](figures/fig-02.png)

### One interface, several backends

The provider abstraction keeps a CPU-only path, so the service still works on a machine without a GPU, and it can point at any OpenAI-compatible endpoint.

![Figure 3](figures/fig-03.png)

The same model serves the service's other search tools. The retrieval built on these embeddings is described under [Hybrid retrieval](https://coreyjames.ai/technologies/hybrid-retrieval), and the code-graph side of the service is [A code explainer that is not allowed to invent](https://coreyjames.ai/stories/a-code-explainer-that-is-not-allowed-to-invent).

### Transport and capacity

The client authenticates to the inference server with mutual TLS, and the capacity layer treats the embedding endpoint as a bounded resource.

![The client certificate](figures/fig-04.png)

The inference server is Hugging Face's, used as provided; my work is the client, the migration, the transport security and the capacity behaviour around it.

> I make deliberate calls about where a model should live in a system and how a migration should land without breaking callers.

## What was verified

Each line is a claim the canonical page supports, with the figure as the page states it.

- Embedding inference serving: an in-process embedding model moved behind Hugging Face's inference server on a local GPU, with the embedding interface unchanged for every caller.
- Code search indexing: ~19,000 files embedded into ~294,000 structure-aware chunks at 1,024 dimensions.
- Mutual TLS client security: client certificates held only in memory and wiped on release, never written to disk, with capacity errors told apart from fatal ones.

## Related

- [A code explainer that is not allowed to invent](https://github.com/coreyjames-ai/fafohive/tree/main/stories/a-code-explainer-that-is-not-allowed-to-invent) · https://coreyjames.ai/stories/a-code-explainer-that-is-not-allowed-to-invent/
- [Hybrid retrieval](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/hybrid-retrieval) · https://coreyjames.ai/technologies/hybrid-retrieval/
- System: [FAFOHive](https://github.com/coreyjames-ai/fafohive)

## Citation

Corey James. "Hugging Face Text Embeddings Inference." coreyjames.ai, 2026. https://coreyjames.ai/technologies/hugging-face-text-embeddings-inference/

```bibtex
@misc{coreyjames-hugging-face-text-embeddings-inference,
  author = {Corey James},
  title = {Hugging Face Text Embeddings Inference},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/technologies/hugging-face-text-embeddings-inference/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/technologies/hugging-face-text-embeddings-inference}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
