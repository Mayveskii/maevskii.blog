---
layout: landing
title: Home
---

<section id="hero" class="hero">
  <div class="hero-content">
    <img class="hero-avatar" src="{{ '/assets/images/avatar.jpg' | relative_url }}" alt="Artemii Maevskii">
    <h1>Artemii Maevskii</h1>
    <div class="hero-subtitle">DevOps / SRE / AI Infrastructure Engineer</div>
    <div class="hero-tagline">
      8 years of production experience — from system administrator to core administrator single-handedly running an entire company's IT infrastructure.
      Research line in AI infrastructure (embryo → Mimic) and protocol-level open source: merged PR in ethereum/go-ethereum, consensus security fixes in gonka-ai/gonka.
    </div>
    <div class="hero-links">
      <a href="#about">About me</a>
      <a href="#experience">Experience</a>
      <a href="#portfolio">Portfolio</a>
      <a href="https://github.com/Mayveskii" target="_blank" rel="noopener">GitHub</a>
      <a href="https://t.me/fullom3m3" target="_blank" rel="noopener">Telegram</a>
    </div>
  </div>
</section>

<section id="about" class="section">
  <div class="wrapper">
    <h2 class="section-title">About</h2>
    <div class="panel">
      <p>Infrastructure engineer with <strong>8 years of production experience</strong>: from system administrator to core administrator carrying an entire company's IT alone — development, deployment, operations, security.</p>
      <p>A separate track is AI infrastructure research (<strong>embryo → Mimic</strong>) and protocol-level open source: a merged PR in <strong>ethereum/go-ethereum</strong> and security fixes for the BLS/DKG consensus in <strong>gonka-ai/gonka</strong>.</p>
      <p class="about-more"><a href="{{ '/about/' | relative_url }}">Read full bio →</a></p>
    </div>
  </div>
</section>

<section id="research" class="section">
  <div class="wrapper">
    <h2 class="section-title">AI Infrastructure Research</h2>
    <div class="skill-grid">
      <div class="skill-card flagship">
        <h3><a href="https://github.com/Mayveskii/embryo" target="_blank" rel="noopener">embryo (binary-mesh)</a> — flagship</h3>
        <p>"Deterministic intelligence": autonomous code analysis, vulnerability hunting and fix generation without an LLM call on mesh coverage. Go monolith + C core (CGO, mmap, binary runtime with 28 opcodes), MCP server with 57 tools, semantic mesh on int8-quantized embeddings (298K slots, &lt;1 ms answers at sim ≥ 0.85), 5-signal hybrid RAG (Qdrant, 180K points), vulnerability hunting in real protocols (gonka, go-ethereum).</p>
      </div>
      <div class="skill-card flagship">
        <h3><a href="https://github.com/Mayveskii/Mimic" target="_blank" rel="noopener">Mimic</a> — the line continues</h3>
        <p>MCP server with a C-core execution engine, orchestrator and 48+ tools.</p>
      </div>
      <div class="skill-card">
        <h3><a href="https://github.com/Mayveskii/teeth_master" target="_blank" rel="noopener">teeth_master</a></h3>
        <p>Evidence-based knowledge base (dentistry, manual therapy) in an agent-ready format: domain skills, research SOPs, source discipline. An example of structuring a subject domain for LLM agents.</p>
      </div>
    </div>
  </div>
</section>

