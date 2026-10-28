# Technologies (177)

**177 technologies, each with the systems and stories where it matters**

Canonical: https://coreyjames.ai/technologies/  
Author: Corey James · Published: 2026-10-28 · Kind: index  

## datastore (6)

- [FAISS](faiss) · FAISS is a reference and a bake-off participant in my vector work; my own GPU store builds deterministic indexes and reports their health.
- [Garnet](garnet) · A Redis-compatible store evaluated for the memory service's hot path.
- [pgvector](pgvector) · Vector search inside PostgreSQL backs the memory service's hybrid retrieval and the capabilities model's data factory.
- [PostgreSQL](postgresql) · PostgreSQL is the source of truth for everything I build: a governance work graph, lease-based claiming designed against its concurrency model, and diagnosis from its own tuple statistics.
- [Redis](redis) · Redis Streams carry my execution substrate's command bus with Lua-atomic job promotion, the agent runtime's messaging, and the write-behind queue. Topology is explicit and documented.
- [SQLite](sqlite) · SQLite gives each of FAFOHive's social and media modules durable, transactional state that one process owns.

## discipline (82)

- [Admission control and rate limiting](admission-control-and-rate-limiting) · Every surface I expose has a stated limit and a typed refusal.
- [Agent tool-execution safety and sandboxing](agent-tool-execution-safety-and-sandboxing) · Every action any agent takes in my runtime passes one frozen pipeline: validation, authorisation, limits, sanitisation, audit, observation.
- [Agent tool qualification testing](agent-tool-qualification-testing) · No tool in my agent runtime ships without golden fixtures and attack fixtures, and the build fails otherwise.
- [Append-only log and journal design](append-only-log-and-journal-design) · The Inference Fabric's broker is an append-only, memory-mapped log on NVMe whose unit is the token.
- [Application security hardening and threat modelling](application-security-hardening-and-threat-modelling) · I review my own public endpoints, fix findings in severity order with explicit probes, and re-run the threat model when a fix breaks the world.
- [Applied cryptography](applied-cryptography) · I apply cryptography where it buys attribution and non-repudiation, and I do not invent primitives.
- [Approximate nearest-neighbour search](approximate-nearest-neighbour-search) · I built exact, inverted-file and lattice nearest-neighbour search as GPU kernels with CPU references and equivalence tests, inside a vector store whose index builds are deterministic and whose search reports its own health.
- [Binary wire protocol design](binary-wire-protocol-design) · I design binary wire protocols when the problem needs them: the Teams audio link with byte-identical C# and Rust implementations, the broker's token-level transport, the vector store's RPC wire.
- [Budget enforcement and cost governance](budget-enforcement-and-cost-governance) · Spend is a first-class control in my substrate: a fail-closed daily budget on GPU provisioning that agents cannot raise from inside the provisioning path, per-second accounting, and cost attributed to the work order that spent it.
- [Business-provider APIs rebuilt as governed agent tools](business-provider-apis-rebuilt-as-governed-agent-tools) · Payments, email/CRM and social-publishing APIs, rebuilt operation by operation as governed agent tools under stable names, with credentials server-side, attribution where it round-trips and every call accounted.
- [Cache synchronisation and leader election](cache-synchronisation-and-leader-election) · The API integration platform keeps its cache coherent across workers and elects a leader for its sync worker.
- [Capacity engineering, backpressure and load testing](capacity-engineering-backpressure-and-load-testing) · I load-test what I build and report the misses: a 2,048-client ladder against a GPU decoder, bounded endpoints and saturating rerank in the memory service, and a pre-registered target I missed and explained.
- [Catalog versioning and drift detection](catalog-versioning-and-drift-detection) · Every host in my agent fleet runs the same approved tool catalog, verified by content hash, with drift detection that falls back from notifications to polling under measured thresholds and never flaps.
- [Cluster-health metrics on the GPU](cluster-health-metrics-on-the-gpu) · Per-cluster metrics, each answering a question a corpus manager asks, computed across thousands of clusters in fused GPU launches and defined by CPU reference code.
- [Code generation and metaprogramming](code-generation-and-metaprogramming) · I generate code where repetition is the risk: a generator that emits a whole function and wires it into the estate transactionally, and YAML tool schemas compiled into dispatch at build time.
- [Code graph and static dependency analysis](code-graph-and-static-dependency-analysis) · The code graph under my memory service is extracted with a parser into partitioned edge tables; dependency traces are bounded database traversals with no model involved, and the explainer may narrate only proven edges.
- [Context engineering and persistent agent memory](context-engineering-and-persistent-agent-memory) · Agents forget between sessions, so I built the memory that remembers for them: every tool call captured, extracted and re-injected into later sessions, and a council shell with durable state in PostgreSQL.
- [Contract-first interface design](contract-first-interface-design) · Every job an agent receives in my governance platform carries a schema that says what must come back. Contracts first, prose only for behaviour.
- [Conversational turn-taking and barge-in](conversational-turn-taking-and-barge-in) · I built a voice engine in which several AI voices share one conversation without talking over each other, and a person speaking stops the agent.
- [Cost attribution for AI work](cost-attribution-for-ai-work) · Every token my agents spend is attributed to the work order that bought it.
- [CPU reference implementations and GPU equivalence testing](cpu-reference-implementations-and-gpu-equivalence-testing) · Every GPU metric has a plain-Rust CPU twin that defines it.
- [Credential brokering and secrets management](credential-brokering-and-secrets-management) · No agent in my estate holds a credential it does not need, and most hold none.
- [Database performance diagnosis](database-performance-diagnosis) · I diagnose database performance from the database's own statistics, one change at a time.
- [Declarative tool and agent definition](declarative-tool-and-agent-definition) · In my agent runtime a tool is a YAML declaration and an agent class is a composition.
- [Determinism and numerical reproducibility](determinism-and-numerical-reproducibility) · Bit-identical or nothing, wherever the reference is bitwise with itself.
- [Distributed job orchestration](distributed-job-orchestration) · One function definition runs as a job or a service, batched by rows or by GPU token budget, anywhere from in-process to rented cloud GPUs, by configuration.
- [Distributed-systems reliability](distributed-systems-reliability) · Nothing waits on anything else, every component restarts independently, and the accounting balances.
- [Evidence-gated acceptance](evidence-gated-acceptance) · A capability counts only when evidence shows it wired and exercised at runtime, and the gates say what is still unproven.
- [Evidence-gated API integration](evidence-gated-api-integration) · My API integration platform treats each third-party API as a declarative unit over a generic core, with evidence for every gate.
- [Evidence-grounded LLM output](evidence-grounded-llm-output) · A model in my systems may narrate evidence it was handed; it may not produce evidence.
- [Federated compute provisioning](federated-compute-provisioning) · One call stands up GPU capacity on a local card, a LAN workstation over mutual TLS, or rented cloud spot capacity, behind a fail-closed daily budget.
- [Gaussian-kernel cluster analysis](gaussian-kernel-cluster-analysis) · A per-cluster length scale from a histogram median, then potential depth, curvature, escape probability, superposition, interference and entanglement as field metrics over an embedding cluster.
- [Governed AI-assisted software engineering](governed-ai-assisted-software-engineering) · Written definitions of done, builders and reviewers from different model families, intake and promotion procedures, and evidence that decides.
- [GPU admission control and co-residency](gpu-admission-control-and-co-residency) · Two models on one GPU, with the second admitting work against measured memory and refusing with a number: a 0.6B router beside a 30B model, through a 2,048-client burst.
- [GPU inference engine engineering](gpu-inference-engine-engineering) · I built a batched continuous-decode engine with paged key-value memory, admission control, canary-gated binding and typed refusals, and I tried the vendor's industrial stack first and closed it on measurements.
- [GPU memory management](gpu-memory-management) · ActiveKV inverts who owns memory: history in pinned host RAM, the GPU a budgeted working set.
- [GPU numerical kernel design](gpu-numerical-kernel-design) · Kernels with fixed-order reductions, one block per output row, no K-split tiling: determinism by construction.
- [GPU profiling and tracing](gpu-profiling-and-tracing) · I instrument ActiveKV down to the runtime call level and I measure the instrument: a profiler that serialised the copy engine it was observing got its verdict retracted in the plan.
- [Grammar-constrained decoding](grammar-constrained-decoding) · A grammar compiled from the tool registry constrains the decoder so that names outside the catalog cannot be produced.
- [Hidden-state extraction](hidden-state-extraction) · The Inference Fabric's runtime has a single-pass hidden-state extraction mode with an empirical, fail-closed tensor-semantics detector.
- [Hybrid retrieval](hybrid-retrieval) · Dense embeddings fused with BM25 and reranked, with every constant found by sweep.
- [Idempotency, exactly-once effects and crash recovery](idempotency-exactly-once-effects-and-crash-recovery) · A restart never repeats a provider call, a broker restart never re-runs work the GPUs hold, and an agent's claimed completion is a claim.
- [Identity and access management for AI agents](identity-and-access-management-for-ai-agents) · I worked out, from real tenant evidence, how an AI employee legitimately answers, calls and acts inside Microsoft 365, with per-employee tokens minted server-side and never handed to a model.
- [Independent verification and adversarial review](independent-verification-and-adversarial-review) · Builders do not judge their own work. Quality assurance, a gatekeeper that accepts only delivered facts, and an adversarial reviewer on a different vendor's model are separate seats, and a FAIL stays a FAIL.
- [KV-cache engineering](kv-cache-engineering) · The key-value cache is the largest thing on the card after the weights. I moved it to the host in ActiveKV, kept it hot in the Inference Fabric's broker, and in both cases measured the bus.
- [Large-scale GPU data pipelines](large-scale-gpu-data-pipelines) · A generation pipeline that populated tens of millions of dataset items on two consumer GPUs, with persistent item identities, lease-based claiming and prompts baked at build time for cache reuse.
- [Large-scale refactoring with parity proof](large-scale-refactoring-with-parity-proof) · Rewrite a system, prove it is the same system. My governance platform's own refactors carry parity proofs, and the largest example is a GPU runtime ported to C++ without changing a token.
- [LD_PRELOAD symbol interposition](ld-preload-symbol-interposition) · Symbol interposition let me intercept runtime calls directly when the vendor's tracing path was itself distorting measurements.
- [Lease-based work claiming](lease-based-work-claiming) · Parallel workers claim work by lease, designed against the dead-tuple behaviour of PostgreSQL's concurrency model, so two workers never process the same item and nothing is lost on a crash.
- [Link-time plugin registration](link-time-plugin-registration) · A generated function is registered at link time so that it is fully wired or the build fails. There is no half-registered state.
- [Linux security primitives](linux-security-primitives) · Container limits, path safety, shell allow-lists, UID pinning and egress control are the floor under my agent runtime, not an afterthought.
- [LLM fine-tuning](llm-fine-tuning) · A full-parameter fine-tune of a 0.6B model on registry-generated data, finished in minutes, measured on a frozen set against a baseline that tied it.
- [MCP tool design](mcp-tool-design) · Tools shaped as jobs, cost stated on every call, every write read back, every create with a delete: the written standard every MCP tool in my estate must meet.
- [ML evaluation methodology](ml-evaluation-methodology) · Frozen evaluation sets, pre-registered targets, known-answer controls, a list of results never to quote, and a baseline built to beat me. It tied, and the tie is what I publish.
- [Model quantization](model-quantization) · A published 4-bit-weight quantization that fits a 27B model on one 32 GB card for 36 percent more throughput at 3 percent perplexity cost, an INT8 compressed history tier for ActiveKV, and FP8 serving on NVIDIA.
- [Multi-agent system architecture and orchestration](multi-agent-system-architecture-and-orchestration) · A governance control plane, a persona-driven runtime and a voice-first collaboration shell: three ways I have organised many agents around one body of work, with the state outside any model's head.
- [Multi-vendor LLM integration](multi-vendor-llm-integration) · Three frontier model families and local open-weight models run side by side in my programs, through subscription sessions, API seats and my own GPUs, with a terms-of-service firewall deciding which traffic may go where.
- [Network egress confinement](network-egress-confinement) · The most privileged agent seat in my estate is fenced: its only way out is a proxy that allows a handful of exact destinations.
- [Observability and alerting](observability-and-alerting) · SMS alerting is wired to the service fleet, with a metrics stack and dashboards beside it, and a status dashboard that says plainly what each service is doing.
- [Performance engineering and benchmarking](performance-engineering-and-benchmarking) · Fixed model, one variable at a time, negatives beside positives, and an intake screen that rejects gains tuned to the test fixture.
- [Policy-as-code enforcement](policy-as-code-enforcement) · Policy in my governance platform is enforced by hooks, not remembered by prompts: a lead cannot edit an artifact, work cannot dispatch before its evidence exists, a hook may never report an operation that did not happen.
- [PostgreSQL bulk-update engineering](postgresql-bulk-update-engineering) · Statement shape, batch width and index cost, each judged by what the database actually does with a write.
- [Prompt-injection-aware tooling](prompt-injection-aware-tooling) · Tool descriptions are attack surface. Shell-template injection fixtures are mandatory for the tool kind that needs them, and the discovery tool's description is capped by a test.
- [Provider-terms compliance in model routing](provider-terms-compliance-in-model-routing) · A terms-of-service firewall in the agent runtime decides which traffic may reach which provider, so a subscription session is used as its vendor permits.
- [Real-time audio pipeline engineering](real-time-audio-pipeline-engineering) · PCM framing, resampling, echo-cancellation reference, pacing and drop-on-reconnect: the audio path from a desk microphone or a Teams call to my own speech models.
- [Research data forensics](research-data-forensics) · I rebuild and prove a research dataset before I trust it.
- [Reversible infrastructure mutation](reversible-infrastructure-mutation) · Edits that touch several services happen in one rollback-protected transaction, and every create has a symmetric delete. The function generator is the worked example.
- [Schema-agnostic data access and SQL-injection defence](schema-agnostic-data-access-and-sql-injection-defence) · Database access in generated code goes through a schema resolver that validates every identifier; raw pools are excluded from the sandbox; SQL is never assembled from strings an agent wrote.
- [Schema and migration discipline](schema-and-migration-discipline) · Forward-only migrations, schema contracts and a baseline frozen as immutable. Schema is a contract, and I treat it that way.
- [Schema-driven build-time code generation](schema-driven-build-time-code-generation) · YAML tool schemas compile into dispatch at build time in my MCP gateway and the execution substrate, so a tool cannot be half-wired.
- [Site reliability engineering](site-reliability-engineering) · A declared systemd fleet, tunnelled ingress, a documented Redis topology and written runbooks keep my estate recoverable.
- [State-machine design for multi-agent workflows](state-machine-design-for-multi-agent-workflows) · Work-order lifecycles, stand-down and resume, and transition compilation: the governance platform is state machines all the way down.
- [Static analysis as tests](static-analysis-as-tests) · Static checks run as tests in my governance platform: a carve gate on imports, a check that no hook can surface a non-operation.
- [Streaming statistics in CUDA](streaming-statistics-in-cuda) · Welford and Chan moments, histogram quantiles and compare-and-swap float atomics, written once in a device library and tested on their own, so every metric kernel is numerically stable in single precision.
- [Synthetic training-data generation](synthetic-training-data-generation) · The capabilities model's training corpus is generated from the tool registry by a data factory, so the model is rebuilt from the catalog whenever the catalog changes.
- [Tiled pairwise kernels](tiled-pairwise-kernels) · One tiling design makes every quadratic cluster metric exact at a hundred thousand members, with bounded memory and no sampling.
- [Token-aware GPU batch scheduling](token-aware-gpu-batch-scheduling) · The token is the unit of GPU scheduling in my broker: shape-pure batches packed to each card's declared limits, across two different GPUs.
- [Vendor-integration reverse engineering](vendor-integration-reverse-engineering) · When vendor documentation runs out I probe the platform itself, capture the wire, and compose what actually works.
- [Web crawling and document extraction](web-crawling-and-document-extraction) · A native crawler and section extractor for PDFs, Markdown and HTML feed the reference index behind my memory service.
- [Webhook ingestion and verification](webhook-ingestion-and-verification) · Inbound vendor events are signature-checked, batched durably and delivered to the team that caused them, in the gateway and in the in-house social integrations.
- [Write-behind persistence](write-behind-persistence) · Writes in my substrate go through a write-behind queue and a batching writer, so producers never block on the database.
- [Zero-inbound network exposure](zero-inbound-network-exposure) · No host in my estate accepts an inbound connection. Everything arrives through authenticated tunnels or a private mesh, and every public surface is fronted by TLS and rate limits.

