# T1563 — Remote Service Session Hijacking

> Adversaries may take control of preexisting sessions with remote services to move laterally in an environment. Users may use valid credentials to log into a service specifically designed to accept remote connections, such as telnet, SSH, and RDP.

## Identity

- **Record id**: `dea:risk-lateral-movement-t1563-remote-service-session-hi-59468q`
- **Type**: Risk
- **Version**: 0.1.0
- **Lifecycle**: proposed (candidate corpus; admitted via the gated intake
  workflow; canonical admission is a separate evidence-gated step)

## Evidence

Cited from the MITRE ATT&CK knowledge base (mitre/cti STIX, live attack-pattern object). risk_category/likelihood/impact are provisional programmatic values documented here; per-organization likelihood and impact are canonical-admission decisions.

- kind: `published-document` — reference: https://attack.mitre.org/techniques/T1563/ (MITRE ATT&CK enterprise, technique T1563)

## Classification-or-relationships

Deferred: relationship assertions are not made at candidate admission;
bindings land at canonical admission with per-assertion evidence.

## Provenance

Ladder passage: candidate (2026-11-14, Emmanuel A. Otchere).

## Governance

Functional owner: Emmanuel A. Otchere. Steward: Emmanuel A. Otchere. Approval: proposed
(candidate corpus; the approval decision belongs to canonical admission).
