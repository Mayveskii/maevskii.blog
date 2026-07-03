---
layout: home
title: Home
---

<div class="hero">
  <div class="hero-content">
    <h1>Artemii Maevskii</h1>
    <div class="hero-subtitle">Senior DevOps / SRE / AI Infrastructure Engineer</div>
    <div class="hero-tagline">
      Infrastructure engineer with 6.5+ years of production experience in automation, enterprise security, networking, virtualization and AI infrastructure.
    </div>
    <div class="hero-links">
      <a href="{{ site.baseurl }}/organizations/">Organizations</a>
      <a href="https://github.com/Mayveskii">GitHub</a>
      <a href="https://t.me/fullom3m3">Telegram</a>
    </div>
  </div>
</div>

<div class="panel">
  <h2>Summary</h2>
  <p>I progressed from Linux/Windows system administrator to DevOps/Senior Sysadmin responsible for 500+ hosts, NDA-critical infrastructure, and internal HR/InfoSec products.</p>
  <p>I am an active open-source contributor to L1/L2 protocols and AI infrastructure: security fixes, error propagation, consensus bugs, semantic cache, LLM inference hardening in <strong>ethereum/go-ethereum</strong>, <strong>gonka-ai/gonka</strong> and <strong>gonkalabs/opengnk</strong>. In recent years I have been building my own AI/ML projects: RAG, MCP servers, decentralized AI.</p>
  <p>Public GitHub is a new account (2025) because previous work was under strict NDA.</p>
</div>

## Key Skills

<div class="panel">
  <p><strong>Infrastructure & Virtualization:</strong> Proxmox VE (clusters, API, backups), bare-metal, datacenter management, Hetzner/VPS/VDS, Windows Server (2016/2019/2022/2025), Active Directory, GPO, PowerShell</p>
  <p><strong>Automation & CI/CD:</strong> Ansible (playbooks, roles, vault), GitLab CI/CD, GitHub Actions, Bash, Python, Git, Infrastructure as Code</p>
  <p><strong>Monitoring & Observability:</strong> Zabbix (500+ hosts, custom metrics), Grafana dashboards, Proxmox API integrations, custom metrics</p>
  <p><strong>Containers:</strong> Docker, Docker Compose, Docker Registry; Kubernetes — familiar with the tool and ready for production use (no large-scale cluster experience yet)</p>
  <p><strong>Cloud & CDN:</strong> Cloud providers (instance deployment, 24/7 availability), CDN, VPS/VDS</p>
  <p><strong>Networking & Security:</strong> MikroTik (routing, VPN, firewall), Wireguard/OpenVPN/IPSec, DNS, NAT, proxy, firewall, OWASP, traffic analysis, OSI model</p>
  <p><strong>Databases:</strong> PostgreSQL (administration, replication, backup), MariaDB, MySQL, Redis, SQL, SQLAlchemy, Alembic</p>
  <p><strong>AI / ML Infrastructure:</strong> Python, Go, RAG (pgvector), LLM inference (vLLM), MCP/agents, OpenCV, TensorFlow, Tesseract OCR</p>
  <p><strong>Development & Web:</strong> PHP/Laravel, JavaScript, Node.js, React, Vue.js, Java, Kotlin, REST API, Nginx, Apache</p>
  <p><strong>Communications & Enterprise:</strong> Asterisk, Matrix Synapse, TURN server, Bitrix Portal, PERCo-WEB, Telegram Bot API, satellite communications</p>
</div>

## Experience

### TemplateState — DevOps Engineer / Senior System Administrator
*April 2023 – Present · Remote*

**Stack:** Proxmox VE, Ansible, GitLab CI/CD, Zabbix, Grafana, Python, Docker, PostgreSQL, Linux, Windows Server, Active Directory, Bitrix, mail services

- Grew into a DevOps/Senior Sysadmin role, fully owning infrastructure and deployment of corporate services.
- Administer Proxmox VE virtualization clusters: API, backups, migrations, resources.
- Automated infrastructure with Ansible (playbooks, roles, vault) + GitLab CI/CD, making deployments reproducible.
- Implemented Infrastructure as Code practices: Git repositories + Ansible for configuration management.
- Develop and maintain GitLab CI/CD pipelines for deployment automation.
- Built and maintain production Active Directory from scratch: Root DC on Windows Server 2022, DNS, GPO, replication.
- Implemented 3-2-1 backup strategy on PBS cluster for critical systems.
- Run monitoring for 500+ hosts in Zabbix + Grafana dashboards; integrated Proxmox API for real-time metrics across 100+ servers.
- Administer corporate systems: Bitrix Portal, mail infrastructure.
- Designed and deployed an internal HR system: full-cycle from code to production and support (PHP/Laravel/JS + PostgreSQL).
- Projects: full AD deployment from scratch, legacy systems migration to Proxmox virtualization, GitLab + Ansible IaC workflow integration.

### TezTour [NDA] — Senior System Administrator (Information Security Dept.)
*January 2020 – February 2023 · Office / remote · Critical infrastructure*

