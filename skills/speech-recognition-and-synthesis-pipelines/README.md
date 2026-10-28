# speech recognition and synthesis pipelines

Pages on coreyjames.ai that demonstrate this skill, decided at build time against every page (highest first).

Canonical: https://coreyjames.ai/llms.txt  
Author: Corey James · Published: 2026-10-28 · Kind: skill index  

| Page | Result | Kind |
| --- | --- | --- |
| [Voice agents in calls and meetings](https://github.com/coreyjames-ai/portfolio/tree/main/research/capabilities/voice-agents-in-meetings) · [page](https://coreyjames.ai/capabilities/voice-agents-in-meetings/) | Speech recognition, synthesis and turn-taking on my own hardware, joined to the platforms people already use | capability |
| [Helix](https://github.com/coreyjames-ai/helix) · [page](https://coreyjames.ai/systems/helix/) | Humans and several AI minds in one room, and one colleague who can be reached wherever the work is: in team chat, by voice, and in a Teams call | system |
| [ONNX Runtime](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/onnx-runtime) · [page](https://coreyjames.ai/technologies/onnx-runtime/) | ONNX Runtime serves embeddings in the evaluation harness and in the voice engine's lighter models. | technology |
| [Speech recognition model](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/speech-recognition-model) · [page](https://coreyjames.ai/technologies/speech-recognition-model/) | An open speech-recognition model is the recogniser in my voice engine, integrated rather than modified. | technology |
| [Speech synthesis model](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/speech-synthesis-model) · [page](https://coreyjames.ai/technologies/speech-synthesis-model/) | The neural speech model that gives Helix its voice in Teams calls, a local room and produced narration. | technology |
| [One percent network, seventy-eight percent GPU](https://github.com/coreyjames-ai/helix/tree/main/stories/one-percent-network-seventy-eight-percent-gpu) · [page](https://coreyjames.ai/stories/one-percent-network-seventy-eight-percent-gpu/) | A slow Teams turn was blamed on the cloud hop; measurement showed the network was about one percent of it and a speech GPU shared with an embedding service was most of the rest, so the compute moved and the cloud stayed | story |
| [Building the streaming my speech model did not ship](https://github.com/coreyjames-ai/helix/tree/main/stories/building-the-streaming-my-speech-model-did-not-ship) · [page](https://coreyjames.ai/stories/building-the-streaming-my-speech-model-did-not-ship/) | The open-weight voice model I chose had no streaming hook, so I ported its token loop, decoded its audio in chunks and pinned its diffusion noise so the joins are seamless | story |
| [Real-time audio pipeline engineering](https://github.com/coreyjames-ai/portfolio/tree/main/technologies/real-time-audio-pipeline-engineering) · [page](https://coreyjames.ai/technologies/real-time-audio-pipeline-engineering/) | PCM framing, resampling, echo-cancellation reference, pacing and drop-on-reconnect: the audio path from a desk microphone or a Teams call to my own speech models. | technology |
| [Saying numbers out loud](https://github.com/coreyjames-ai/helix/tree/main/stories/saying-numbers-out-loud) · [page](https://coreyjames.ai/stories/saying-numbers-out-loud/) | A chemical formula came out as a sneeze and a thousand as ten thousand; a speech contract and a deterministic scrubber give the voice speakable text while the screen keeps the written answer | story |
| [The same brain, typed or spoken](https://github.com/coreyjames-ai/helix/tree/main/stories/the-same-brain-typed-or-spoken) · [page](https://coreyjames.ai/stories/the-same-brain-typed-or-spoken/) | Why a spoken request and a typed request produce exactly one durable turn in the same conversation, and what it took to keep the two from drifting apart | story |
| [A proof that proved nothing](https://github.com/coreyjames-ai/helix/tree/main/stories/a-proof-that-proved-nothing) · [page](https://coreyjames.ai/stories/a-proof-that-proved-nothing/) | An echo-cancellation score looked excellent until an unrelated reference scored higher; the rebuilt proof uses a negative control, and the same discipline runs through the voice engine's tests | story |

## Citation

Corey James. "speech recognition and synthesis pipelines: evidence on coreyjames.ai." 2026. https://coreyjames.ai/llms.txt
