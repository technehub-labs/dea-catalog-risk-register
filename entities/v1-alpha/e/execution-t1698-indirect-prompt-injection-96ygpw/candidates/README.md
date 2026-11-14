# T1698 — Indirect Prompt Injection

> Adversaries may deliver malicious prompts to an LLM indirectly by embedding the prompts in content that the adversary expects may be processed by an LLM. These prompts can be included in web pages, documents, emails, tickets, code, or other sources that an agent, copilot, or other AI system may retrieve and process.

## Identity

- **Record id**: `dea:risk-execution-t1698-indirect-prompt-injection-96ygpw`
- **Type**: Risk
- **Version**: 0.1.0
- **Lifecycle**: proposed (candidate corpus; admitted via the gated intake
  workflow; canonical admission is a separate evidence-gated step)

## Evidence

Cited from the MITRE ATT&CK knowledge base (mitre/cti STIX, live attack-pattern object). risk_category/likelihood/impact are provisional programmatic values documented here; per-organization likelihood and impact are canonical-admission decisions.

- kind: `published-document` — reference: https://attack.mitre.org/techniques/T1698/ (MITRE ATT&CK enterprise, technique T1698)

## Classification-or-relationships

Deferred: relationship assertions are not made at candidate admission;
bindings land at canonical admission with per-assertion evidence.

## Provenance

Ladder passage: candidate (2026-11-14, Emmanuel A. Otchere).

## Governance

Functional owner: Emmanuel A. Otchere. Steward: Emmanuel A. Otchere. Approval: proposed
(candidate corpus; the approval decision belongs to canonical admission).
