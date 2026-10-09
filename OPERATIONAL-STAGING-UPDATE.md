# Operational staging and canonical Auth integration

## Delivered

Track B now has a separate HTTPS staging hostname: https://staging-sport.amiraliyaghouti.com. The existing sport DNS record and WordPress data were preserved during this update.

The deployed private release is `9b96830f6a55632daf4ed507d99fcee764f056bd`, version `0.1.0-staging.8`. It integrates the independently verified Auth/Route checkpoint and current Main API contracts. Linux production build and explicit migration status passed with exactly 17 migrations; candidate migration 018 was not adopted.

The deployment work includes separate supervised application services, isolated queue/heartbeat state, immutable release custody, bounded logs, HTTPS renewal verification, encrypted backups and a repeatable browser acceptance gate. No credentials, private data, infrastructure access material or QA screenshots are published here.

## Verified outcomes

- Real HTTPS Member/Staff login, workspace and branch resolution, direct authorization and separate same-Person Users.
- Current grants after branch/workspace removal, session revocation, stale authorization revision and disabled accounts.
- Canonical CRM List/Today and safe Reception reads return 200. Candidate-only reads remain unavailable; deployment does not fabricate facts or activate candidate schema.
- 32 responsive theme/width configurations after reboot, including keyboard interactions, reduced motion and overflow checks.
- Actual dependency failure degrades readiness; recovery occurs automatically.
- Controlled reboot restores services automatically.
- Application rollback to the previously verified release and rollforward passed without a database rollback.
- Authenticated encrypted backup, isolated restore, tamper denial and an off-server custody copy passed.

## Remaining gates

Synthetic staging platform acceptance passed. Main handoff remains **NOT_READY**, with P0=0 and two tracked P1 gates: accepted VPS REAL_PILOT/Edge admission, and the pre-existing discrepancy between the intended Track A hostname and its current DNS destination. The latter was reported to the owner; this execution added only the new staging record.

The real 208-locker catalogue is absent from staging. No fixture replacement, source-reader deployment, direct source database access or physical control was introduced. Live Shadow validation remains FALSE. Main Development owns final release and cutover decisions.

Daily encrypted backups are scheduled locally; off-server copying was verified as an owner-custody step and is not claimed to be an automatic offsite service. Larger-data capacity and production disaster recovery are outside this bounded synthetic staging acceptance.
