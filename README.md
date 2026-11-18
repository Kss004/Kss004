# Shashwat
 
**AI Engineer: agent systems, LLM infrastructure, evals**
 
I build the layer between language models and real systems: tool-calling agents, MCP infrastructure, structured outputs, voice agents, and the evals and guardrails that keep them trustworthy in production.
 
Delhi, India · [kss04.me](https://kss04.me) · [LinkedIn](https://www.linkedin.com/in/kumar-shashwat-sandilya-b75332218/)
 
---
 
### Selected work
 
- **[Harbor](https://github.com/Kss004/KubernetesBasedMCPGateway)** ([live](https://app.169-58-78-14.sslip.io)): one `/mcp` endpoint over 4 upstream servers · credentials never leave the gateway · per-user keys, roles, audit log · threat model and NetworkPolicies
- **[Hotseat](https://github.com/Kss004/Hotseat)** ([live](https://hotseat-lac.vercel.app)): multi-provider router with failover · Zod-validated outputs with repair retry · SSE streaming that never switches provider mid-reply
- **[Codex Usage Analyzer](https://github.com/Kss004/Codex-Usage-Analyzer)** ([live](https://codex-usage-analyzer.vercel.app)): top 10% of ~10,000 at the OpenAI + AI Builders India Hackathon · live LLM eval that caught a model ordering bug
- **[AEO Diagnostic](https://github.com/Kss004/AEO_Tool)**: parallel fan-out across 5 LLMs with fallback and 429 backoff · structured extraction · tested in CI
### How I build
 
- **Evals before features:** if a behaviour matters, it has a test case and a pass rate.
- **Treat every model output and every fetched document as untrusted input.**
- **Design for failure:** timeouts, fallbacks and budgets on every external call.
- **Trace everything:** a bug you can't find in a trace is a bug you'll ship twice.
### Stack
 
- **Languages:** Python, TypeScript
- **AI:** OpenAI, Anthropic, Gemini and Groq APIs · Vercel AI SDK · LangGraph · MCP · pgvector
- **Backend:** FastAPI, asyncio, Pydantic · Next.js, Node · Postgres, Redis
- **Infra:** Docker, Kubernetes, Helm, GCP, Vercel
 
