# T1558.002 — Silver Ticket

> Adversaries who have the password hash of a target service account (e.g. SharePoint, MSSQL) may forge Kerberos ticket granting service (TGS) tickets, also known as silver tickets. Kerberos TGS tickets are also known as service tickets.

## Identity

- **Record id**: `dea:risk-credential-access-t1558002-silver-ticket-cnz3p6`
- **Type**: Risk
- **Version**: 0.1.0
- **Lifecycle**: proposed (candidate corpus; admitted via the gated intake
  workflow; canonical admission is a separate evidence-gated step)

## Evidence

Cited from the MITRE ATT&CK knowledge base (mitre/cti STIX, live attack-pattern object). risk_category/likelihood/impact are provisional programmatic values documented here; per-organization likelihood and impact are canonical-admission decisions.

- kind: `published-document` — reference: https://attack.mitre.org/techniques/T1558/ (MITRE ATT&CK enterprise, technique T1558.002)

## Classification-or-relationships

Deferred: relationship assertions are not made at candidate admission;
bindings land at canonical admission with per-assertion evidence.

## Provenance

Ladder passage: candidate (2026-11-14, Emmanuel A. Otchere).

## Governance

Functional owner: Emmanuel A. Otchere. Steward: Emmanuel A. Otchere. Approval: proposed
(candidate corpus; the approval decision belongs to canonical admission).