**Stack:** Linux, MikroTik, VPN (Wireguard, OpenVPN, IPSec), Python, PostgreSQL, Docker, Zabbix, Matrix, Wireshark, Asterisk, TensorFlow, OpenCV, Telegram Bot API

- Ensured 24/7 availability and security of critical infrastructure for a large international tour operator.
- Administered network infrastructure: MikroTik routing, VPN, firewall, DNS.
- Ensured information security of critical systems.
- Developed internal automation tools for the InfoSec department using Python + PostgreSQL.
- Monitored network traffic and identified security incidents.
- Configured Zabbix monitoring on MikroTik to control network health and analyze traffic.
- Ensured 99.9% uptime of critical infrastructure.

**Key projects:**

- **Network node monitoring and traffic analysis system (2022)**  
  Port mirroring → tcpdump + Python parser → node activity metrics collection → Zabbix over Wireguard tunnel. Result: real-time anomaly detection.

- **Secure messenger (2021)**  
  Deployed a secure instance with E2E encryption + TURN server for VoIP/video over own servers. Result: fully secure solution with high availability and fault tolerance.

- **Android app for security service (2021)**  
  Full-cycle development in Java/Kotlin: design, development, release, API integration, database work, secure storage. Result: prevented critical company losses through rapid data collection.

- **Document recognition system with OpenCV and TensorFlow (2020)**  
  Standalone OCR solution for passports and text documents using TesseractOCR. Result: automated processing of 1,500+ documents/day.

- **Telegram bots for HR automation (2020)**  
  Python + PostgreSQL + Docker, integration with external APIs. Result: handled 10,000+ applications/month, reducing HR workload.

### TezTour Thailand — System Administrator
*May 2018 – December 2019 · Office*

**Stack:** Linux (CentOS, Ubuntu), Windows Server, PostgreSQL, MariaDB, Bash, Python, Zabbix, Docker

- Administered Linux/Windows servers, databases, and user infrastructure.
- Developed Bash/Python scripts to automate routine tasks.
- Supported users and resolved technical incidents.
- Maintained owner infrastructure.
- Supported Zabbix monitoring and Docker containers.

## Open-source Contributions

### ethereum / go-ethereum — protocol-level security fixes

