<a href="https://github.com/asquitt#selected-work">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/banner-dark.svg">
    <img alt="Demario Asquitt: I build what sits between an AI agent's next action and production. AgentHub decides whether it may act, AgentGuard checks whether the input is hostile, AgentTrace records what happened, SynthArena measures whether a change helped." src="assets/banner-light.svg" width="100%">
  </picture>
</a>

<p align="center">
  <a href="https://demario-portfolio.demarioasquitt.chatgpt.site/"><b>Portfolio</b></a> ·
  <a href="https://www.linkedin.com/in/demario-asquitt/"><b>LinkedIn</b></a> ·
  <a href="mailto:demarioasquitt@gmail.com"><b>Email</b></a>
</p>

Most agent demos stop at *"it called the tool."* My work starts there:

> **Was it allowed to?** &nbsp;**Was the input hostile?** &nbsp;**What actually happened?** &nbsp;**Did the last change make it better?**

I'm a software engineer who builds backend and AI infrastructure. Each question above is its own open-source repo, written as production code with real tests, migrations, CI, and failure-path handling, not as a notebook.

## Selected work

| | Project | What's hard about it | Read this first |
|:-:|---|---|---|
| 🔐 | **[AgentHub](https://github.com/asquitt/agent-hub)**<br><sub>Python · FastAPI · MCP</sub> | Agent identity with **attenuating delegation**. Authority is rechecked at the network boundary, so a revoked credential can't slip through. Crash-safe idempotency keeps an *unknown* outcome instead of blindly replaying it, and every call gets an **Ed25519-signed receipt**. | [`relay/service.py`](https://github.com/asquitt/agent-hub/blob/main/src/relay/service.py) |
| 🛡️ | **[AgentGuard](https://github.com/asquitt/agent-guard)**<br><sub>Python · Celery · Next.js</sub> | An LLM proxy with **21 pluggable detectors** (prompt injection, MCP security, memory exfiltration, scope enforcement, and more). Twelve run inline in the request path and nine run as background analysis. A red-team engine mutates attacks across Unicode, encodings, Markdown, and multi-turn escalation. | [`detection/pipeline.py`](https://github.com/asquitt/agent-guard/blob/main/agentguard-backend/backend/app/services/detection/pipeline.py) |
| 🔭 | **[AgentTrace](https://github.com/asquitt/agent-trace)**<br><sub>Python · PostgreSQL · Celery</sub> | Trace context that survives nested `async` calls *and* queue hops. Storage is tenant-scoped, prompt capture is opt-in, and a durable outbox with claim and expiry recovery makes notifications survive retries. | [`tracing/context.py`](https://github.com/asquitt/agent-trace/blob/main/src/tracing/context.py) |
| 🧪 | **[SynthArena](https://github.com/asquitt/synth-arena)**<br><sub>TypeScript · pnpm monorepo</sub> | Agent evals beyond one lucky run: repeated trials, composable graders, and **regression diffs** that catch a newly broken scenario hidden by a better average, with cost and latency deltas alongside. | [`replay/regression.ts`](https://github.com/asquitt/synth-arena/blob/main/packages/replay/src/regression.ts) |

**Also built**

- 📱 **[Cove](https://github.com/asquitt/cove)**: an iPhone app (Swift, SwiftUI, SwiftData) for adults with ADHD, run as a privacy-first field study with pre-declared go/no-go criteria. All data stays on the device.
- 🌿 **[NatureDex](https://github.com/asquitt/NatureDex)**: a cross-platform plant classifier and collection app. **1st Overall at BackyardHacks.**
- 🎓 Before this, I built a conversational AI platform that gives universities self-serve access to course, tuition, and admissions data. It handles **100K+ chatbot interactions a month** (FastAPI, Java, Scala, Postgres, Elasticsearch, Kafka, and a WCAG 2.1-compliant Next.js front end).

## How I build

- **Boundaries before features.** Every tool call has scoped authority, every trace has an owner, and every retry knows what already happened.
- **Claims you can check.** Failure-path tests, runnable examples, and READMEs that state what the code *doesn't* do.
- **Product in view.** Reliability matters because someone is trying to get work done. I like following a problem from the API contract to the person using it.

## Toolbox

<p>
  <a href="#toolbox"><img src="https://skillicons.dev/icons?i=python,ts,go,swift,fastapi,nextjs,react,postgres,redis,kafka,elasticsearch,docker,kubernetes,githubactions&perline=14" alt="Python, TypeScript, Go, Swift, FastAPI, Next.js, React, PostgreSQL, Redis, Kafka, Elasticsearch, Docker, Kubernetes, GitHub Actions"></a>
</p>

## Recognition

- 🥇 **1st Place, NEDSI Annual Conference 2022**: multilingual sentiment analysis to predict threats from social media
- 🥇 **1st Overall, BackyardHacks**: NatureDex

---

<sub>Open to backend and AI-infrastructure roles. If you're working on agent permissions, evals, tracing, or reliable workflow execution, <a href="mailto:demarioasquitt@gmail.com">let's talk</a>. Earlier work (2020–2023) lives at <a href="https://github.com/demarioasquitt">@demarioasquitt</a>, an account I no longer have access to.</sub>
