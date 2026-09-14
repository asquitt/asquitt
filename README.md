# Demario Asquitt

### Backend engineering, distributed systems, and AI agents you can inspect.

I build the systems around AI: how agents get permission to act, how their work is traced, how failures are recovered, and how we decide whether a change actually helped.

My projects span Python services, TypeScript applications, agent infrastructure, and evaluation tooling. I like following a problem all the way from an API contract to the person trying to use it.

[Portfolio](https://demario-portfolio.demarioasquitt.chatgpt.site/) · [LinkedIn](https://www.linkedin.com/in/demario-asquitt/) · [Email](mailto:demarioasquitt@gmail.com)

## Selected work

| Project | The problem I explored | Start here |
| --- | --- | --- |
| **[AgentHub](https://github.com/asquitt/agent-hub)** | Scoped agent identity, revocation, and accountable MCP tool calls | [Relay and signed receipts](https://github.com/asquitt/agent-hub/tree/main/src/relay) |
| **[AI Trace](https://github.com/asquitt/agent-trace)** | Following async AI workflows while controlling sensitive trace data | [Context and tracing](https://github.com/asquitt/agent-trace/tree/main/src/tracing) |
| **[AgentGuard](https://github.com/asquitt/agent-guard)** | Inspecting AI requests through detector pipelines and adversarial test cases | [Detection pipeline](https://github.com/asquitt/agent-guard/tree/main/agentguard-backend/backend/app/services/detection) |
| **[SynthArena](https://github.com/asquitt/synth-arena)** | Finding behavioral, cost, and latency regressions in agent evaluations | [Graders](https://github.com/asquitt/synth-arena/blob/main/packages/core/src/graders.ts) |
| **[Distributed KV Store](https://github.com/asquitt/distributed-kv-store)** | Consensus, fault tolerance, and durable state | [Repository](https://github.com/asquitt/distributed-kv-store) |
| **[Cove](https://github.com/asquitt/cove)** | Making task capture and planning more approachable | [iOS application](https://github.com/asquitt/cove) |

## How I approach engineering

**Make the boundary explicit.** A tool call needs scoped authority. A trace needs an owner. A retry needs a clear answer about what already happened.

**Make the claim inspectable.** I care about failure-path tests, reproducible examples, and readable implementation links. A local test and a deployed customer outcome answer different questions.

**Keep the product in view.** Reliability matters most when it helps someone complete their work. I enjoy the connection between backend design, clear interfaces, and useful products.

## Tools I work with

Python · TypeScript · SQL · FastAPI · React / Next.js · PostgreSQL · Redis / Celery · Docker

My main interests are backend platforms, distributed systems, AI infrastructure, observability, and developer tools.

## Let's build something useful

I'm interested in engineering roles and collaborations where I can own meaningful backend or AI infrastructure problems. If you're working on agent permissions, evaluation, tracing, or reliable workflow execution, I'd enjoy comparing notes.

**[Get in touch](mailto:demarioasquitt@gmail.com)** or open an issue on a project with a concrete question or small reproduction.
