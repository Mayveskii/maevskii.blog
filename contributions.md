---
layout: page
title: Open Source
permalink: /contributions/
---

I work on protocol reliability, consensus safety and error propagation. Most findings come from [embryo](https://github.com/Mayveskii/embryo) — my own autonomous code-analysis system — and are prepared, tested and submitted by it under my review. Statuses verified via the GitHub API on 2026-09-22.

**At a glance:** merged in kubernetes-sigs/kueue (CNCF) · merged in ethereum/go-ethereum · merged in gonka-ai/gonka (consensus, Go/Cosmos SDK).

---

## kubernetes-sigs / kueue (CNCF, SIG-Scheduling)

- [Issue #13572](https://github.com/kubernetes-sigs/kueue/issues/13572) + [PR #13573](https://github.com/kubernetes-sigs/kueue/pull/13573) (**merged**, cherry-picked into release branches) — a trust-boundary bug class in the job framework: through non-controller ownerReferences one cluster user could delete and hijack other users' Workloads.

## ethereum / go-ethereum

- [PR #34039](https://github.com/ethereum/go-ethereum/pull/34039) (**merged**) — core: fix txLookupLock mutex leak on error returns in reorg().

## gonka-ai / gonka

Decentralized AI network (Go / Cosmos SDK). A series of PRs on BLS/DKG consensus and error propagation.

- [PR #1071](https://github.com/gonka-ai/gonka/pull/1071) (**merged**) — error propagation hardening.

---

## Own research

- [embryo](https://github.com/Mayveskii/embryo) — autonomous code analysis and fix generation: successful solutions are distilled into proven executable patterns and reused without repeated inference. The hunting pipeline behind the findings above.
- [Mimic](https://github.com/Mayveskii/Mimic) — deterministic execution layer for AI agents: every operation is validated before it runs, cost is measured, failures roll back.
