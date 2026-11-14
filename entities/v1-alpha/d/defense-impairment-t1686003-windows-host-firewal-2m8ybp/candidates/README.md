# T1686.003 — Windows Host Firewall

> Adversaries may disable or modify the Windows host firewall to bypass controls limiting network usage. This can include disabling the Windows host firewall entirely, suppressing specific profiles (domain, private, public), or adding, deleting, and modifying firewall rules to allow or restrict traffic.

## Identity

- **Record id**: `dea:risk-defense-impairment-t1686003-windows-host-firewal-2m8ybp`
- **Type**: Risk
- **Version**: 0.1.0
- **Lifecycle**: proposed (candidate corpus; admitted via the gated intake
  workflow; canonical admission is a separate evidence-gated step)

## Evidence

Cited from the MITRE ATT&CK knowledge base (mitre/cti STIX, live attack-pattern object). risk_category/likelihood/impact are provisional programmatic values documented here; per-organization likelihood and impact are canonical-admission decisions.

- kind: `published-document` — reference: https://attack.mitre.org/techniques/T1686/ (MITRE ATT&CK enterprise, technique T1686.003)

## Classification-or-relationships

Deferred: relationship assertions are not made at candidate admission;
bindings land at canonical admission with per-assertion evidence.

## Provenance

Ladder passage: candidate (2026-11-14, Emmanuel A. Otchere).

## Governance

Functional owner: Emmanuel A. Otchere. Steward: Emmanuel A. Otchere. Approval: proposed
(candidate corpus; the approval decision belongs to canonical admission).
