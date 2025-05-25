# Changelog

## 0.0.62
  Breaking changes - NO.

Changes:
- Set `--rpc.max-connections=10000`, default 500.

## 0.0.61
  Breaking changes - NO.

Changes:
- Update reth to `v1.4.3`.
- Update nimbus to `v25.5.0`.

## 0.0.60
  Breaking changes - NO.

Changes:
- Set CPU/RAM limits on backup job pod, to decrease "noisy neighbour" impact.

## 0.0.58
  Breaking changes - NO.

Changes:
- Add readiness probe sidecar, so STS's pods will wait when each upgraded pod become ready, before upgrading the next one.
