# dea-catalog-risk-register

> DEA catalog for **Risk** — OpenDEAM v0.3.0 (ADR-0003).

## Risk (`RSK`)

- **Entity id:** `dea:entity-risk`
- **Allocation:** L2 · L2-risk-compliance
- **Status:** proposed

A condition or event that threatens the enterprise's ability to persist or to realize a capability/objective.

## Relationships (from the OpenDEAM model)

- **RSK → CAP** — threatens (dependency, 0..N:0..N)
- **RSK → SF** — threatens (dependency, 0..N:0..N)
- **CTL → RSK** — mitigates (governance, 0..N:0..N)
- **AIM → RSK** — subject to (governed_by) (governance, 0..N:0..N)

## Allocation contract

This repo's `metamodel-pointer.yaml` is validated in CI against the pinned
OpenDEAM root model (`v0.3.0`) via the reusable
`validate-against-model.yml` workflow. Drift fails CI.

Content (entity instances) lands when the entity promotes from
`proposed` to `planned`/`scaffold` per the model lifecycle.

## License

Apache 2.0 — see [LICENSE](./LICENSE) and [NOTICE](./NOTICE).
