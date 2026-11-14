# T1007 — System Service Discovery

> Adversaries may try to gather information about registered local system services. Adversaries may obtain information about services using tools as well as OS utility commands such as <code>sc query</code>, <code>tasklist /svc</code>, <code>systemctl --type=service</code>, and <code>net start</code>.

## Identity

- **Record id**: `dea:risk-discovery-t1007-system-service-discovery-jfce9v`
- **Type**: Risk
- **Version**: 0.1.0
- **Lifecycle**: proposed (candidate corpus; admitted via the gated intake
  workflow; canonical admission is a separate evidence-gated step)

## Evidence

Cited from the MITRE ATT&CK knowledge base (mitre/cti STIX, live attack-pattern object). risk_category/likelihood/impact are provisional programmatic values documented here; per-organization likelihood and impact are canonical-admission decisions.

- kind: `published-document` — reference: https://attack.mitre.org/techniques/T1007/ (MITRE ATT&CK enterprise, technique T1007)

## Classification-or-relationships

Deferred: relationship assertions are not made at candidate admission;
bindings land at canonical admission with per-assertion evidence.

## Provenance

Ladder passage: candidate (2026-11-14, Emmanuel A. Otchere).

## Governance

Functional owner: Emmanuel A. Otchere. Steward: Emmanuel A. Otchere. Approval: proposed
(candidate corpus; the approval decision belongs to canonical admission).