<section id="portfolio" class="section">
  <div class="wrapper">
    <h2 class="section-title">Portfolio</h2>
    <div class="skill-grid">
      <div class="skill-card">
        <h3><a href="https://github.com/Mayveskii/stacktrace" target="_blank" rel="noopener">stacktrace</a></h3>
        <p>Self-hosted DMS with an AI assistant: RAG over documents (Qdrant + local embeddings + LLM gateway), OCR pipeline (Tesseract, Celery, OpenCV), Collabora Online editing via WOPI.</p>
      </div>
      <div class="skill-card">
        <h3><a href="https://github.com/Mayveskii/hradmin" target="_blank" rel="noopener">hradmin</a></h3>
        <p>HR recruiting analytics on top of Bitrix24: ETL into PostgreSQL, Laravel 12 + Filament, reports/dashboards, sync drift control.</p>
      </div>
      <div class="skill-card">
        <h3><a href="https://github.com/Mayveskii/b24_bot" target="_blank" rel="noopener">b24_bot</a></h3>
        <p>Support and facility-management bot in Bitrix24 (Node.js): ticket intake, operator routing, statistics, notifications.</p>
      </div>
      <div class="skill-card">
        <h3><a href="https://github.com/Mayveskii/b24doc_runner" target="_blank" rel="noopener">b24doc_runner</a></h3>
        <p>Bitrix24 Disk → self-hosted NAS file migration: analysis, export, SQLite audit registry — "not a single byte lost".</p>
      </div>
      <div class="skill-card">
        <h3><a href="https://github.com/Mayveskii/Nemesis" target="_blank" rel="noopener">Nemesis</a></h3>
        <p>GitOps management of a fleet of 15+ production Proxmox VE hypervisors: plan → approve → apply → verify, snapshots before changes, runbooks, guardrails for the AI agent.</p>
      </div>
      <div class="skill-card">
        <h3><a href="https://github.com/Mayveskii/ansible-danila" target="_blank" rel="noopener">ansible-danila</a></h3>
        <p>Ansible automation for a fleet of 15+ hypervisors and hundreds of VMs: HTML monitoring reports, Zabbix agent diagnostics, fail2ban hardening, read-only incident collection, webhook triggers from a bot.</p>
      </div>
      <div class="skill-card">
        <h3><a href="https://github.com/Mayveskii/proxdash" target="_blank" rel="noopener">proxdash</a></h3>
        <p>Proxmox infrastructure dashboard: Flask, background cache, automatic network topology diagram (Mermaid), anti-bruteforce.</p>
      </div>
      <div class="skill-card">
        <h3><a href="https://github.com/Mayveskii/rfo_poligon" target="_blank" rel="noopener">rfo_poligon</a></h3>
        <p>CCTV panel on top of Flussonic: HLS camera grid, access groups, Docker Compose, pytest.</p>
      </div>
      <div class="skill-card">
        <h3><a href="https://github.com/Mayveskii/nextcloud" target="_blank" rel="noopener">nextcloud</a></h3>
        <p>Production Nextcloud in Docker (MariaDB + Redis); documented post-mortem of an upgrade incident with recovery.</p>
      </div>
      <div class="skill-card">
        <h3><a href="https://github.com/Mayveskii/docpool" target="_blank" rel="noopener">docpool</a></h3>
        <p>RAG document management, Go.</p>
      </div>
      <div class="skill-card">
        <h3><a href="https://github.com/Mayveskii/race-invariant" target="_blank" rel="noopener">race-invariant</a> · <a href="https://github.com/Mayveskii/boundsafe" target="_blank" rel="noopener">boundsafe</a></h3>
        <p>Testing demos in C: reproducing and fixing a data race (counter without a mutex) and an out-of-bounds write.</p>
      </div>
    </div>
    <p class="experience-more"><a href="https://github.com/Mayveskii?tab=repositories" target="_blank" rel="noopener">All repositories on GitHub →</a></p>
  </div>
</section>

