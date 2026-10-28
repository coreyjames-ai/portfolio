# FAFODev



Canonical: https://coreyjames.ai/tools/fafodev/  
Author: Corey James · Published: 2026-10-28 · Kind: tool group  
Systems: [FAFO Core and Function Forge](https://github.com/coreyjames-ai/fafo-core) · [Inference Fabric](https://github.com/coreyjames-ai/inference-fabric) · [Agent Swarm](https://github.com/coreyjames-ai/agent-swarm) · [FAFOHive](https://github.com/coreyjames-ai/fafohive)  

## What was built

FAFODev is the server I use to build and operate [FAFO Core](https://coreyjames.ai/systems/fafo-core) and the [Inference Fabric](https://coreyjames.ai/systems/inference-fabric) through an AI assistant. I made a deliberate choice about its shape: one tool per subsystem, with an `action` argument that selects the operation. Eighteen tools carry 171 actions. An assistant only has to learn eighteen names, each tool returns its own documentation on request, and every subsystem's operations live in one place with one schema. Many of these tools are Core functions themselves, built with the function generator below, so the platform is operated through its own machinery. [Tools that build tools under governance](https://coreyjames.ai/stories/tools-that-build-tools-under-governance) tells the generator's story.

## Jobs, containers and GPUs

`control_plane_management` operates the control plane that runs every Core function, on the local host, in a dedicated container, or on remote GPU capacity.

- `execute_job` runs a job, optionally in a container on a chosen local or rented GPU, with the runtime injected into any image.
- `get_job_status` reports one job's live status.
- `control_function` sends live controls to a running function: pause, resume, emergency stop, scale workers, change batch size, stop a job, restart, quarantine or release from quarantine.
- `get_status` reports the control plane's and each function's health.
- `get_health_status` adds GPU and inference metrics to that health view.
- `get_history` returns the history of control actions.
- `create_service` turns a job definition into a long-running background service.
- `stop_service` stops a background service.
- `list_services` lists the services that are running.
- `list_containers` lists container history on local and rented hardware.
- `list_running_containers` lists running containers.
- `get_container_status` reports one container's status and metrics.
- `terminate_container` stops a container by hand.
- `list_available_images` lists the container images in the manifest.
- `validate_container_config` checks a container configuration before a job is submitted.
- `get_provider_docs` returns the configuration schema and examples for a compute provider.
- `get_budget_status` reports a schema's compute spending against its budget.
- `set_schema_budget_limits` sets a schema's default budget limits.
- `get_pricing_cache` shows cached provider prices, with local GPUs at zero.
- `get_local_gpu_queue` lists jobs waiting to fall back to a local GPU.
- `get_recovery_queue` lists jobs waiting for recovery after a failure.
- `trigger_recovery` starts recovery for a failed container.
- `get_events` returns recent container lifecycle events.
- `subscribe_events` subscribes to live event notifications.

`federated_node_management` runs persistent GPU inference nodes and the remote machines they live on. A node outlives any single job.

- `provision_node` brings up a GPU inference node or an agent-swarm member host, locally, on a LAN machine or on rented GPUs.
- `node_status` reports the nodes and their state.
- `terminate_node` shuts a node down.
- `drain_queues` forces a node to drain its queues now.
- `set_idle_timeout` sets how long a node waits idle before it drains.
- `list_available_images` lists the node images in the manifest.
- `list_available_engines` lists the built TensorRT-LLM engines.
- `setup_remote_host` onboards a spare LAN machine as a remote Docker host, with TLS, engine sync, registry access and monitoring.
- `teardown_remote_host` removes a remote host.
- `sync_engine_to_remote_host` copies engine directories to a registered host.
- `list_remote_hosts` lists the remote hosts and whether each is alive.
- `get_documentation` returns the tool's documentation.

## Building functions

`fafo_function_generator` writes a new Core function and wires it into every place a function has to be registered, so a developer writes only the business logic. A function is generated either for application processing, which reads, computes and writes back, or for bulk work done entirely inside PostgreSQL, and it can include the scaffolding for submitting inference work.

- `create_function` generates a new function and its files.
- `update_function` updates an existing function's wiring and documentation.
- `validate_function` checks a function's integration and that it compiles.
- `delete_function` removes a function and all of its registrations.
- `get_documentation` explains the two processing lanes with examples.

`service_testing_template` is the reference function the generator produces, used for smoke tests. Like the other generated functions, it runs as a one-time job or as a service triggered by queue depth, a timer or continuously.

- `submit_job` submits a smoke-test job for a schema.
- `get_documentation` returns its documentation.

## Data writes and admission

`db_writer_control` operates the shared database write service that every function writes through, with a main queue and a bulk queue.

- `get_status`, `get_info` and `health_check` report the service, its queues and its components.
- `get_queue_status` and `get_queue_metrics` report each queue's depth and performance.
- `get_logs` returns recent log entries.
- `pause` and `resume` pause and resume writing.
- `emergency_stop` shuts the service down immediately.
- `scale_workers`, `stop_workers` and `restart_workers` change the worker pool.
- `get_batch_rules` and `update_batch_rules` read and change how writes are batched.
- `update_config`, `update_controller_config` and `update_queue_config` change settings live.
- `get_config`, `persist_config`, `reload_config`, `get_config_history` and `diff_config` read, save, reload, trace and compare the configuration.
- `get_scaling_status`, `set_scaling_enabled`, `set_scaling_override` and `trigger_scaling_eval` read and steer automatic scaling.
- `cleanup_stale_consumers` clears queue consumers left behind by dead workers.

`admission_control` decides how much bulk work may run at once, so heavy jobs cannot overload the database.

- `status` reports admission state, capacity and active jobs.
- `active_jobs` details the jobs in progress.
- `queue_metrics` reports queue depths, throughput and bottlenecks.
- `get_job_history` returns past job performance.
- `get_performance_stats` analyses performance and bottlenecks.
- `get_entity_lineage` lists every job that touched given records.
- `get_capacity_recommendations` recommends capacity settings.
- `set_mode` switches admission off, to shadow mode or to enforcement.
- `set_tokens` sets the capacity limits.
- `set_refill_rates` sets how quickly capacity is returned.
- `set_control_loop` sets the control loop's timing.
- `force_release` releases admission locks left stuck by a failed job.

## Vectors and corpus analytics

`vsm_management` operates vector storage: per-model schemas whose vectors are held in shards, built in generations and recovered from checkpoints.

- `vsm_list_schemas` lists every schema that has vector storage.
- `vsm_get_schema_status` gives one schema's detailed status.
- `vsm_list_generations` lists a schema's generations.
- `vsm_list_shards` lists a schema's shards.
- `vsm_get_active_shards` shows which shards readers have mapped.
- `vsm_describe_shard` shows one shard's files, sizes and alignment.
- `vsm_get_metrics` returns the service's metrics.
- `vsm_health` reports whether the service is alive and its circuit state.
- `vsm_finalize_generation` finalizes a stuck generation.
- `vsm_cancel_generation` cancels a generation and marks it for deletion.
- `vsm_activate_generation` activates a built generation.
- `vsm_force_alignment_check` re-runs the alignment checks on a shard.
- `vsm_cleanup_old_generations` lists old generations that can be removed.
- `vsm_recovery_report` lists pending recovery records.
- `vsm_acknowledge_recovery` marks a recovery record resolved.
- `vsm_list_ready_checkpoints` lists checkpoints ready to be claimed.
- `vsm_describe_checkpoint` shows one checkpoint in full.
- `vsm_release_checkpoint` returns a claimed checkpoint to ready, for recovery.
- `validate_schema` checks a schema's setup.
- `get_job_status` reports a job's status.
- `get_documentation` returns the operator reference.
- `submit_job` exists for the common function contract and is refused, because this tool manages storage and never creates vectors.

`faiss_manager` builds and checks FAISS indexes over the stored vectors, with any index type and its parameters, memory, threads and optional GPU.

- `submit_job` runs a count, build or validation over the cluster, member or candidate indexes.
- `get_job_status` reports that job.
- `get_index_status` reports the state of a schema's indexes.
- `validate_schema` checks the schema the indexes are built from.
- `get_documentation` returns tested index configurations and a guide.

`embedding_management` runs the embedding pipeline.

- `health_stats` shows which schemas need embedding work.
- `submit_job` queues embedding work for a schema.
- `start_orchestrator` starts the workers that carry it out.

`cu_health_management` measures the health of the clusters in a corpus, at three depths.

- `view_tier1` returns seven basic metrics straight from the database.
- `process_tier2` queues fourteen statistical metrics for selected clusters.
- `process_tier3` queues seventeen advanced metrics computed with FAISS.

Clusters are selected by ID, age, metric thresholds, saturation pressure, growth events, quality or a random sample.

`cuda_metrics` computes the same cluster-health metrics with my CUDA kernels on the GPU.

- `submit_job` submits that computation for a schema, as a job or a triggered service.
- `get_documentation` returns its documentation.

`vec2vec_management` relieves clusters that are under pressure by moving members to better-matching clusters, comparing vectors to vectors. In forward mode it finds members that suit a pressured cluster's centre; in reverse mode it finds the best centre for each member of a pressured cluster.

- `analyze_pressure` measures cluster saturation and picks the candidates.
- `submit_job` queues the redistribution for a schema.

`gatekeeper` decides whether proposed new cluster members are accepted, held or rejected, by comparing them with existing cluster centres on similarity, distance, norm and population rules. It is a single-purpose tool with no actions: one call defines the job and the control plane runs it.

## Mining and probes

`probe_generator` builds probe sequences from linguistic material, designed to activate a model in useful ways during prefill. It sends them to an explicit buffer address and model consumer.

- `submit_job` submits probe generation for a schema, as a job or a triggered service.
- `get_documentation` returns its documentation.

`mining` runs a probe set through a TensorRT-LLM engine and captures a chosen internal tensor for every probe into vector storage. A run is deterministic and can be repeated safely.

- `submit_mining_run` creates a run after checking its extraction settings against the engine's capabilities.
- `get_mining_run_status` reports how many probes were submitted, processed and failed.
- `list_mining_runs` lists recent runs.
- `cancel_mining_run` cancels the probes not yet completed.
- `replay_mining_failures` puts failed probes back in line.
- `get_documentation` returns the operator reference.

## Agents and code

`agent_persona_launcher` launches and manages sandboxed agent containers from persona definitions, as part of [Agent Swarm](https://coreyjames.ai/systems/agent-swarm).

- `list_personas` lists the personas.
- `list_tools` lists the tools agents can be given.
- `reload_personas` and `reload_tools_catalog` reload either catalog without a restart.
- `preflight_managed_member` checks a governed team member's launch before it happens.
- `launch_agent` gives an agent its identity and record and starts its container.
- `recreate_agent` replaces an ended governed member under a recovery authorisation.
- `pause_agent` and `resume_agent` suspend and resume an agent's loop without losing its state.
- `kill_agent` stops one agent.
- `kill_persona` stops every running agent of a persona.
- `list_active` lists running agents.
- `get_agent_status` reports one agent.
- `get_agent_observations` returns what an agent recorded.
- `send_message` delivers a message to an agent's inbox.
- `list_endpoints` lists the model endpoints agents can reach.
- `get_documentation` returns the tool's documentation.

`swarm_management` gives the operator visibility into the agent swarm and control of its secrets.

- `list_active` lists active agents, filtered by persona, tool or host.
- `get_agent_status` reports one agent job.
- `catalog_version` shows whether every host runs the same tool catalog.
- `trace_a2a` follows one agent conversation hop by hop and finds the first unacknowledged message.
- `list_hosts` lists the swarm's hosts.
- `store_secret`, `rotate_secret` and `revoke_secret` store, replace and delete operator secrets.
- `list_secrets` lists secret names and metadata. Values are never returned.
- `import_secrets` imports secrets in bulk from a file on the server.
- `push_secret` sends a stored secret to a member host.
- `mint_swarm_transport_cert` issues the certificate the swarm's hosts use to talk to each other.
- `submit_job` and `get_documentation` follow the common function contract.

`gitlab_management` gives agents a governed path into GitLab and Git.

- `list_issues`, `get_issue` and `check_updates` read issues and watch them for changes.
- `post_comment` comments on an issue or merge request.
- `update_status` moves an issue through workflow labels.
- `create_merge_request` opens a merge request.
- `git_status`, `git_branch`, `git_checkout`, `git_pull`, `git_commit` and `git_push` run the repository operations, with commits made under the agent's identity.
- `get_documentation` returns the branching rules agents must follow.

Putting a whole subsystem behind one tool is the decision I would make again. An assistant can run GPU jobs, operate vector storage and launch agents with eighteen names to remember, and each tool explains itself when asked.

## What was verified

Each line is a claim the canonical page supports, with the figure as the page states it.

- Platform operations through an AI assistant: 18 tools with 171 actions let an assistant run jobs, containers and GPUs, control functions in flight and operate the inference fabric.
- MCP server design: one tool per subsystem with an action argument and self-documentation, many of them functions built by the platform's own generator.

## Related

- [Tools that build tools, under governance](https://github.com/coreyjames-ai/fafo-core/tree/main/stories/tools-that-build-tools-under-governance) · https://coreyjames.ai/stories/tools-that-build-tools-under-governance/
- System: [FAFO Core and Function Forge](https://github.com/coreyjames-ai/fafo-core)
- System: [Inference Fabric](https://github.com/coreyjames-ai/inference-fabric)
- System: [Agent Swarm](https://github.com/coreyjames-ai/agent-swarm)
- System: [FAFOHive](https://github.com/coreyjames-ai/fafohive)

## Citation

Corey James. "FAFODev." coreyjames.ai, 2026. https://coreyjames.ai/tools/fafodev/

```bibtex
@misc{coreyjames-fafodev,
  author = {Corey James},
  title = {FAFODev},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/tools/fafodev/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/tools/fafodev}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
