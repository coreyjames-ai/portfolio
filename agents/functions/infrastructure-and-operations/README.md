# Infrastructure and operations

**Machines, queues, databases and spend, watched through the night.**

Canonical: https://coreyjames.ai/agents/functions/infrastructure-and-operations/  
Author: Corey James · Published: 2026-11-11 · Kind: agent function  

## The roles

- [The Night Shift](https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/night-shift) · [page](https://coreyjames.ai/agents/roles/night-shift/): For a one-person operations team.
- [The Spend Controller](https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/spend-controller) · [page](https://coreyjames.ai/agents/roles/spend-controller/): For whoever signs off on compute spend.
- [The Branch Office Engineer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/branch-office-engineer) · [page](https://coreyjames.ai/agents/roles/branch-office-engineer/): For a lead with machines in other offices and rented data centres.
- [The Database Guard](https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/database-guard) · [page](https://coreyjames.ai/agents/roles/database-guard/): For a team whose database takes writes from many directions.
- [The Security Officer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/security-officer) · [page](https://coreyjames.ai/agents/roles/security-officer/): For a security lead.
- [The Studio Engineer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/studio-engineer) · [page](https://coreyjames.ai/agents/roles/studio-engineer/): For a studio or IT lead with graphics machines.
- [The Pipeline Foreman](https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/pipeline-foreman) · [page](https://coreyjames.ai/agents/roles/pipeline-foreman/): For a data team lead who needs a new processing job by Thursday.
- [The Watch Office](https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/watch-office) · [page](https://coreyjames.ai/agents/roles/watch-office/): For an operations lead who wants one screen and alerts that mean something.
- [The Safe Change Desk](https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/safe-change-desk) · [page](https://coreyjames.ai/agents/roles/safe-change-desk/): For an operations lead who has to change a live system on a weekday.
- [The Housekeeper](https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/housekeeper) · [page](https://coreyjames.ai/agents/roles/housekeeper/): For an operations lead whose systems collect clutter.

## Specialists these roles share

- [Alert Tuner](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/alert-tuner) · [page](https://coreyjames.ai/agents/specialists/alert-tuner/): This agent keeps alert rules and text-message delivery working by testing each rule and its route from start to finish.
- [Batch Job Controller](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/batch-job-controller) · [page](https://coreyjames.ai/agents/specialists/batch-job-controller/): Runs a large job on a local card or a rented one, pauses, scales or stops it mid-flight, turns a one-off job into an always-on service, and isolates a job that misbehaves.
- [Cloud Compute Dispatcher](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/cloud-compute-dispatcher) · [page](https://coreyjames.ai/agents/specialists/cloud-compute-dispatcher/): This agent picks an image, checks the container settings, runs the job on local or rented GPUs, keeps an eye on it and shuts the container down when it is done.
- [Database Traffic Controller](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/database-traffic-controller) · [page](https://coreyjames.ai/agents/specialists/database-traffic-controller/): Keeps heavy bulk writes from flattening the database: it prices each write by its expected load, lets cheap work through, holds heavy work until there is room, and tunes the write workers.
- [Fleet Help Desk](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/fleet-help-desk) · [page](https://coreyjames.ai/agents/specialists/fleet-help-desk/): Answers plain questions such as "what is running on which GPU", "what has today cost" or "which machine is free" by picking the right fleet tools for the question.
- [GPU Spend and Power Guard](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/gpu-spend-and-power-guard) · [page](https://coreyjames.ai/agents/specialists/gpu-spend-and-power-guard/): Keeps rendering inside the daily spend limit and the office's power limit: no job starts without budget, and only one graphics card runs flat out at a time.
- [Idle Machine Drainer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/idle-machine-drainer) · [page](https://coreyjames.ai/agents/specialists/idle-machine-drainer/): Sets how long a machine may sit idle, empties its queues when the time is up and shuts it down.
- [Launch Pre-flight Checker](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/launch-pre-flight-checker) · [page](https://coreyjames.ai/agents/specialists/launch-pre-flight-checker/): Checks the machine image, the settings and the budget before a job starts, and names what is wrong while fixing it is still free.
- [Machine Decommissioner](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/machine-decommissioner) · [page](https://coreyjames.ai/agents/specialists/machine-decommissioner/): Takes a retired machine out of the fleet, revokes its certificates and confirms nothing still routes work to it.
- [New Render Machine Setup Technician](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/new-render-machine-setup-technician) · [page](https://coreyjames.ai/agents/specialists/new-render-machine-setup-technician/): Brings a new graphics machine into service: confirms the GPU, starts the service, registers the models already on disk, runs a test image and a test video and shuts down.
- [Night-Shift Fleet Watch](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/night-shift-fleet-watch) · [page](https://coreyjames.ai/agents/specialists/night-shift-fleet-watch/): Watches machines, GPUs and services overnight, texts your phone only for what matters, runs the standard health checks before waking you, and has a summary ready in the morning.
- [On-call Pager](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/on-call-pager) · [page](https://coreyjames.ai/agents/specialists/on-call-pager/): It turns each alert into a short text message on the on-call phone.
- [Planned Maintenance Coordinator](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/planned-maintenance-coordinator) · [page](https://coreyjames.ai/agents/specialists/planned-maintenance-coordinator/): Drains work, takes the database backup, shuts the services down in the documented order, brings them back in order, and checks each stage before moving on.
- [Remote Machine Rebuilder](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/remote-machine-rebuilder) · [page](https://coreyjames.ai/agents/specialists/remote-machine-rebuilder/): Removes a remote machine, rejoins it from a clean state with the standard images and setup, starts the agents it should host, and has an independent reviewer check the result against a checklist.
- [Secrets and Certificates Officer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/secrets-and-certificates-officer) · [page](https://coreyjames.ai/agents/specialists/secrets-and-certificates-officer/): Keeps every credential and certificate in one locked store.
- [Service Caretaker](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/service-caretaker) · [page](https://coreyjames.ai/agents/specialists/service-caretaker/): This agent watches the status, memory and logs of every core service and restarts only the services it is allowed to restart.
- [Smoke Test Runner](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/smoke-test-runner) · [page](https://coreyjames.ai/agents/specialists/smoke-test-runner/): Sends a small harmless batch through the service, once or on a trigger, and confirms it came out the other end.
- [Stuck Job Unblocker](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/stuck-job-unblocker) · [page](https://coreyjames.ai/agents/specialists/stuck-job-unblocker/): Finds the locks left behind by dead jobs, confirms nothing live depends on them and releases them so the queue moves again.
- [Throttle Rehearsal Analyst](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/throttle-rehearsal-analyst) · [page](https://coreyjames.ai/agents/specialists/throttle-rehearsal-analyst/): Runs a new limit in rehearsal mode, where every decision is logged and nothing is delayed, then reports which jobs would have waited before the limit is enforced.
- [Throughput Tuner](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/throughput-tuner) · [page](https://coreyjames.ai/agents/specialists/throughput-tuner/): Adjusts how work is batched and flushed, from a careful standard setting to a very high-volume one, and measures the result.
- [Worker Fleet Scaler](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/worker-fleet-scaler) · [page](https://coreyjames.ai/agents/specialists/worker-fleet-scaler/): This agent adds or removes background workers as the backlog grows and shrinks, restarts stuck ones and clears out dead connections.
- [Write Queue Firefighter](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/write-queue-firefighter) · [page](https://coreyjames.ai/agents/specialists/write-queue-firefighter/): Takes the page when the database write queue backs up, follows the recovery procedure, drains the queue if it has to, and confirms that writes are flowing again.

## The engineering behind these roles

- [High-throughput batch inference and embeddings](https://coreyjames.ai/capabilities/high-throughput-batch-inference/): Capability
- [One call to a GPU anywhere](https://coreyjames.ai/stories/one-call-to-a-gpu-anywhere/): Engineering story
- [Pricing writes by what they cost the database](https://coreyjames.ai/stories/pricing-writes-by-what-they-cost/): Engineering story
- [The hardening fix that locked everyone out](https://coreyjames.ai/stories/the-hardening-fix-that-locked-everyone-out/): Engineering story

## Citation

Corey James. "Infrastructure and operations." coreyjames.ai, 2026. https://coreyjames.ai/agents/functions/infrastructure-and-operations/

```bibtex
@misc{coreyjames-agent-function-infrastructure-and-operations,
  author = {Corey James},
  title = {Infrastructure and operations},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/functions/infrastructure-and-operations/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/functions/infrastructure-and-operations}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