<section id="skills" class="section">
  <div class="wrapper">
    <h2 class="section-title">Key Skills</h2>
    <div class="skill-grid">
      <div class="skill-card">
        <h3>Infrastructure & Virtualization</h3>
        <p>Proxmox VE/PBS, bare-metal, datacenter, Hetzner/VPS/VDS, LXC, KVM, Windows Server 2016–2025, Active Directory, GPO, Keycloak, MeshCentral, PowerShell</p>
      </div>
      <div class="skill-card">
        <h3>Automation & CI/CD</h3>
        <p>Ansible (playbooks, roles, vault), GitLab CI/CD (self-hosted runner), GitHub Actions, Git, IaC, GitOps</p>
      </div>
      <div class="skill-card">
        <h3>Monitoring & Observability</h3>
        <p>Zabbix (500+ hosts), Grafana, custom metrics, Proxmox API</p>
      </div>
      <div class="skill-card">
        <h3>Containers</h3>
        <p>Docker, Docker Compose, Docker Registry; Kubernetes — ready for production</p>
      </div>
      <div class="skill-card">
        <h3>Networking & Security</h3>
        <p>MikroTik, Wireguard, OpenVPN, IPSec, DNS, NAT, firewall, OWASP, Wireshark/tcpdump, fail2ban</p>
      </div>
      <div class="skill-card">
        <h3>Databases</h3>
        <p>PostgreSQL (replication, backup), MariaDB, MySQL, Redis (HA, Sentinel), SQLite, Qdrant, pgvector, SQLAlchemy, Alembic</p>
      </div>
      <div class="skill-card">
        <h3>AI / ML Infrastructure</h3>
        <p>RAG, LLM inference (vLLM), MCP servers/agents, embeddings (sentence-transformers, int8 quantization), OpenCV, TensorFlow, Tesseract OCR</p>
      </div>
      <div class="skill-card">
        <h3>Development</h3>
        <p>Python, Go, PHP (Laravel 12, Filament, Yii2), JavaScript/Node.js, TypeScript/Next.js, Java, Kotlin, C, Bash, REST API, Nginx, Apache</p>
      </div>
      <div class="skill-card">
        <h3>Enterprise & Comms</h3>
        <p>Bitrix24 (REST API, bots, webhooks), mailcow, Asterisk, Matrix Synapse, TURN, Nextcloud, Collabora Online (WOPI), Flussonic, PERCo-WEB, Telegram Bot API</p>
      </div>
      <div class="skill-card">
        <h3>Practices</h3>
        <p>Runbooks, post-mortems, controlled failure tests, rollback plans, handing systems over to internal teams</p>
      </div>
    </div>
  </div>
</section>

<section id="experience" class="section">
  <div class="wrapper">
    <h2 class="section-title">Experience</h2>
    <div class="timeline">
      <div class="timeline-item">
        <div class="timeline-marker"></div>
        <div class="timeline-content panel">
          <h3>danila-master.ru — Core Administrator</h3>
          <div class="timeline-meta">April 2023 – July 2026 · Remote</div>
          <p>The company's entire IT infrastructure in one pair of hands, built and deployed personally: Active Directory domain on Windows Server 2022 with Keycloak SSO, MeshCentral fleet management, software distribution via GPO, GitLab CI/CD deployment pipeline with staged rollouts and rollback, corporate products developed and operated solo (HR analytics, Bitrix24 bots, DMS with AI assistant, dashboards), GitOps-managed fleet of 15+ Proxmox hypervisors (500+ hosts/VMs), Ansible automation, mailcow / Bitrix24 / Asterisk.</p>
        </div>
      </div>
      <div class="timeline-item">
        <div class="timeline-marker"></div>
        <div class="timeline-content panel">
          <h3>System Administrator → Senior System Administrator, InfoSec (NDA)</h3>
          <div class="timeline-meta">2018 – 2023 · 5 years</div>
          <p>Five continuous years: from server administration at an international company (Thailand) to a senior role in the information security department of a large international tour operator. 99.9% uptime of critical 24/7 infrastructure; MikroTik networks and VPNs; custom network monitoring (port mirroring → tcpdump + Python parser → Zabbix); E2E-encrypted corporate messenger (Matrix Synapse) with its own TURN server; Android app for the security service; OCR document recognition (1500+ docs/day); HR Telegram bots (10,000+ tickets/month). Employer names under NDA.</p>
        </div>
      </div>
    </div>
    <p class="experience-more"><a href="{{ '/contributions/' | relative_url }}">See open-source contributions →</a></p>
  </div>
</section>

<section id="contact" class="section">
  <div class="wrapper">
    <h2 class="section-title">Get in touch</h2>
    <div class="panel contact-panel">
      <div class="contact-links">
        <a href="https://t.me/fullom3m3" target="_blank" rel="noopener">Telegram: @fullom3m3</a>
        <a href="mailto:maevskiiartemii@gmail.com">maevskiiartemii@gmail.com</a>
        <a href="https://github.com/Mayveskii" target="_blank" rel="noopener">GitHub: Mayveskii</a>
        <a href="https://mayveskii.github.io/maevskii.blog/">Blog: mayveskii.github.io</a>
      </div>
    </div>
  </div>
</section>