- [PR #34039](https://github.com/ethereum/go-ethereum/pull/34039) (merged) — core: fix txLookupLock mutex leak on error returns in reorg()
- [PR #34737](https://github.com/ethereum/go-ethereum/pull/34737) — core/overlay: prevent silent transition state restart on decode failure
- [PR #34665](https://github.com/ethereum/go-ethereum/pull/34665) — core/txpool/blobpool: prevent data loss in limbo.update on setAndIndex failure
- [PR #34099](https://github.com/ethereum/go-ethereum/pull/34099) — core/filtermaps: return 0 on error in tailPartialBlocks
- [PR #34098](https://github.com/ethereum/go-ethereum/pull/34098) — core/state/snapshot: handle bloom filter errors in diffLayer.rebloom
- [PR #34097](https://github.com/ethereum/go-ethereum/pull/34097) — core/state: log Reader error in commitAndFlush instead of discarding
- [PR #34096](https://github.com/ethereum/go-ethereum/pull/34096) — eth/protocols/snap: handle StateReader error in ServiceTrieNodesQuery
- [PR #34095](https://github.com/ethereum/go-ethereum/pull/34095) — core/filtermaps: replace panics with error returns in matcher
- [Issue #34944](https://github.com/ethereum/go-ethereum/issues/34944) — core/txpool/blobpool: data loss in limbo.update on setAndIndex failure
- [Issue #34038](https://github.com/ethereum/go-ethereum/issues/34038) — core: txLookupLock mutex leaked on error returns in reorg()

### gonka-ai / gonka — decentralized AI infrastructure

**Merged / closed:**
- [PR #1071](https://github.com/gonka-ai/gonka/pull/1071) (merged) — hardening: propagate internal errors across inference/validation/pricing paths
- [PR #1076](https://github.com/gonka-ai/gonka/pull/1076) — fix: propagate storage errors in UpdateDynamicPricing
- [PR #1075](https://github.com/gonka-ai/gonka/pull/1075) — fix: return errors from OverlapsWithPoC instead of swallowing them
- [PR #1074](https://github.com/gonka-ai/gonka/pull/1074) — fix: propagate storage errors in SubmitPocValidationsV2
- [PR #1073](https://github.com/gonka-ai/gonka/pull/1073) — fix: propagate errors in handleInferenceCompleted
- [PR #1072](https://github.com/gonka-ai/gonka/pull/1072) — fix: reject zero completion tokens in FinishInference
- [PR #1012](https://github.com/gonka-ai/gonka/pull/1012) — fix(keeper): propagate SetPocValidationV2 storage error in SubmitPocValidationsV2
- [PR #970](https://github.com/gonka-ai/gonka/pull/970) — fix(keeper): use regexp instead of fmt.Sscanf to parse ErrInsufficientFunds in ClaimRewards
- [PR #968](https://github.com/gonka-ai/gonka/pull/968) — fix(keeper): propagate InjectParamsIntoContext error in Validation handler
- [PR #961](https://github.com/gonka-ai/gonka/pull/961) — test: add reservoir sampling fairness property test
- [PR #960](https://github.com/gonka-ai/gonka/pull/960) — fix: add max-size guard to bandwidth limiter usage maps
- [PR #959](https://github.com/gonka-ai/gonka/pull/959) — fix: unify epoch cache to single invalidation path
- [PR #958](https://github.com/gonka-ai/gonka/pull/958) — fix: add per-epoch validation submission rate limit
- [PR #957](https://github.com/gonka-ai/gonka/pull/957) — fix: add graceful shutdown with signal handling in decentralized-api
- [PR #956](https://github.com/gonka-ai/gonka/pull/956) — fix: return error when InjectParamsIntoContext fails in Validation
- [PR #909](https://github.com/gonka-ai/gonka/pull/909) — bls: propagate caller context to BlsManager and add per-call timeouts
- [PR #878](https://github.com/gonka-ai/gonka/pull/878) — feat(binary-singularity): semantic cache extending #859 #860
- [PR #859](https://github.com/gonka-ai/gonka/pull/859) — feat(semantic-cache): L2 quality gate pipeline — adaptive coherence floor + hub loop closure
- [PR #852](https://github.com/gonka-ai/gonka/pull/852) — fix(bls): use slot-weighted votes in DKG dealer consensus
- [PR #851](https://github.com/gonka-ai/gonka/pull/851) — fix(bls): remove self-validation fallback in group key validation
- [Issue #1067](https://github.com/gonka-ai/gonka/issues/1067) — bug: ClaimRewards error handling — payout path silently continues on failure
- [Issue #848](https://github.com/gonka-ai/gonka/issues/848) — Security: BLS group key validation falls back to self-validation
- [Issue #849](https://github.com/gonka-ai/gonka/issues/849) — Bug: DKG permanent failure — dealer consensus uses unweighted participant votes but quorum uses slot weights

**Open:**
- [PR #1098](https://github.com/gonka-ai/gonka/pull/1098) — devshards Postgres support for devshard storage
- [PR #1017](https://github.com/gonka-ai/gonka/pull/1017) — fix(keeper): add overflow guards in bitcoin supply-cap distribution loop
- [PR #1013](https://github.com/gonka-ai/gonka/pull/1013) — fix(subnet): prevent fund loss in unsettled escrow distribution
- [PR #969](https://github.com/gonka-ai/gonka/pull/969) — fix(dapi): use signal.NotifyContext for graceful shutdown
- [PR #910](https://github.com/gonka-ai/gonka/pull/910) — bls: add epoch-level idempotency guard to ProcessKeyGenerationInitiated
- [PR #854](https://github.com/gonka-ai/gonka/pull/854) — fix(payloadstorage): advance minPruned only after successful prune
- [Issue #908](https://github.com/gonka-ai/gonka/issues/908) — bls: BlsManager stores context.Background() — DKG gRPC calls have no cancellation or timeout

### gonkalabs / opengnk — inference quality & semantic cache

- [PR #2](https://github.com/gonkalabs/opengnk/pull/2) (merged) — L1 semcache: handler X-Cache, toolsim, internal/semcache
- [PR #1](https://github.com/gonkalabs/opengnk/pull/1) (merged) — feat(quality): add inference quality metrics middleware

### Mayveskii / Mimic — MCP execution engine

- [PR #4](https://github.com/Mayveskii/Mimic/pull/4) (merged) — chore: bump Go to 1.26 for security and future compatibility
- [PR #3](https://github.com/Mayveskii/Mimic/pull/3) (merged) — ci: refactor workflows, archive old specs, add releasing docs

### Mayveskii / docpool — RAG document workflow

*Go / PostgreSQL / pgvector · [github.com/Mayveskii/docpool](https://github.com/Mayveskii/docpool)*

Document workflow system with RAG architecture: integration with GonkaGate API, vector search, AI document processing.

### Mayveskii / danila.local — Active Directory automation

*PowerShell · [github.com/Mayveskii/danila.local](https://github.com/Mayveskii/danila.local)*

Automation of Windows Server / AD / GPO domain infrastructure.

## Organizations

- **[mv-core](https://github.com/mv-core)** — decentralized AI compute and protocol infrastructure. Consensus, inference optimization, semantic caching, networking and systems programming.
- **[mv-ml](https://github.com/mv-ml)** — applied machine learning: document AI, OCR, computer vision, RAG, agents and production ML tooling.

## Education

- Vocational education — Economics and accounting
- Additional education — Public and municipal administration

## Languages

- Russian — native
- English — B2 (fluent technical reading)

---

Get in touch: [Telegram](https://t.me/fullom3m3) · [GitHub](https://github.com/Mayveskii)
