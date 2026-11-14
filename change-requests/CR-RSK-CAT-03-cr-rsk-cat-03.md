# CR-RSK-CAT-03: Risk Candidate Corpus (MITRE ATT&CK + CISA KEV)

**Status**: Landed (this PR)
**Layer**: Catalog content (candidate corpus intake)
**Owner**: Emmanuel A. Otchere
**Date**: 2026-11-14
**Admission authority**: candidate corpus only (canonical admission remains the evidence-gated step; FOUNDATIONS D-4/D-5)
**Trigger**: Catalog population programme (2026-11 owner directive). This CR populates the risk-register queue — the candidate seed sources named per FOUNDATIONS §7 and CR-RSK-CAT-01.
**Carrier**: Single PR on feature branch `feat/cr-rsk-cat-03`. PR review, not direct push.
**Lands against**: `main`
**Depends on**: CR-RSK-CAT-02 (ingestion groundwork).

## 1. What this CR lands

**2,716 Risk candidate submissions** in `contributions/queue/<shard>/<slug>.yaml` from two evidence banks:

| Bank | Source | Records |
|---|---|---|
| attack-techniques.json | MITRE ATT&CK knowledge base (mitre/cti STIX; enterprise 706 + ICS 104 + mobile 125 live attack-patterns) | 935 |
| cisa-kev.json | CISA Known Exploited Vulnerabilities catalog (official JSON feed) | 1,781 |

Provenance in `ingestion/manifest.yaml` (bank sha256s, source URLs, retrieval dates, mapping note). Every submission carries `source_ref` (MITRE ATT&CK technique id / CISA KEV CVE id), a `published-document` evidence citation, and published description prose.

**Honest mappings**: risk_category=technology for both banks; likelihood=possible (ATT&CK techniques — the neutral-credible enum value) and almost-certain (KEV — the catalog's confirmed-exploitation definition); impact=major (KEV: severe for known ransomware campaigns). All values provisional and documented per record; per-organization likelihood/impact are canonical-admission decisions.

**Shard distribution**: slugs are semantic-prefix-first (ATT&CK tactic; KEV vendor) so the letter-shard layout respects the 800-entry directory cap (largest shard < 400).

## 2. What changes

- `contributions/queue/<shard>/` — 2,716 intake submissions (`status: queued`)
- `ingestion/manifest.yaml` — corpus provenance record (new)
- No `CATALOG.yaml` change (queue ≠ index)
- This CR file and the index row

## 3. Verification

- `check_contributions.py`: CONFORMANT (2,716 queue files)
- No directory holds 800+ entries
- Spot-checks: technique records trace to attack.mitre.org ids; KEV records trace to CVE ids in the official feed

## 4. NOT-List

- NOT record admission (nothing under `entities/` changes; admission follows in CR-RSK-CAT-04/05).
- NOT a modification of gates, schemas, or intake tooling.
- NOT an authoritative likelihood/impact assessment — provisional by construction.

## 5. Acceptance criteria

1. 2,716 gate-CONFORMANT submissions; manifest carries both bank sha256s + source URLs.
2. Submissions carry no `id`; `status: queued`; `submitted_by: Emmanuel A. Otchere`.
3. `CATALOG.yaml` counts unchanged.