## framework (15)

- [Axum](axum) · Axum is the HTTP layer under most of my Rust services: the memory gateway, the voice engine's control surface, the execution substrate's endpoints.
- [CUTLASS](cutlass) · CUTLASS-for-SYCL is part of the kernel stack I patched on Intel's Xe2 architecture for ActiveKV's attention.
- [FastAPI](fastapi) · The OAuth authorization server and the earlier Python dispatch layer are FastAPI.
- [Handlebars](handlebars) · Handlebars templates drive the function generator's fourteen-file output.
- [Hugging Face Transformers](hugging-face-transformers) · Hugging Face Transformers is the training path for my capabilities model: a full fine-tune of every parameter, finished in minutes, rebuilt whenever the catalog changes.
- [Microsoft real-time media SDK](microsoft-real-time-media-sdk) · A .NET 8 media service on Microsoft's real-time media SDK, handling unmanaged buffers on the SDK's clock and joined to a Linux voice engine across clouds.
- [pybind11](pybind11) · pybind11 binds ActiveKV's C++ engine into vLLM and PyTorch; a line-by-line audit proves every remaining Python line is a framework contract.
- [PyO3](pyo3) · An earlier in-process Python binding for embeddings, replaced by a separate inference server.
- [PyTorch](pytorch) · ActiveKV extends PyTorch's XPU backend and ATen from native code; the capabilities model is a PyTorch fine-tune.
- [ratatui](ratatui) · A terminal console over my execution substrate's Redis control plane, for watching function services and steering them.
- [React](react) · React builds the Mattermost plugins, the Teams work tab and the meeting-stage app for Helix.
- [rmcp (Rust MCP SDK)](rmcp-rust-mcp-sdk) · The Rust MCP SDK underlies my memory gateway and the meeting action server.
- [sqlx](sqlx) · sqlx carries my Rust services' PostgreSQL access; where no table is known at compile time, I check against the schema itself instead.
- [Tokio](tokio) · Tokio is under every Rust service I run. Where the hot path is small, as in the broker's dispatch loop, I keep it synchronous on purpose and say why.
- [tree-sitter](tree-sitter) · tree-sitter parses a multi-language monorepo into the chunks and edges behind my code search and dependency graph.

