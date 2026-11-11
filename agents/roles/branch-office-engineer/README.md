# The Branch Office Engineer

**For a lead with machines in other offices and rented data centres.**

Canonical: https://coreyjames.ai/agents/roles/branch-office-engineer/  
Author: Corey James · Published: 2026-11-11 · Kind: agent role  

## The story

The agent brings a remote machine into the fleet over a connection that only dials out, so nothing at the site has to be opened to the internet. It places work there, relays what happens back to the main site and can rebuild the machine from nothing. Rented processors in a data centre are bought and released through the same agent.

## Function

[Infrastructure and operations](https://coreyjames.ai/agents/functions/infrastructure-and-operations/): Machines, queues, databases and spend, watched through the night.

## The crew

The specialists behind this role, grouped by the kind of work they do.

### Supervises other agents

- [Remote Agent Placer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/remote-agent-placer) · [page](https://coreyjames.ai/agents/specialists/remote-agent-placer/): Starts an AI worker on the machine best placed for the job, local or remote, and confirms that machine accepted it.

### Runs infrastructure

- [Remote Site Operator](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/remote-site-operator) · [page](https://coreyjames.ai/agents/specialists/remote-site-operator/): Joins a new remote machine to the fleet, gives it its own certificates, copies the models across, keeps it reachable without opening any inbound door in the firewall, and retires it cleanly when it is no longer needed.
- [Remote Machine Rebuilder](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/remote-machine-rebuilder) · [page](https://coreyjames.ai/agents/specialists/remote-machine-rebuilder/): Removes a remote machine, rejoins it from a clean state with the standard images and setup, starts the agents it should host, and has an independent reviewer check the result against a checklist.
- [GPU Server Onboarder](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/gpu-server-onboarder) · [page](https://coreyjames.ai/agents/specialists/gpu-server-onboarder/): This agent prepares a newly built AI engine to take work from the shared queue by writing and checking the settings files it needs.
- [Cloud GPU Buyer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/cloud-gpu-buyer) · [page](https://coreyjames.ai/agents/specialists/cloud-gpu-buyer/): Rents cloud GPUs only when the day's budget allows, prefers the cheapest current spot price, connects them back to your private network over an outbound link, and hands them back as soon as the work is done or the money runs out.
- [GPU Fleet Manager](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/gpu-fleet-manager) · [page](https://coreyjames.ai/agents/specialists/gpu-fleet-manager/): Starts a GPU worker on whichever machine you name, tells you what is running where, and shuts down idle workers with their final cost.
- [Planned Maintenance Coordinator](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/planned-maintenance-coordinator) · [page](https://coreyjames.ai/agents/specialists/planned-maintenance-coordinator/): Drains work, takes the database backup, shuts the services down in the documented order, brings them back in order, and checks each stage before moving on.
- [Model Courier](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/model-courier) · [page](https://coreyjames.ai/agents/specialists/model-courier/): Copies each new model build to the remote machines that serve it and confirms every copy arrived complete.
- [New Render Machine Setup Technician](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/new-render-machine-setup-technician) · [page](https://coreyjames.ai/agents/specialists/new-render-machine-setup-technician/): Brings a new graphics machine into service: confirms the GPU, starts the service, registers the models already on disk, runs a test image and a test video and shuts down.
- [Cloud Compute Dispatcher](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/cloud-compute-dispatcher) · [page](https://coreyjames.ai/agents/specialists/cloud-compute-dispatcher/): This agent picks an image, checks the container settings, runs the job on local or rented GPUs, keeps an eye on it and shuts the container down when it is done.
- [Idle Machine Drainer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/idle-machine-drainer) · [page](https://coreyjames.ai/agents/specialists/idle-machine-drainer/): Sets how long a machine may sit idle, empties its queues when the time is up and shuts it down.

### Audits and guards

- [Secrets and Certificates Officer](https://github.com/coreyjames-ai/portfolio/tree/main/agents/specialists/secrets-and-certificates-officer) · [page](https://coreyjames.ai/agents/specialists/secrets-and-certificates-officer/): Keeps every credential and certificate in one locked store.

## The engineering behind this role

- [One call to a GPU anywhere](https://coreyjames.ai/stories/one-call-to-a-gpu-anywhere/): Engineering story
- [Built for Blackwell](https://coreyjames.ai/stories/built-for-blackwell/): Engineering story

## Citation

Corey James. "The Branch Office Engineer." coreyjames.ai, 2026. https://coreyjames.ai/agents/roles/branch-office-engineer/

```bibtex
@misc{coreyjames-agent-role-branch-office-engineer,
  author = {Corey James},
  title = {The Branch Office Engineer},
  year = {2026},
  howpublished = {\url{https://coreyjames.ai/agents/roles/branch-office-engineer/}},
  note = {GitHub copy: https://github.com/coreyjames-ai/portfolio/tree/main/agents/roles/branch-office-engineer}
}
```

Part of [Corey James's portfolio](https://github.com/coreyjames-ai/portfolio) · site: https://coreyjames.ai/ · MCP server: https://coreyjames.ai/mcp · agent card: https://coreyjames.ai/.well-known/agent.json
