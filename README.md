<h1 align="center">Hi, I'm Anish Kunda 👋</h1>

<p align="center">
  <b>Backend Engineer · Full Stack · AI Agents · AI&ML Engineer</b><br/>
  Correctness-first distributed systems and agents that stay inside their guardrails.
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/anishkunda/"><img src="https://img.shields.io/badge/LinkedIn-anishkunda-0A66C2?style=flat&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:anish03anish@gmail.com"><img src="https://img.shields.io/badge/Email-anish03anish%40gmail.com-D14836?style=flat&logo=gmail&logoColor=white" alt="Email"/></a>
  <a href="https://github.com/pulls?q=is%3Apr+author%3Aanishkun+-user%3Aanishkun"><img src="https://img.shields.io/badge/Open%20Source-PRs%20to%20PennyLane%20%C2%B7%20Weblate%20%C2%B7%20OpenAlgo-2ea44f?style=flat&logo=github" alt="Open source PRs"/></a>
  
</p>

---

### What I do

I build backend systems where the hard part is **getting it right under concurrency and failure** — ledgers that can't double-spend, queues that survive crashes, event relays with at-least-once delivery — and, more recently, **AI agents** that act through MCP servers behind a fail-closed permission layer.

- 🏢 **Software Engineering Intern @ Nishi Tech Solutions** (Nov 2025 – Aug 2026) — built an AI phone-ordering agent for restaurant clients (FastAPI WebSockets, Twilio, Deepgram, ElevenLabs) with a LangGraph state machine and Gemini tool-calling; configured Flask and Django applications and built and tested their REST APIs.
- 🏆 **1st place, AI Autonomous Hackathon 2025, VR Siddhartha** (Feb 2025) — led a 4-member team to build MindMate AI, a 3D chess platform, in 24 hours: Classic, Quantum, and Ghost modes, each with a custom-trained AI model, plus Stockfish-based analysis; out of 100+ teams.
- 🎓 B.Tech CSE (AI & ML), Mohan Babu University — 2022 – 2026.

---

### Featured projects

| Project | What it proves | Stack |
|---|---|---|
| **[ReLife](https://github.com/anishkun/ReLife)** — self-improving personal agent | ACT-R-inspired memory in SQLite (relevance rises with use, decays over time) with two-stage recall over SQLite FTS5 and optional vector search; deterministic "sleep" pass that decays, dedupes, and mines repeated actions into reusable workflows; opt-in LLM "dream" critic that reversibly prunes memory; a decompose → delegate → resume build orchestrator whose ledger survives session-limit resets. 580+ deterministic tests, no live model calls. | Python · Claude Agent SDK · MCP · SQLite |
| **[ApexPay](https://github.com/anishkun/ApexPay)** — event-driven financial ledger | Lexicographic lock ordering + JPA `PESSIMISTIC_WRITE` to make deadlocks and double-spends impossible; Transactional Outbox + Idempotency facade inside one ACID boundary; outbox relay with publisher confirms, `FOR UPDATE SKIP LOCKED`, bounded backoff, and dual DLQs; Flyway-owned schema validated by Hibernate; Testcontainers ITs prove 24 concurrent retries → exactly one debit. ECS structured logs with correlation IDs, OpenTelemetry tracing, Spring Security. | Java 21 · Spring Boot 3 · PostgreSQL · RabbitMQ · Docker |
| **[AI Phone Ordering System](https://github.com/anishkun/AI-Phone-Ordering-System)** — real-time voice agent | Bidirectional Twilio media streams → Deepgram STT → LangGraph state machine → ElevenLabs TTS at sub-500 ms round-trip; the LLM never touches prices or inventory — strict tool-calling against a deterministic backend produces exact POS payloads; human hand-off on frustration. | Python · FastAPI · WebSockets · LangGraph |
| **[Persistent Disk-Backed Message Broker](https://github.com/anishkun/PersistentDiskBackedMessageBroker)** — durable FIFO queue from scratch | Append-only length-prefixed log with zero-copy `FileChannel`/`ByteBuffer` I/O, crash-safe partial-record handling, logical offsets, thread-safe enqueue/dequeue, and a bundled throughput benchmark. Zero dependencies. | Java · NIO |
| **[TextPrivate](https://github.com/anishkun/TextPrivate)** — encrypted Android messenger | Encrypted sessions with a disguise-mode UI; MVVM, Hilt DI, Material 3. | Kotlin · Jetpack Compose |

---

### Open-source contributions

I read other people's code as carefully as my own. 5 PRs merged upstream so far:

- **[Weblate](https://github.com/WeblateOrg/weblate/pulls?q=is%3Apr+author%3Aanishkun)** (3 merged) — glossary mislabelled unflagged terms as untranslatable; outline-button icons ignored text colour; the editor now remembers whether string details are expanded.
- **[OpenAlgo](https://github.com/marketcalls/openalgo/pulls?q=is%3Apr+author%3Aanishkun)** (2 merged) — normalised Upstox tick sizes from paise to rupees; removed the Close button from positions already squared off. More fixes open for review.
- **[PennyLane](https://github.com/PennyLaneAI/pennylane/pulls?q=is%3Apr+author%3Aanishkun)** (open for review) — gate-commutation and circuit-compilation fixes, including [`is_commuting`](https://github.com/PennyLaneAI/pennylane/pull/10175) treating partially-overlapping SWAP-like ops as commuting.

→ [All PRs](https://github.com/pulls?q=is%3Apr+author%3Aanishkun+-user%3Aanishkun)

---



<p>
  <img src="https://skillicons.dev/icons?i=java,spring,python,fastapi,postgres,mysql,redis,sqlite,rabbitmq,kafka,docker,git,kotlin,linux,idea,postman" height="40" alt="tools"/>
</p>



---


