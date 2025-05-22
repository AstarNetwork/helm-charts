# Changelog

## 0.0.60
  Breaking changes - NO.

Changes:
- Set CPU/RAM limits on backup job pod, to decrease "noisy neighbour" impact.

## 0.0.58
  Breaking changes - NO.

Changes:
- Add readiness probe sidecar, so STS's pods will wait when each upgraded pod become ready, before upgrading the next one.