## hardware (3)

- [Intel Arc GPUs](intel-arc-gpus) · An Intel Arc Pro GPU is ActiveKV's home: a 27B model serving 128,000-token histories on one 32 GB card, kernel patches on a new architecture, and a published quantization built for it.
- [NVIDIA Blackwell GPUs](nvidia-blackwell-gpus) · Consumer NVIDIA Blackwell GPUs carried the Inference Fabric, the capabilities model and early ActiveKV work, first on one card and then on two mismatched cards draining one broker queue.
- [NVMe (cold-tier storage)](nvme-cold-tier-storage) · The broker's cold tier is NVMe: billions of queued tokens survive a restart in shape-pure order.

## language (11)

- [Bash](bash) · Test harnesses, release scripts, proof runs and service glue across every system are shell.
- [C++](c-plus-plus) · ActiveKV's runtime is C++ throughout, ported from Python under bitwise-parity gates, and the Inference Fabric's TensorRT boundary is C++.
- [C#](c-sharp) · The Windows side of my Teams integration is C# on .NET 8: a media service on Microsoft's real-time SDK, screen-share publication, and a product MCP server later ported to the official .NET SDK.
- [CUDA C++](cuda-c-plus-plus) · I write CUDA where it earns its place: a cluster-health and vector-search engine for the newest NVIDIA architecture, and a tool-discovery decoder whose reductions are ordered so output bits never depend on the batch.
- [JavaScript](javascript) · Relays, meeting-stage apps, extension scripts and the OAuth consent surfaces are JavaScript where the platform demands it.
- [Lua](lua) · Lua scripts make the Redis control plane's job promotion atomic and keep the broker's hot-path bookkeeping on the server.
- [Python](python) · Python is where I prototype and where frameworks demand it: ActiveKV began in Python inside vLLM before the native port, the OAuth server is Python, and the training and evaluation harnesses are Python.
- [Rust](rust) · Rust is my systems language: about a million and a half lines across the governance platform, the agent runtime, the collaboration shell, the memory gateway, the execution substrate and the inference pipeline.
- [SQL](sql) · SQL is how I query the stores everything else projects from: work graphs, tuple statistics, retrieval tables, cost ledgers.
- [TypeScript](typescript) · TypeScript builds the meeting-stage app, the relay between Teams and my agent, the public site runtime, and the in-house social integrations.
- [YAML](yaml) · Tools, personas, execution profiles and tool schemas are YAML in my estate, compiled and hash-pinned rather than parsed at runtime.

## model (6)

- [Model families and types](model-families-and-types) · I pick a model for the job and the hardware it has to run on, then I change it until it fits.
- [Multilingual embedding model](multilingual-embedding-model) · the multilingual embedding model is the embedding model behind my code and reference search, served from a local text-embedding server.
- [Reranker model](reranker-model) · A cross-encoder reranker sits behind my hybrid retrieval, on a seam that tells load from breakage.
- [Speech recognition model](speech-recognition-model) · An open speech-recognition model is the recogniser in my voice engine, integrated rather than modified.
- [Speech synthesis model](speech-synthesis-model) · The neural speech model that gives Helix its voice in Teams calls, a local room and produced narration.
- [Text embedding models](text-embedding-models) · I ran a bake-off across embedding families for retrieval and replaced an incumbent chosen by habit with one chosen by measurement.

## platform (28)

- [Cargo](cargo) · Multi-crate workspaces, feature-gated builds and a carve gate that keeps product crates free of estate-specific imports.
- [Chrome extensions (Manifest V3)](chrome-extensions-manifest-v3) · A browser extension lets an agent act through my own authenticated browser session where no API exists, with duplicate-safe receipts and a read-back after every change.
- [Cloudflare Tunnel](cloudflare-tunnel) · Tunnelled ingress means my estate has no open inbound ports.
- [Cloudflare Workers](cloudflare-workers) · An edge worker exposes a trimmed, authenticated tool surface to a vendor's agent platform without opening the estate behind it.
- [ComfyUI](comfyui) · A node-based media pipeline runs as a GPU media studio behind my memory gateway, with provenance tracked on every generated asset.
- [Docker](docker) · Containers are how my agents are sandboxed, how GPU consumers are provisioned on local, LAN and cloud hosts, and how release images are proven.
- [FFmpeg](ffmpeg) · FFmpeg frames a headless Linux desktop as H.264 for screen sharing into Teams meetings and drives the media studio's transforms.
- [Git](git) · My governance platform reads git as evidence: witness, task and decision commits, authorship trailers, and the rule that every commit is pushed and nothing is rewritten.
- [GitLab](gitlab) · Self-hosted GitLab is where my agents open merge requests they are not allowed to merge, and where discovered defects are filed as issues.
- [Grafana](grafana) · Dashboards are how I captured the numbers on this site.
- [Hugging Face Hub](hugging-face-hub) · I published a 4-bit quantization of a 27-billion-parameter model with its card, provenance and measured trade-off.
- [Mattermost](mattermost) · An unmodified open-source team chat server hosts my multi-model collaboration shell, with bot seats for several vendors and a council mode that deliberates rather than fans out.
- [Meta Graph API](meta-graph-api) · An in-house integration with Meta's Graph API, with usage telemetry, a ledger of everything the app created, and signature-checked webhooks.
- [Microsoft Agent 365](microsoft-agent-365) · I provisioned a governed digital employee under Microsoft's Agent 365, and built the MCP server through which any model acts in a meeting as that specific employee.
- [Microsoft Azure](microsoft-azure) · Azure hosts the Windows side of my Teams integration: a media bridge with managed identity, vault-held secrets and authenticated access.
- [Microsoft Copilot Studio](microsoft-copilot-studio) · I expose a trimmed, authenticated tool surface to Microsoft Copilot Studio through an edge proxy, and worked out from the wire why its connector stalled after initialisation.
- [Microsoft Entra ID](microsoft-entra-id) · Entra Agent ID gives my digital employee its identity; I compose the Microsoft principals it involves into paths the platform actually accepts.
- [Microsoft Graph](microsoft-graph) · Microsoft Graph is how the employee reads mail, posts in meeting chat and answers calls, with tokens minted per employee and validated before use.
- [Microsoft Teams](microsoft-teams) · People call my digital employee in Teams and it answers; they invite it to meetings and it presents, shares a screen and calls on raised hands. It does not raise its own, because the platform offers no way to.
- [NGINX](nginx) · NGINX fronts the OAuth server and the estate's other web services with TLS and rate limits, ahead of any application code.
- [NVIDIA Nsight Systems](nvidia-nsight-systems) · Nsight traces are where I found what the engine was actually doing, and where I learned to check that the trace was not itself the cause.
- [Prometheus](prometheus) · Prometheus carries the numbers that decide whether GPUs earn their keep, follows a fleet that changes under it, and pages one operator's phone.
- [Public environmental data APIs](public-environmental-data-apis) · Public weather and environmental data feed a product-shaped MCP server that exposes 21 tools, with a trimmed surface for a vendor agent platform.
- [Reddit](reddit) · An in-house Reddit integration through my own browser session, with duplicate-safe receipts and a read-back after every change.
- [RunPod](runpod) · Rented cloud GPU spot capacity is one provisioning target behind my substrate's fail-closed daily budget; always available, never uncapped.
- [systemd](systemd) · Every service in my estate that stays up is a locked-down systemd unit; the agent runtime, the credential service and the governance watcher among them.
- [tmux](tmux) · tmux is how my governance platform drives vendors' interactive command-line tools as persistent governed sessions, and how I verify that a message actually landed.
- [X API](x-api) · An in-house X integration where one service owns the rate limit, the monthly budget and the send log, and never re-sends an action whose outcome is unknown.

## protocol (17)

- [ACME](acme) · Automated certificate issuance keeps my services' TLS current without a human in the loop, in the agent runtime and the access plane.
- [Agent Client Protocol (ACP)](agent-client-protocol-acp) · I built agents that speak the Agent Client Protocol so coding assistants can be driven as governed workers rather than chat windows.
- [CBOR](cbor) · Canonical CBOR encodes the vector store's RPC wire and the extraction specifications, so equal specifications are byte-identical.
- [GraphQL](graphql) · A typed Rust client for a cloud GPU provider's GraphQL API.
- [H.264](h-264) · H.264 framing from a headless Linux desktop to the Windows media bridge, so an AI meeting attendee can share a terminal or browser as it works.
- [JSON-RPC](json-rpc) · JSON-RPC is the transport under the Model Context Protocol surfaces I build and consume.
- [JSON Schema](json-schema) · Every work-order contract, tool definition and generated function surface in my estate is a JSON Schema, and schemas compile into dispatch at build time.
- [JSON Web Token (JWT)](json-web-token-jwt) · Scoped JWTs for agent seats, employee-scoped tokens for Microsoft identities, bearer introspection that fails closed. Identity in my systems is derived from the token, never from tool input.
- [MessagePack](messagepack) · Compact binary serialisation on the agent runtime's message bus and the broker's internal entries.
- [Model Context Protocol (MCP)](model-context-protocol-mcp) · Every agent in my estate reaches every tool through MCP: a gateway of 475 tools, generated servers, a product server ported to .NET, and a single discovery tool backed by a model.
- [OAuth 2.0](oauth-2-0) · I built an OAuth 2.0 authorization server for commercial AI assistants, with consent as the real control, and my memory gateway validates tokens from several issuers against published keys.
- [OpenAI-compatible API](openai-compatible-api) · An OpenAI-compatible endpoint is the common shape my local models, the voice engine and ActiveKV present to callers.
- [OpenAPI](openapi) · OpenAPI descriptions are the declarative input to my API integration platform and to the generated tool surfaces behind the memory gateway.
- [TLS and mTLS](tls-and-mtls) · TLS with hot certificate rotation on every public surface; mutual TLS between my hosts for LAN GPU provisioning.
- [Unix domain sockets](unix-domain-sockets) · Unix sockets are the transport between my governance hooks and their runtime, between the voice engine and its clients, and between the capabilities model's decoder and its callers.
- [WebAuthn](webauthn) · Hardware-key sign-in for the person who approves an OAuth grant, on an alternate entrypoint of the server, with the assistants' path left unchanged.
- [WebSocket](websocket) · One authenticated WebSocket per call carries the binary audio link between Teams and my voice engine, and survives a mid-call reconnect.

## runtime (9)

- [CUDA Driver API](cuda-driver-api) · My CUDA analytics engine talks to the driver API directly from Rust, built for a GPU architecture the Rust ecosystem had not caught up with.
- [Hugging Face Text Embeddings Inference](hugging-face-text-embeddings-inference) · A local text-embedding inference server serves the embedding model to the memory service, replacing an earlier in-process binding.
- [Intel oneAPI](intel-oneapi) · Intel's oneAPI stack is what ActiveKV's native engine and its kernel patches are built against, inside the vendor's own toolchain for ABI match.
- [NVIDIA TensorRT-LLM](nvidia-tensorrt-llm) · TensorRT-LLM is the engine under the Inference Fabric. I never touched its kernels; everything I gained came from how work was fed to it, and I tried it first for the capabilities model before closing that path on evidence.
- [NVIDIA TensorRT](nvidia-tensorrt) · Raw TensorRT backs the single-pass hidden-state extraction mode in the Inference Fabric's runtime.
- [oneDNN](onednn) · Patches to Intel's math library for a GPU architecture the ecosystem had not caught up with, each one held to bit-identical output.
- [ONNX Runtime](onnx-runtime) · ONNX Runtime serves embeddings in the evaluation harness and in the voice engine's lighter models.
- [SYCL](sycl) · ActiveKV's attention operators and its kernel patches on Intel Xe2 are SYCL, each gated on bit-identical outputs.
- [vLLM](vllm) · vLLM is the engine ActiveKV lives inside, patched at the scheduler, worker and attention backend, and the server under my local open-source models.

## Citation

Corey James. "Technologies." coreyjames.ai, 2026. https://coreyjames.ai/technologies/
