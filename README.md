# Mohammed Usmani

AI & ML Engineer, based in Bengaluru. I build agentic systems that run in
production — multi-agent orchestration, retrieval pipelines, realtime voice,
and the multi-tenant backends underneath them.

Most of what I work on is closed-source, so I write it up properly at
[mohammedusmani.me](https://www.mohammedusmani.me). There's an agent on the
homepage that will answer questions about any of it from a real corpus, and
cite where the answer came from.

---

### Things I've built

**[FS Preparation Agent](https://www.mohammedusmani.me/projects/fs-prep-agent)** — a financial statement engine, ~89K LOC of Python.
Its core is a Cross-Reference Graph linking every statement line to its note and
ledger account. Links are proposed by deterministic resolvers and only confirmed
when the numbers actually reconcile. Where an LLM helps, it just points at cells —
the pass/fail verdict comes from the same arithmetic either way, so it can't
hallucinate a passing reconciliation.

**[NetworkChains](https://www.mohammedusmani.me/projects/networkchains)** — the AI layer of a sales platform. [Live](https://www.networkchains.com).
An agentic copilot, a realtime call assistant, a relationship graph and
conversational image editing, over six purpose-scoped vector collections. The
part I'm happiest with: a seven-layer prompt stack that took worst-case input
from ~96K to ~2K tokens a turn, and getting speaker attribution out of the
transport instead of paying for a diarization model.

**[Luca](https://www.mohammedusmani.me/projects/luca)** — AI accounting platform for Indian CAs. [Live](https://askluca.in).
~199K LOC. Five LLM providers behind one registry with health-scored fallback,
pgvector RAG, 11 chat modes, and 10 statutory-compliance modules over a
106-table schema.

**[EyesAI](https://www.mohammedusmani.me/projects/eyesai)** — an Android agent that operates a phone end-to-end for blind users.
Planner → Executor → Verifier, 87% task completion. On-device vision at 88.2% /
151ms, and voice control that handles English, Hindi and Hinglish at 94%. The
Look screen deliberately draws no bounding boxes — overlays are useless to the
people it's for, so everything comes through speech and haptics.

The rest — [23 systems total](https://www.mohammedusmani.me/work) — is at mohammedusmani.me/work, with writeups that go into the engineering decisions.

---

### Open source

Grouped by what they actually are:

**Agent systems**
- **[Cortex](https://github.com/mohammed-usmani/Cortex)** — self-curating memory for a personal agent. Belief revision over an episodic log, so it updates and retires beliefs instead of just appending.
- **[GoalKeeper](https://github.com/mohammed-usmani/GoalKeeper)** — Taskwarrior-style urgency engine with an LLM layer bolted on top. The scoring is pure and fully tested; the model proposes and never silently mutates your data.
- **[APIAgent](https://github.com/mohammed-usmani/APIAgent)** — multi-agent API testing that parses a project and writes its own OpenAPI docs.

**Apps & tools**
- **[solidboard](https://github.com/mohammed-usmani/solidboard)** — Kanban on SolidJS with a hand-rolled drag-and-drop engine. Two runtime dependencies, total.
- **[gameweb](https://github.com/mohammed-usmani/gameweb)** — gaming portal with an ETL pipeline that ingests and normalises 3,000+ games.
- **[CityFix](https://github.com/Sumeet-2023/CityFix)** — civic issue reporting, UN SDG 11. I built the backend and schema. Took 3rd at GNEC International.

---

### How I tend to work

If there's one thing that shows up in everything above, it's that the model
proposes and deterministic code decides. Tie-outs are arithmetic. Figures an
agent states have to come from a tool call or they get flagged. Money that can't
be traced to a source gets withheld rather than shown. It's slower to build and
much harder to embarrass.

**Stack:** Python (FastAPI), TypeScript (Node, Express, NestJS), LangGraph, MCP,
OpenAI / Anthropic / Gemini, Deepgram and Voxtral for speech, Qdrant and pgvector
for retrieval, Celery and BullMQ, PostgreSQL / MongoDB / Redis, Docker on
GCP, AWS and DigitalOcean.

---

### Elsewhere

[Portfolio](https://www.mohammedusmani.me) ·
[Resume](https://www.mohammedusmani.me/resume) ·
[LinkedIn](https://linkedin.com/in/mohammed-usmani-927a96286) ·
[Devpost](https://devpost.com/mohammedusmani2005) ·
[Devfolio](https://devfolio.co/@Mohamammed) ·
[X](https://x.com/MohammedUs68507)

mohammedusmani2005@gmail.com · **Open to AI/ML and backend engineer roles at product-focused startups.**

---

Also: Top 17 nationally at Blend360's AI For Good (out of 5,000+ applicants),
and 3rd at GNEC International and at Codeathon.

---

![Mohammed Usmani — production output and contribution history](https://www.mohammedusmani.me/api/card)

<sub>Contribution counts include private repos — 2,116 of 2,799.</sub>
