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
      <a href="{{ site.baseurl }}/contributions/">Contributions</a>
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

## Open-source Work

I contribute security and reliability fixes to core protocols and AI infrastructure. Highlights include merged fixes in **ethereum/go-ethereum**, consensus and inference hardening in **gonka-ai/gonka**, and L1 semantic cache work in **gonkalabs/opengnk**. My own projects include **Mayveskii/Mimic**, **Mayveskii/docpool** and **Mayveskii/danila.local**.

[See full contribution list →]({{ site.baseurl }}/contributions/)

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
