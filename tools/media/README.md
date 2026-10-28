# Media and image generation



Canonical: https://coreyjames.ai/tools/media/  
Author: Corey James · Published: 2026-10-28 · Kind: tool group  
Systems: [FAFOHive](https://github.com/coreyjames-ai/fafohive) · [Helix](https://github.com/coreyjames-ai/helix)  

## What was built

I wanted any agent in my estate to be able to make images, video and narration on my own GPUs, without anyone hand-starting a ComfyUI server or copying files between machines. The hard parts are around the rendering: a GPU is shared with other work, model files are large, a render can finish while its delivery fails, and an agent that retries blindly burns GPU time on work it already did. So these 33 tools treat every step as a durable operation with its own identifier. Starting a service goes through the compute budget. Model downloads are planned before they run and checked after. A render and its delivery are tracked separately, so a failed copy is repeated without rendering again. The service runs as a controller on each media host and the hub forwards these tools to it, as described on the [FAFOHive](https://coreyjames.ai/systems/fafohive) page. Narration uses the same voice service as [Helix](https://coreyjames.ai/systems/helix).

## Hosts and services

`media_list_hosts` lists the media machines, their GPUs and whether they are reachable.

`media_list_service_profiles` lists the prepared ComfyUI service configurations on a host, with their mounts and GPU compatibility.

`media_start_service` starts a managed ComfyUI instance on a chosen GPU from one of those profiles, after the compute budget admits it.

`media_stop_service` stops one instance, either letting its jobs drain or cancelling them. Installed models and files stay.

`media_restart_service` restarts one instance with the same drain or cancel choice and a fresh budget admission, without touching other GPU work.

`media_service_status` reports an instance's health, GPU, queue and errors, which separates a start request from a service that is ready.

`media_service_logs` reads a page of an instance's logs, with secrets redacted and a cursor for the next page.

`media_operation_status` returns the stored outcome of any media operation by its identifier. It is how an agent resolves an uncertain start, transfer or narration.

## Models

`comfy_list_models` lists model and LoRA files, showing separately whether each is present, intact and visible to the loaders.

`comfy_get_model` shows one model's origin, installed locations, dependencies and what the loaders report about it, which explains why a file that exists can still be unusable.

`comfy_inspect_model_source` examines named files in a Hugging Face repository at an exact revision before anything is downloaded.

`comfy_check_model_access` tests whether the configured Hugging Face access can reach those files, separating a working login from repository access and licence consent.

`comfy_prepare_model_download` builds a fixed download plan with the exact files, revision, destinations and bytes required, so the installation can be checked before it starts.

`comfy_download_model` carries out a prepared plan with server-held access, checks the files and registers them in the inventory.

`comfy_cancel_model_download` stops one download, keeping its partial progress and anything already installed.

`comfy_verify_model` checks the bytes of an installed model when it looks damaged.

`comfy_refresh_models` compares the inventory with what a running instance's loaders can see, without interrupting its work.

`comfy_reconcile_models` finds models that were copied into the model folders by hand and adds them to the inventory.

`comfy_release_models` unloads cached models from the GPU of an idle instance. The files stay on disk.

## Workflows and jobs

`comfy_list_nodes` lists the node types a particular instance actually has installed.

`comfy_get_node_schema` shows one node type's inputs, outputs and loader choices, which is the wiring contract for a workflow.

`comfy_validate_workflow` checks a workflow graph for problems before it runs.

`comfy_submit_workflow` queues a workflow with explicit input bindings and an exact output destination, and returns a receipt that tracks rendering and delivery separately.

`comfy_job_status` shows a job's state and errors next to its delivery result, so a failure is placed in generation or in transfer.

`comfy_job_events` reads a job's progress events, with optional waiting and a cursor.

`comfy_cancel_job` cancels one job without clearing the rest of the queue.

`comfy_job_outputs` lists the files a job produced and where each one was delivered.

## Media files and narration

`media_stage_input` copies an exact source file from a host into an instance's staging area and returns a reference a workflow can load.

`media_deliver_output` copies a finished file to an exact host and filename, checking size and hash. It repeats a delivery without repeating the render.

`media_probe` reads a media file's metadata with FFprobe without changing it.

`media_transform` applies FFmpeg operations: transcode, resize and crop, concatenate, normalize audio, burn in subtitles, or put narration under video.

`media_list_voices` lists the configured narration voices.

`media_synthesize_narration` turns text into a WAV file with a chosen voice and delivers it to an exact destination.

These tools are how I make an agent a reliable user of expensive hardware: every action is admitted, identified, resumable and checked, and the agent always knows which part of a job failed.

## What was verified

Each line is a claim the canonical page supports, with the figure as the page states it.

- GPU media generation for AI agents: 33 tools let an agent start a managed ComfyUI service on a chosen GPU, plan model downloads, render images and video and produce narration.
- Durable operations design: every step has its own identifier, starts go through the compute budget, and a render is tracked apart from its delivery so a failed copy never re-renders.

## Related

- System: [FAFOHive](https://github.com/coreyjames-ai/fafohive)
- System: [Helix](https://github.com/coreyjames-ai/helix)

## Citation

Corey James. "Media and image generation." coreyjames.ai, 2026. https://coreyjames.ai/tools/media/

```bibtex
@misc{coreyjames-media,
  author = {Corey James},
  title = {Media and image generation},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/tools/media/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/tools/media}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
