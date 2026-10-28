# zero-trust and zero-inbound networking

Pages on coreyjames.ai that demonstrate this skill, decided at build time against every page (highest first).

Canonical: https://coreyjames.ai/llms.txt  
Author: Corey James · Published: 2026-10-28 · Kind: skill index  

| Page | Result | Kind |
| --- | --- | --- |
| [Zero-inbound network exposure](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/zero-inbound-network-exposure) · [page](https://coreyjames.ai/technologies/zero-inbound-network-exposure/) | No host in my estate accepts an inbound connection. Everything arrives through authenticated tunnels or a private mesh, and every public surface is fronted by TLS and rate limits. | technology |
| [Site reliability engineering](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/site-reliability-engineering) · [page](https://coreyjames.ai/technologies/site-reliability-engineering/) | A declared systemd fleet, tunnelled ingress, a documented Redis topology and written runbooks keep my estate recoverable. | technology |
| [Cloudflare Tunnel](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/cloudflare-tunnel) · [page](https://coreyjames.ai/technologies/cloudflare-tunnel/) | Tunnelled ingress means my estate has no open inbound ports. | technology |
| [Federated compute provisioning](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/federated-compute-provisioning) · [page](https://coreyjames.ai/technologies/federated-compute-provisioning/) | One call stands up GPU capacity on a local card, a LAN workstation over mutual TLS, or rented cloud spot capacity, behind a fail-closed daily budget. | technology |
| [Auth and access plane](https://github.com/coreyjames-ai/auth-and-access-plane) · [page](https://coreyjames.ai/systems/auth-and-access-plane/) | How commercial AI assistants and my own agents reach a private tool estate: OAuth, token validation, edge exposure and an operations layer | system |
| [NGINX](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/nginx) · [page](https://coreyjames.ai/technologies/nginx/) | NGINX fronts the OAuth server and the estate's other web services with TLS and rate limits, ahead of any application code. | technology |
| [Microsoft Copilot Studio](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/microsoft-copilot-studio) · [page](https://coreyjames.ai/technologies/microsoft-copilot-studio/) | I expose a trimmed, authenticated tool surface to Microsoft Copilot Studio through an edge proxy, and worked out from the wire why its connector stalled after initialisation. | technology |
| [One call to a GPU anywhere](https://github.com/coreyjames-ai/fafo-core/tree/main/stories/one-call-to-a-gpu-anywhere) · [page](https://coreyjames.ai/stories/one-call-to-a-gpu-anywhere/) | Provisioning a GPU consumer node on the workbench, on a LAN host or in the cloud with one tool call, under a daily budget that only a human can set | story |
| [Unix domain sockets](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/unix-domain-sockets) · [page](https://coreyjames.ai/technologies/unix-domain-sockets/) | Unix sockets are the transport between my governance hooks and their runtime, between the voice engine and its clients, and between the capabilities model's decoder and its callers. | technology |
| [Microsoft Azure](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/microsoft-azure) · [page](https://coreyjames.ai/technologies/microsoft-azure/) | Azure hosts the Windows side of my Teams integration: a media bridge with managed identity, vault-held secrets and authenticated access. | technology |
| [TLS and mTLS](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/tls-and-mtls) · [page](https://coreyjames.ai/technologies/tls-and-mtls/) | TLS with hot certificate rotation on every public surface; mutual TLS between my hosts for LAN GPU provisioning. | technology |
| [Cloudflare Workers](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/cloudflare-workers) · [page](https://coreyjames.ai/technologies/cloudflare-workers/) | An edge worker exposes a trimmed, authenticated tool surface to a vendor's agent platform without opening the estate behind it. | technology |
| [rmcp (Rust MCP SDK)](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/rmcp-rust-mcp-sdk) · [page](https://coreyjames.ai/technologies/rmcp-rust-mcp-sdk/) | The Rust MCP SDK underlies my memory gateway and the meeting action server. | technology |

## Citation

Corey James. "zero-trust and zero-inbound networking: evidence on coreyjames.ai." 2026. https://coreyjames.ai/llms.txt
