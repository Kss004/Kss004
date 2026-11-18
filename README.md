# Kumar Shashwat

**AI Engineer: agent systems, LLM infrastructure, evals**

I build the layer between language models and real systems: tool-calling agents, MCP infrastructure, structured outputs, voice agents, and the evals and guardrails that keep them trustworthy in production.

Delhi, India · open to relocation · [kss04.me](https://kss04.me) · [LinkedIn](https://www.linkedin.com/in/kumar-shashwat-sandilya-b75332218/)

---

### Selected work

| Project | What it is | Engineering highlights |
| --- | --- | --- |
| **[Harbor](https://github.com/Kss004/KubernetesBasedMCPGateway)** | A team MCP gateway on Kubernetes ([live](https://app.169-58-78-14.sslip.io)) | Aggregates 4 upstream MCP servers behind one `/mcp` endpoint, with namespaced tools to avoid name collisions · upstream credentials stay inside the gateway · per-user API keys, role checks and a full audit log · NetworkPolicies and a written threat model · the same Helm charts on kind and k3s |
| **[Hotseat](https://github.com/Kss004/Hotseat)** | AI role-play coach for high-stakes meetings ([live](https://hotseat-lac.vercel.app)) | Multi-provider LLM router with timeouts and failover · Zod-validated structured outputs with a repair retry that feeds back the validation error · SSE streaming that never switches provider mid-reply · per-call latency and status logging · web content treated as untrusted input |
| **[Codex Usage Analyzer](https://github.com/Kss004/Codex-Usage-Analyzer)** | Finds where Codex saves engineering time in a codebase ([live](https://codex-usage-analyzer.vercel.app)) | Top 10% of ~10,000 at the OpenAI + AI Builders India Hackathon · 50 unit tests plus a property-based live LLM eval, which caught a model ordering bug that is now fixed deterministically |
| **[AEO Diagnostic](https://github.com/Kss004/AEO_Tool)** | Measures brand visibility across 5 LLMs | Parallel query × model fan-out with per-cell fallback, 429 backoff and timeouts · structured extraction with a deterministic fallback · tested in CI |

### Experience

- **HyrGPT, Generative AI:** multi-agent interview scheduling, async phone screening, and voice agents over SIP telephony (LiveKit, Plivo, Telnyx).
- **KPMG:** a meeting-intelligence bot that processed enterprise-scale meeting volume.
- **Leetlingo, Co-founder:** an AI interview-prep platform.

### How I build

- **Evals before features:** if a behaviour matters, it has a test case and a pass rate.
- **Treat every model output and every fetched document as untrusted input.**
- **Design for failure:** timeouts, fallbacks and budgets on every external call.
- **Trace everything:** a bug you can't find in a trace is a bug you'll ship twice.

### Stack

**Languages:** Python, TypeScript
**AI:** OpenAI, Anthropic, Gemini and Groq APIs · Vercel AI SDK · LangGraph · MCP · pgvector
**Backend:** FastAPI, asyncio, Pydantic · Next.js, Node · Postgres, Redis
**Infra:** Docker, Kubernetes, Helm, GCP, Vercel

**Education:** B.Tech, Computer & Communication Engineering, Manipal University Jaipur · BSc, Data Science, IIT Madras
