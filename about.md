---
layout: page
title: Artemii Maevskii
permalink: /about/
---

I am an infrastructure engineer (DevOps / SRE / AI Infrastructure) with **8 years of production experience**. I went from system administrator to core administrator single-handedly carrying a company's entire IT — development, deployment, operations, security. A separate track is AI infrastructure research (**embryo → Mimic**) and protocol-level open source.

Location: Moscow, Russia · Remote worldwide.

## Career path

### danila-master.ru — Core Administrator (April 2023 – July 2026, remote)

The company's entire IT infrastructure in one pair of hands, assembled and deployed personally: domain, virtualization, networks, monitoring, CI/CD, corporate services, mail, internal product development, documentation and handover of processes to support.

Key implementations:

- **Domain infrastructure from scratch.** Active Directory on Windows Server 2022 (DNS, GPO, replication) across all of Russia with timezone debugging; SSO on Keycloak; MeshCentral in LXC for fleet management — agents, scheduled load and service-state metrics, reporting to a corporate bot.
- **Centralized software distribution via AD.** MSI installation via GPO from SYSVOL, dynamic resources in apps.json, content updates via actions on a self-hosted runner; versions verified at machine restart outside working hours in regional windows; support only observes the result via a runbook.
- **Deployment pipeline for the website (Yii2) and related services.** Self-hosted GitLab + runner, dev/test/prod environments, tag-based releases, cascading deploy with nodes drained from traffic, backward-compatible DB migrations, smoke tests, rollback as a deploy of the previous tag.
- **Full-cycle corporate products (dev + deploy + operations, solo):**
  - [hradmin](https://github.com/Mayveskii/hradmin) — HR recruiting analytics on top of Bitrix24: ETL into PostgreSQL, Laravel 12 + Filament, reports/dashboards, sync drift control.
  - [b24_bot](https://github.com/Mayveskii/b24_bot) — support and facility-management bot in Bitrix24 (Node.js).
  - [b24doc_runner](https://github.com/Mayveskii/b24doc_runner) — Bitrix24 Disk → self-hosted NAS file migration with an SQLite audit registry.
  - [stacktrace](https://github.com/Mayveskii/stacktrace) — self-hosted DMS with an AI assistant: RAG over documents (Qdrant + local embeddings + LLM gateway), OCR pipeline, Collabora Online via WOPI.
  - [proxdash](https://github.com/Mayveskii/proxdash) — Proxmox infrastructure dashboard (Flask).
  - [rfo_poligon](https://github.com/Mayveskii/rfo_poligon) — CCTV panel on top of Flussonic.
  - [nextcloud](https://github.com/Mayveskii/nextcloud) — production file cloud in Docker (MariaDB + Redis), with a documented upgrade-incident post-mortem.
- **GitOps hypervisor management ([Nemesis](https://github.com/Mayveskii/Nemesis)).** Production Proxmox VE under a plan → approve → apply → verify regime: snapshots before changes, preflight, runbooks, no direct mutations, guardrails for the AI agent.
- **Ansible fleet automation ([ansible-danila](https://github.com/Mayveskii/ansible-danila)).** ~20 hosts: HTML monitoring reports, Zabbix agent diagnostics, fail2ban hardening, read-only incident collection, webhook triggers from a bot.
- **Mail infrastructure.** mailcow in production, Bitrix24 portal, Asterisk.

Client infrastructure project work (NDA):

- **MariaDB/PBS (electronic metering provider).** Fixed degradation of a ~226 GB production database during 2-hour vzdump backups: I/O and network diagnostics, designed a binlog replica on a separate LXC, moved backups to the replica, qemu-guest-agent with fsfreeze hook, data access by mounting PBS archives without full restore.
- **Redis for an HR bot of a medical branch (large organization).** Cascading failure of a shared instance (OOM + allkeys-lru: lost sessions, queues, reconnect storm) → refactoring: separated cache/sessions/queues/locks into dedicated instances, per-purpose eviction policies, AOF for queues, Sentinel, connection pooling, metrics in Zabbix. Incidents stopped.

### 2018 – 2023 · System Administrator → Senior System Administrator, InfoSec (NDA)

Five continuous years: from server administration at an international company (Thailand) to a senior role in the information security department of a large international tour operator. Employer names under NDA.

- 99.9% uptime of critical infrastructure with 24/7 requirements.
- Networks: MikroTik (routing, firewall), VPN (Wireguard, OpenVPN, IPSec), DNS.
- Network node monitoring and traffic analysis: port mirroring → tcpdump + Python parser → metrics in Zabbix over a Wireguard tunnel; real-time anomaly detection.
- Secure corporate messenger with E2E encryption (Matrix Synapse) and its own TURN server — high availability, fault tolerance.
- Full-cycle Android app for the security service (Java/Kotlin, API, secure storage) — from design to release.
- OCR document recognition system (OpenCV, TensorFlow, Tesseract) — 1500+ documents a day.
- HR Telegram bots (Python, PostgreSQL, Docker) — 10,000+ tickets a month.
- Foundation era: Linux/Windows servers, PostgreSQL/MariaDB, Bash/Python, Zabbix, Docker, user and owner infrastructure support.

## AI infrastructure research

- **[embryo](https://github.com/Mayveskii/embryo) (binary-mesh) — flagship research.** "Deterministic intelligence": autonomous code analysis, vulnerability hunting and fix generation without an LLM call on mesh coverage. Go monolith + C core (CGO, mmap, binary runtime with 28 opcodes), MCP server with 57 tools, semantic mesh on int8-quantized embeddings (298K slots, <1 ms answers at sim ≥ 0.85), 5-signal hybrid RAG (Qdrant, 180K points), vulnerability hunting in real protocols (gonka, go-ethereum), commit survival analysis via git blame, honest recording of negative results.
- **[Mimic](https://github.com/Mayveskii/Mimic) — the line continues.** MCP server with a C-core execution engine, orchestrator, 48+ tools.
- **[teeth_master](https://github.com/Mayveskii/teeth_master)** — evidence-based knowledge base (dentistry, manual therapy) in an agent-ready format: domain skills, research SOPs, source discipline.

## Open source (protocol level)

64 PRs in the first year of the public account (account created 2025; previous work under NDA), 10 issues including security class. Full list: [Contributions]({{ '/contributions/' | relative_url }}).

- **ethereum/go-ethereum** — PR [#34039](https://github.com/ethereum/go-ethereum/pull/34039) (merged): txLookupLock mutex leak in reorg(); error-handling series across core/txpool/filtermaps/snapshot (#34095–#34099, #34665, #34737); issues #34038, #34944.
- **gonka-ai/gonka** (decentralized AI, Go/Cosmos SDK) — ~25 PRs: #1071 (merged) error propagation across inference/validation/pricing; BLS/DKG consensus security fixes (#851, #852; issues #848, #849); semantic cache (#859, #878); overflow guards, rate limits, graceful shutdown.
- **gonkalabs/opengnk** — PRs #1, #2 (merged): inference quality metrics middleware, L1 semantic cache.

## Full technology stack

**Infrastructure:** Proxmox VE/PBS, bare-metal, datacenter, Hetzner/VPS/VDS, LXC, KVM, Windows Server 2016–2025, Active Directory, GPO, Keycloak, MeshCentral, PowerShell.

**Automation / CI-CD:** Ansible (playbooks, roles, vault), GitLab CI/CD (self-hosted runner), GitHub Actions, Git, IaC, GitOps.

**Monitoring:** Zabbix (500+ hosts), Grafana, custom metrics, Proxmox API.

**Networking & Security:** MikroTik, Wireguard, OpenVPN, IPSec, DNS, NAT, firewall, OWASP, Wireshark/tcpdump, fail2ban.

**Containers:** Docker, Docker Compose, Registry; Kubernetes — ready for production.

**Databases:** PostgreSQL (replication, backup), MariaDB, MySQL, Redis (HA, Sentinel), SQLite, Qdrant, pgvector, SQLAlchemy, Alembic.

**AI / ML:** RAG, LLM inference (vLLM), MCP servers/agents, embeddings (sentence-transformers, int8 quantization), OpenCV, TensorFlow, Tesseract OCR.

**Development:** Python, Go, PHP (Laravel 12, Filament, Yii2), JavaScript/Node.js, TypeScript/Next.js, Java, Kotlin, C, Bash, REST API, Nginx, Apache.

**Enterprise:** Bitrix24 (REST API, bots, webhooks), mailcow, Asterisk, Matrix Synapse, TURN, Nextcloud, Collabora Online (WOPI), Flussonic, PERCo-WEB, Telegram Bot API.

**Practices:** runbooks, post-mortems, controlled failure tests, rollback plans, handing systems over to internal teams.

## Education and languages

- RANEPA (Moscow), Economics and Accounting, secondary vocational education, 2014.
- Additionally: State and Municipal Administration.
- Russian — native; English — B2 (technical documentation, OSS correspondence).

## Contacts

- Telegram: [@fullom3m3](https://t.me/fullom3m3) (preferred)
- Email: [maevskiiartemii@gmail.com](mailto:maevskiiartemii@gmail.com)
- GitHub: [Mayveskii](https://github.com/Mayveskii)
- Blog: [mayveskii.github.io/maevskii.blog](https://mayveskii.github.io/maevskii.blog/)
- Location: Moscow, Russia · Remote worldwide
