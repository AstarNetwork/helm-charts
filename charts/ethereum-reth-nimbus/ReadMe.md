# Changelog

## 0.0.64
  Added `nameOverride` over `p2pNlb` to harcode load-balancer name if chosen.
  Breaking changes - NO.

## 0.0.63
  Breaking changes - NO.

Changes:
- Comment out default rediness-probe container env vars
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
