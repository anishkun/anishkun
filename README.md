<h1 align="center">Hi, I'm Anish Kunda 👋</h1>

<p align="center">
  <b>Backend Engineer · Java / Spring Boot · AI Agents & MCP</b><br/>
  Correctness-first distributed systems and agents that stay inside their guardrails.
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/anishkunda/"><img src="https://img.shields.io/badge/LinkedIn-anishkunda-0A66C2?style=flat&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:anish03anish@gmail.com"><img src="https://img.shields.io/badge/Email-anish03anish%40gmail.com-D14836?style=flat&logo=gmail&logoColor=white" alt="Email"/></a>
  <a href="https://github.com/pulls?q=is%3Apr+author%3Aanishkun+-user%3Aanishkun"><img src="https://img.shields.io/badge/Open%20Source-PRs%20to%20PennyLane%20%C2%B7%20Weblate%20%C2%B7%20OpenAlgo-2ea44f?style=flat&logo=github" alt="Open source PRs"/></a>
  <img src="https://img.shields.io/badge/U.S.%20Citizen-No%20sponsorship%20needed-555?style=flat" alt="US Citizen"/>
</p>

---

### What I do

I build backend systems where the hard part is **getting it right under concurrency and failure** — ledgers that can't double-spend, queues that survive crashes, event relays that never lose a message — and, more recently, **AI agents** that act through MCP servers behind a fail-closed permission layer.

- 🏢 **Software Engineering Intern @ NishiTech Solutions** (Aug 2025 – Feb 2026) — Java/Spring Boot backend for a payment-processing module; wrote the JUnit + Mockito suites that took coverage to **85%** on a CI/CD pipeline.
- 🏆 **1st place, VR Siddhartha AI Hackathon** (2025) — led a 4-person team building a Stockfish-backed evaluation pipeline with real-time model inference, out of 100+ teams.
- 🎓 B.Tech CSE (AI & ML), Mohan Babu University — 2022 – 2026.

---

### Featured projects

| Project | What it proves | Stack |
|---|---|---|
| **[ReLife](https://github.com/anishkun/ReLife)** — self-improving personal agent | ACT-R-inspired memory in SQLite (relevance rises with use, decays over time) with a two-stage FTS5 + vector recall pipeline; deterministic "sleep" pass that decays, dedupes, and mines repeated actions into reusable workflows; opt-in LLM "dream" critic that reversibly prunes memory; a decompose → delegate → resume build orchestrator whose ledger survives session-limit resets. 80+ deterministic tests, no live model calls. | Python · Claude Agent SDK · MCP · SQLite |
| **[ApexPay](https://github.com/anishkun/ApexPay)** — event-driven financial ledger | Lexicographic lock ordering + JPA `PESSIMISTIC_WRITE` to make deadlocks and double-spends impossible; Transactional Outbox + Idempotency facade inside one ACID boundary; outbox relay with publisher confirms, `FOR UPDATE SKIP LOCKED`, bounded backoff, and dual DLQs; Flyway-owned schema validated by Hibernate; Testcontainers ITs prove 24 concurrent retries → exactly one debit. ECS structured logs with correlation IDs, OpenTelemetry tracing, Spring Security. | Java 21 · Spring Boot 3 · PostgreSQL · RabbitMQ · Docker |
| **[AI Phone Ordering System](https://github.com/anishkun/AI-Phone-Ordering-System)** — real-time voice agent | Bidirectional Twilio media streams → Deepgram STT → LangGraph state machine → ElevenLabs TTS at sub-500 ms round-trip; the LLM never touches prices or inventory — strict tool-calling against a deterministic backend produces exact POS payloads; human hand-off on frustration. | Python · FastAPI · WebSockets · LangGraph |
| **[Agent Orchestrator Platform](https://github.com/anishkun/AgentOrchestratorPlatform)** — multi-tier agent runtime | Loom virtual-thread control plane (R2DBC + Lettuce, no pinning), Kafka for state transitions vs. Redis Streams for high-throughput logs, Redis-checkpointed LangGraph workers with Kafka claim-and-commit, and Firecracker microVM sandboxes with HITL pause/snapshot. | Java 21 · Spring Boot · Kafka · Redis · Python · LangGraph |
| **[Persistent Disk-Backed Message Broker](https://github.com/anishkun/PersistentDiskBackedMessageBroker)** — durable FIFO queue from scratch | Append-only length-prefixed log with zero-copy `FileChannel`/`ByteBuffer` I/O, crash-safe partial-record handling, logical offsets, thread-safe enqueue/dequeue, and a bundled throughput benchmark. Zero dependencies. | Java · NIO |
| **[TextPrivate](https://github.com/anishkun/TextPrivate)** — encrypted Android messenger | Encrypted sessions with a disguise-mode UI; MVVM, Hilt DI, Material 3. | Kotlin · Jetpack Compose |

---

### Open-source contributions

I read other people's code as carefully as my own. Recent fixes upstream:

- **[PennyLane](https://github.com/PennyLaneAI/pennylane/pull/10175)** — `is_commuting` wrongly treated partially-overlapping SWAP-like ops as commuting.
- **[Weblate](https://github.com/WeblateOrg/weblate/pulls?q=is%3Apr+author%3Aanishkun)** — glossary mislabelled unflagged terms as untranslatable; outline-button icons ignored text colour.
- **[OpenAlgo](https://github.com/marketcalls/openalgo/pulls?q=is%3Apr+author%3Aanishkun)** — merged fix normalising Upstox tick sizes from paise to rupees; plus fixes for smart-order exit reporting, position-book "Close" state, asset mtime cache invalidation, token-based Telegram command parsing, and NaN containment in rolling indicators.

→ [All PRs](https://github.com/pulls?q=is%3Apr+author%3Aanishkun+-user%3Aanishkun)

---

### Toolbox

<p>
  <img src="https://skillicons.dev/icons?i=java,spring,python,fastapi,postgres,mysql,redis,sqlite,rabbitmq,kafka,docker,git,kotlin,linux,idea,postman" height="40" alt="tools"/>
</p>

**Languages:** Java, Python, Kotlin &nbsp;·&nbsp; **Frameworks:** Spring Boot, FastAPI, LangGraph, Claude Agent SDK &nbsp;·&nbsp; **Data:** PostgreSQL, MySQL, Redis, SQLite &nbsp;·&nbsp; **Messaging:** RabbitMQ, Kafka &nbsp;·&nbsp; **Testing:** JUnit 5, Mockito, Testcontainers, Flyway &nbsp;·&nbsp; **Core:** DSA, LLD, concurrency, Java NIO / file I/O, REST APIs, AI agents, MCP servers

---

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=anishkun&show_icons=true&hide_border=true&theme=default&include_all_commits=true&count_private=true" height="160" alt="GitHub stats"/>
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=anishkun&layout=compact&hide_border=true&hide=jupyter%20notebook,html" height="160" alt="Top languages"/>
</p>

<p align="center">
  📫 <a href="mailto:anish03anish@gmail.com">anish03anish@gmail.com</a> &nbsp;·&nbsp; <a href="https://www.linkedin.com/in/anishkunda/">LinkedIn</a>
</p>
