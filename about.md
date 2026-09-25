---
layout: page
title: Artemii Maevskii
permalink: /about/
---

I am an infrastructure engineer (DevOps / Senior SysAdmin) with **6 years of production experience**. I went from system administrator to DevOps engineer running a company's entire IT as code — development, deployment, operations, security. A separate track is AI infrastructure research (**embryo → Mimic**) and protocol-level open source.

Location: Moscow, Russia · Remote worldwide.

## Career path

### Core DevOps — danila-master.ru, product company (2023 – 2026, remote)

The company's entire IT infrastructure in one pair of hands, assembled and deployed personally: 15+ Proxmox VE hypervisors, 500+ VMs, domain, virtualization, networks, monitoring, CI/CD, corporate services, mail, internal product development, documentation and handover of processes to support. Everything is managed as code — every hypervisor, every VM, every service lives in git and changes only through it.

Key implementations:

- **Centralized monitoring of 500+ hosts (15+ hypervisors).** Zabbix, VictoriaMetrics, Grafana, Alertmanager, alerts to Telegram, logs via Vector.
- **ETL contour.** Airflow, ClickHouse, VictoriaMetrics, Prometheus, Grafana, full ELK — Filebeat, Logstash, Elasticsearch, Kibana.
- **Kubernetes/OpenShift.** Deploy and update applications via Helm and manifests, pod and service diagnostics, monitoring on Prometheus.
- **Proxy contour for the whole domain infrastructure.** NGINX, Nginx Proxy Manager, HAProxy balancing, wildcard TLS (issuance, rotation, termination).

