# Changelog

## [Unreleased]

### CR-RSK-CAT-06: Canonical Admission Wave

2716 Risk records promoted from the candidate slot to the canonical slot (provenance ladder completed per record; evidence citations preserved; ids untouched). Index: canonical 2716, candidates 0. All gates green.

### CR-RSK-CAT-05: Risk Candidate Admission Batch 02

Admitted 1316 new `Risk` CANDIDATE records through the gated intake workflow (queue gate → admission tool → catalog gates); ids content-derived and collision-checked; records land in `candidates/` subtrees at `lifecycle_status: proposed` / version 0.1.0; candidates count +1316, canonical unchanged; queue entries flipped to `admitted`.

### CR-RSK-CAT-04: Risk Candidate Admission Batch 01

Admitted 1400 new `Risk` CANDIDATE records through the gated intake workflow (queue gate → admission tool → catalog gates); ids content-derived and collision-checked; records land in `candidates/` subtrees at `lifecycle_status: proposed` / version 0.1.0; candidates count +1400, canonical unchanged; queue entries flipped to `admitted`.

### CR-RSK-CAT-03: Risk Candidate Corpus (MITRE ATT&CK + CISA KEV)

2,716 Risk candidate submissions landed in the contribution queue (sharded, gate-CONFORMANT): 935 MITRE ATT&CK live techniques (enterprise + ICS + mobile) + 1,781 CISA KEV vulnerabilities. Published description prose, published-document evidence citations, source_refs (technique ids / CVE ids); provenance in ingestion/manifest.yaml. Likelihood/impact mappings provisional and documented. No catalog entities change; admission follows in CR-RSK-CAT-04/05.

### CR-RSK-CAT-02: Entity Ingestion Groundwork (candidate intake queue + gates)

Gated intake workflow stood up: contribution queue + blocking queue gate (`scripts/check_contributions.py`, self-deriving from the projected schema) + admission tool (`scripts/admit_entity.py`: content-derived ids, collision-checked, candidates/ subtrees at `lifecycle_status: proposed` / v0.1.0) + intake template and process docs. CI: queue gate added as a blocking step; metaframework pin v2.6.0 → v2.8.0 with the shard-aware toolchain re-vendored from the v2.8.0 release (cmp'd). No records admitted by this CR.

### `CR-RSK-CAT-01` — catalogue foundation (kit bring-up)

Standard kit generated from the metamodel (org-wide catalog advancement
programme): hybrid pointer pinned to OpenDEAM v0.8.0;
`dependencies.yaml`; schema projection (copied-and-narrowed) with the
catalogue-instance layer; vendored relationship-instance contract; fixtures;
gates 1-6 wired into `validate-catalogue.yml` plus allocation and authorship
workflows; FOUNDATIONS (D-1..D-6) and record documentation standard. No
records admitted (population gated on CR-RSK-CAT-02).
