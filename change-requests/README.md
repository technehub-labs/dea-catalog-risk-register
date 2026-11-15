# Change Requests: dea-catalog-risk-register

This index tracks every change request that lands on this repository.

| CR | Title | Status | Notes |
|----|-------|--------|-------|
| [CR-RSK-CAT-01](CR-RSK-CAT-01-catalogue-foundation.md) | Catalogue foundation (kit bring-up) | Landed (this PR) | Standard kit: pointer, dependencies, schema projection, gates 1-6, workflows, FOUNDATIONS, record standard. No records admitted. |
| CR-RSK-CAT-02 | Initial population | Planned | Evidence-gated seed population per FOUNDATIONS §7. |

## Numbering

Series tag `CR-RSK-CAT-NN`, sequential. Cross-repo CRs that touch this
repository are recorded here with their home-repo identifier.
| [CR-RSK-CAT-02](CR-RSK-CAT-02-cr-rsk-cat-02.md) | Entity Ingestion Groundwork (candidate intake queue + gates) | **Proposed (this PR)** | Gated intake: queue + blocking queue gate + admission tool (candidate-state subtrees, content-derived ids); pin v2.6.0→v2.8.0 + shard-aware toolchain re-vendor. No records. |
| [CR-RSK-CAT-03](CR-RSK-CAT-03-cr-rsk-cat-03.md) | Risk Candidate Corpus (MITRE ATT&CK + CISA KEV) | **Landed (this PR)** | 2,716 queue submissions (935 ATT&CK techniques + 1,781 CISA KEV vulnerabilities; published prose + evidence citations + source_refs; manifest with sha256s). Queue gate CONFORMANT; no entities change. |
| [CR-RSK-CAT-04](CR-RSK-CAT-04-cr-rsk-cat-04.md) | Risk Candidate Admission Batch 01 (CVE-2025-0411 — 7-Zip Mark of the Web Bypass Vulnerability … CVE-2021-3493 — Linux Kernel Privilege Escalation Vulnerability) | **Landed (this PR)** | Admitted 1400 `Risk` CANDIDATE records via the gated intake workflow (queue gate → admission tool → catalog gates); candidates +1400, canonical unchanged; records at `lifecycle_status: proposed` in `candidates/` subtrees. |
| [CR-RSK-CAT-05](CR-RSK-CAT-05-cr-rsk-cat-05.md) | Risk Candidate Admission Batch 02 (CVE-2022-0185 — Linux Kernel Heap-Based Buffer Overflow Vulnerability … CVE-2026-7273 — Zyxel GS1900 Series Switches Stack-Based Buffer Overflow Vulnerability) | **Landed (this PR)** | Admitted 1316 `Risk` CANDIDATE records via the gated intake workflow (queue gate → admission tool → catalog gates); candidates +1316, canonical unchanged; records at `lifecycle_status: proposed` in `candidates/` subtrees. |
| [CR-RSK-CAT-06](CR-RSK-CAT-06-cr-rsk-cat-06.md) | Canonical Admission Wave (2716) | **Landed (this PR)** | 2716 records promoted candidates/ -> canonical root; ladder completed; evidence preserved; canonical 2716, candidates 0. |