- **Domain infrastructure from scratch.** Active Directory on Windows Server 2022 (DNS, GPO, replication) across all of Russia with timezone debugging; SSO on Keycloak; MeshCentral in LXC for fleet management — agents, scheduled load and service-state metrics, reporting to a corporate bot.
- **Centralized software distribution via AD.** MSI installation via GPO from SYSVOL, dynamic resources in apps.json, content updates via actions on a self-hosted runner; versions verified at machine restart outside working hours in regional windows; support only observes the result via a runbook.
- **Deployment pipeline for the website (Yii2) and related services.** Self-hosted GitLab + runner, dev/uat/prod environments, tag-based releases, cascading deploy with nodes drained from traffic, backward-compatible DB migrations, smoke tests, rollback as a deploy of the previous tag. No manual deployments.
- **Full-cycle corporate products (dev + deploy + operations, solo):**
  - [hradmin](https://github.com/Mayveskii/hradmin) — HR analytics admin panel on top of Bitrix24: Laravel 12 + Filament, ETL into PostgreSQL.
  - [b24_bot](https://github.com/Mayveskii/b24_bot) — support and procurement-department bots in Bitrix24 (Node.js).
  - [b24doc_runner](https://github.com/Mayveskii/b24doc_runner) — Bitrix24 Disk → self-hosted NAS file migration with an SQLite audit registry.
  - [stacktrace](https://github.com/Mayveskii/stacktrace) — self-hosted DMS with an AI assistant: RAG over documents (Qdrant + local embeddings + LLM gateway), OCR pipeline, Collabora Online via WOPI.
  - [proxdash](https://github.com/Mayveskii/proxdash) — Proxmox infrastructure dashboard (Flask).
  - [rfo_poligon](https://github.com/Mayveskii/rfo_poligon) — CCTV panel on top of Flussonic.
  - [nextcloud](https://github.com/Mayveskii/nextcloud) — production file cloud in Docker (MariaDB + Redis), with a documented upgrade-incident post-mortem.
  - [docpool](https://github.com/Mayveskii/docpool) — document management with a RAG chat in Go: PostgreSQL + pgvector, SSE streaming answers, answer verification against sources, protected PDF copies (AES-256-GCM), multi-user.
  - [ai-reviewer](https://github.com/Mayveskii/ai-reviewer) — Go CLI that reviews pull requests with an orchestration of AI personas instead of one prompt.
- **GitOps hypervisor management ([Nemesis](https://github.com/Mayveskii/Nemesis)).** Production Proxmox VE under a plan → approve → apply → verify regime: snapshots before changes, preflight, runbooks, no direct mutations, guardrails for the AI agent.
- **Ansible fleet automation ([ansible-danila](https://github.com/Mayveskii/ansible-danila)).** 15+ hypervisors and hundreds of VMs: HTML monitoring reports, Zabbix agent diagnostics and mass config updates (read-only/safe playbooks), fail2ban hardening, SSH key distribution, hypervisor audits, read-only incident collection, webhook triggers from a bot.
- **Mail infrastructure.** mailcow in production, Bitrix24 portal, Asterisk.

Client infrastructure project work (NDA):

- **Client MariaDB replica.** The client's MariaDB degraded for 2 hours during every backup. Designed a binlog replica on a separate LXC and moved backups to it — the database stopped going down entirely.
- **Client Redis with Sentinel.** Redis failed cascading (OOM took down sessions and queues). Split cache, sessions, queues and locks into dedicated instances, configured eviction policies, AOF and Sentinel — incidents stopped.

### 2019 – 2023 · System Administrator → Senior System Administrator, InfoSec (NDA)

Four continuous years: from server administration at an international company (Thailand) to a senior role in the information security department of a large international tour operator. Employer names under NDA.

- Networks: MikroTik (routing, firewall), VPN (Wireguard, OpenVPN, IPSec), DNS.
- Network node monitoring and traffic analysis: port mirroring → tcpdump + Python parser → metrics in Zabbix over a Wireguard tunnel; real-time anomaly detection.
- Secure corporate messenger with E2E encryption (Matrix Synapse) and its own TURN server — high availability, fault tolerance.
- Full-cycle Android app for the security service (Java/Kotlin, API, secure storage) — from design to release.
- OCR document recognition system (OpenCV, TensorFlow, Tesseract) — 1500+ documents a day.
- HR Telegram bots (Python, PostgreSQL, Docker) — 10,000+ tickets a month.
- Foundation era: Linux/Windows servers, PostgreSQL/MariaDB, Bash/Python, Zabbix, Docker, user and owner infrastructure support.

## AI infrastructure research

- **[embryo](https://github.com/Mayveskii/embryo) (binary-mesh) — flagship research.** Autonomous code analysis and fix generation: successful solutions are distilled into proven executable patterns and reused deterministically, with no repeated inference — knowledge compounds instead of burning in the session context. Proven in practice: the system found and patched defects in real protocols (go-ethereum, gonka, kueue); these findings became the PRs listed below.
- **[Mimic](https://github.com/Mayveskii/Mimic) — the line continues.** Deterministic execution layer for AI agents: every operation is validated before it runs, cost is measured, failures roll back — the agent stops guessing arguments and burning tokens on retries.
- **[teeth_master](https://github.com/Mayveskii/teeth_master)** — evidence-based knowledge base (dentistry, manual therapy) in an agent-ready format: domain skills, research SOPs, source discipline.

## Open source (protocol level)

Merged fixes in CNCF and core infrastructure protocols, found with my own code-analysis system. Full list: [Contributions]({{ '/contributions/' | relative_url }}).

- **kubernetes-sigs/kueue** (CNCF, SIG-Scheduling) — trust-boundary bug class in the job framework: foreign Workloads deleted via non-controller ownerReferences: [issue #13572](https://github.com/kubernetes-sigs/kueue/issues/13572), [PR #13573](https://github.com/kubernetes-sigs/kueue/pull/13573) (merged, cherry-picked into release branches).
- **ethereum/go-ethereum** — PR [#34039](https://github.com/ethereum/go-ethereum/pull/34039) (merged): txLookupLock mutex leak in reorg(); a series of error-handling fixes.
- **gonka-ai/gonka** (decentralized AI, Go/Cosmos SDK) — a series of PRs on BLS/DKG consensus and error propagation; [#1071](https://github.com/gonka-ai/gonka/pull/1071) merged.

## Full technology stack

**Infrastructure:** Kubernetes/OpenShift, Docker, Ansible, GitLab CI, Helm, Prometheus, Grafana, Zabbix, VictoriaMetrics, ClickHouse, ELK (Filebeat, Logstash, Elasticsearch, Kibana), Vector, Airflow, Linux, Proxmox VE/PBS, Nginx, HAProxy, PostgreSQL, MariaDB, Redis, Wireguard, Active Directory.

**Development:** Python, Go, PHP, Node.js, Java, Kotlin, Rust, C, Bash.

## Education and languages

- RANEPA (Moscow), Economics and Accounting, secondary vocational education, 2014.
- Additionally: State and Municipal Administration.
- Russian — native; English — B2 (technical documentation, OSS correspondence).

## Contacts

- Telegram: [@fullom3m3](https://t.me/fullom3m3) (preferred)
- Email: [maevskiiartemii@gmail.com](mailto:maevskiiartemii@gmail.com)
- Phone: +7 (930) 120-91-69
- GitHub: [Mayveskii](https://github.com/Mayveskii)
- Blog: [mayveskii.github.io/maevskii.blog](https://mayveskii.github.io/maevskii.blog/)
- Location: Moscow, Russia · Remote worldwide
