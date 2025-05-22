# Changelog

## 0.0.59
  Breaking changes - NO.

Changes:
- Run `restic backup` with the least IO and CPU priority (`ionice -c3 nice -n19 restic backup ...`).

## 0.0.58
  Breaking changes - NO.

Changes:
- Add readiness probe sidecar, so STS's pods will wait when each upgraded pod become ready, before upgrading the next one.
