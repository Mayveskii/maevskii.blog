---
layout: landing
title: Home
---

<section id="hero" class="hero">
  <div class="hero-content">
    <img class="hero-avatar" src="{{ '/assets/images/avatar.jpg' | relative_url }}" alt="Artemii Maevskii">
    <h1>Artemii Maevskii</h1>
    <div class="hero-subtitle">DevOps / SRE / Systems Engineer</div>
    <div class="hero-tagline">
      6 years of production. I ran an entire company's IT as code — and I patch the protocols you run on.
    </div>
    <div class="hero-facts">
      <span>500+ VMs as code</span>
      <span>merged in CNCF</span>
      <span>merged in go-ethereum</span>
      <span>30 PRs to a consensus protocol</span>
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
      <p><strong>gonka-ai/gonka</strong> (Go, Cosmos SDK) — 30 PRs to consensus and inference; <a href="https://github.com/gonka-ai/gonka/pull/1071" target="_blank" rel="noopener">#1071</a> merged.</p>
      <p><strong>gonkalabs/opengnk</strong> — <a href="https://github.com/gonkalabs/opengnk/pull/1" target="_blank" rel="noopener">#1</a>, <a href="https://github.com/gonkalabs/opengnk/pull/2" target="_blank" rel="noopener">#2</a> merged: inference quality metrics, L1 semantic cache.</p>
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
          <h3>danila-master.ru — DevOps Engineer (lead system administrator)</h3>
          <div class="timeline-meta">April 2024 – July 2026 · Remote</div>
          <p>The company's entire IT in one pair of hands, managed fully as code: 15+ Proxmox hypervisors, 500+ VMs, AD domain across Russia with Keycloak SSO, GitLab CI/CD with zero-downtime deploys, and a line of in-house products shipped solo — from a DMS with an AI assistant to datacenter automation.</p>
        </div>
      </div>
      <div class="timeline-item">
        <div class="timeline-marker"></div>
        <div class="timeline-content panel">
          <h3>System Administrator → Senior System Administrator, InfoSec (NDA)</h3>
          <div class="timeline-meta">2019 – 2023 · 4 years</div>
          <p>From server administration at an international company (Thailand) to a senior InfoSec role at a major international tour operator: 95% uptime under 24/7 requirements, custom network monitoring, E2E-encrypted corporate messenger, OCR at 1,500+ docs/day.</p>
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
        <a href="https://github.com/Mayveskii" target="_blank" rel="noopener">GitHub: Mayveskii</a>
      </div>
    </div>
  </div>
</section>
