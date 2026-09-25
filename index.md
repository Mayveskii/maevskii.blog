---
layout: landing
title: Home
---

<section id="hero" class="hero">
  <div class="hero-content">
    <img class="hero-avatar" src="{{ '/assets/images/avatar.jpg' | relative_url }}" alt="Artemii Maevskii">
    <h1>Artemii Maevskii</h1>
    <div class="hero-subtitle">DevOps / Senior SysAdmin</div>
    <div class="hero-tagline">
      6 years of production. I ran an entire company's IT as code — and I patch the protocols you run on.
    </div>
    <div class="hero-facts">
      <span>500+ VMs as code</span>
      <span>merged in CNCF</span>
      <span>merged in go-ethereum</span>
      <span>merged in gonka (Cosmos SDK)</span>
    </div>
    <div class="hero-links">
      <a href="{{ '/about/' | relative_url }}">Work</a>
      <a href="{{ '/contributions/' | relative_url }}">Open source</a>
      <a href="https://github.com/Mayveskii" target="_blank" rel="noopener">GitHub</a>
      <a href="https://t.me/fullom3m3" target="_blank" rel="noopener">Telegram</a>
    </div>
  </div>
</section>

<section id="featured" class="section">
  <div class="wrapper">
    <h2 class="section-title">Featured work</h2>
    <div class="skill-grid">
      <div class="skill-card flagship">
        <h3><a href="https://github.com/Mayveskii/embryo" target="_blank" rel="noopener">embryo (binary-mesh)</a></h3>
        <p>Autonomous code analysis and fix generation: solutions are distilled into proven patterns and reused without repeated inference. Its findings became merged PRs in kueue, go-ethereum and gonka.</p>
      </div>
      <div class="skill-card">
        <h3><a href="https://github.com/Mayveskii/stacktrace" target="_blank" rel="noopener">stacktrace</a></h3>
        <p>Corporate DMS with an AI assistant, in production: RAG on Qdrant, OCR pipeline, Collabora Online editing. FastAPI, Next.js, PostgreSQL.</p>
      </div>
      <div class="skill-card">
        <h3><a href="https://github.com/Mayveskii/ansible-danila" target="_blank" rel="noopener">ansible-danila</a></h3>
        <p>A datacenter as code: 15+ hypervisors and hundreds of VMs under Ansible — monitoring reports, agent diagnostics, hardening, bot-triggered playbooks.</p>
      </div>
      <div class="skill-card">
        <h3><a href="https://github.com/Mayveskii/docpool" target="_blank" rel="noopener">docpool</a></h3>
        <p>Document management with a RAG chat in Go: pgvector search, streaming answers verified against sources, protected PDF copies.</p>
      </div>
    </div>
    <p class="experience-more"><a href="{{ '/about/' | relative_url }}">Full career &amp; all products →</a></p>
  </div>
</section>

<section id="opensource" class="section">
  <div class="wrapper">
    <h2 class="section-title">Open source</h2>
    <div class="panel">
      <p><strong>kubernetes-sigs/kueue</strong> (CNCF, SIG-Scheduling) — found and fixed a multi-tenancy security hole: one cluster user could delete and hijack others' Workloads. <a href="https://github.com/kubernetes-sigs/kueue/pull/13573" target="_blank" rel="noopener">PR #13573</a> merged, cherry-picked into release branches.</p>
      <p><strong>ethereum/go-ethereum</strong> — <a href="https://github.com/ethereum/go-ethereum/pull/34039" target="_blank" rel="noopener">PR #34039</a> merged: txLookupLock mutex leak in reorg().</p>
      <p><strong>gonka-ai/gonka</strong> (Go, Cosmos SDK) — a series of PRs on BLS/DKG consensus and error propagation; <a href="https://github.com/gonka-ai/gonka/pull/1071" target="_blank" rel="noopener">#1071</a> merged.</p>
      <p class="about-more"><a href="{{ '/contributions/' | relative_url }}">All contributions →</a></p>
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
          <h3>Core DevOps — danila-master.ru, product company</h3>
          <div class="timeline-meta">2023 – 2026 · Remote</div>
          <p>15+ Proxmox VE hypervisors, 500+ VMs, everything managed as code with Ansible. Monitoring of 500+ hosts (Zabbix, VictoriaMetrics, Grafana, Alertmanager, alerts to Telegram, logs via Vector), ETL contour (Airflow, ClickHouse, ELK), Kubernetes/OpenShift, GitLab CI/CD with dev/uat/prod and rollback by tag, proxy contour (NGINX, Nginx Proxy Manager, HAProxy, wildcard TLS), AD from scratch with Keycloak SSO, MeshCentral — plus a line of in-house products shipped solo, from a DMS with an AI assistant to datacenter automation.</p>
        </div>
      </div>
      <div class="timeline-item">
        <div class="timeline-marker"></div>
        <div class="timeline-content panel">
          <h3>System Administrator → Senior System Administrator, InfoSec (NDA)</h3>
          <div class="timeline-meta">2019 – 2023 · 4 years</div>
          <p>From server administration at an international company (Thailand) to a senior InfoSec role at a major international tour operator: custom network monitoring, E2E-encrypted corporate messenger, OCR at 1,500+ docs/day.</p>
        </div>
      </div>
    </div>
  </div>
</section>

<section id="contact" class="section">
  <div class="wrapper">
    <h2 class="section-title">Get in touch</h2>
    <div class="panel contact-panel">
      <div class="contact-links">
        <a href="https://t.me/fullom3m3" target="_blank" rel="noopener">Telegram: @fullom3m3</a>
        <a href="mailto:maevskiiartemii@gmail.com">maevskiiartemii@gmail.com</a>
        <a href="tel:+79301209169">+7 (930) 120-91-69</a>
        <a href="https://github.com/Mayveskii" target="_blank" rel="noopener">GitHub: Mayveskii</a>
      </div>
    </div>
  </div>
</section>
