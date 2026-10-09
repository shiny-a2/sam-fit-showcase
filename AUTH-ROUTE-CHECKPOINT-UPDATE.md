# Independent Auth/Route checkpoint

## What changed

An independent checkpoint now verifies the existing Member and Staff login experience against the current canonical Main API. The test matrix includes separate login entry points, legacy routing, authorized workspace and branch selection, logout destinations, direct protected routes, revoked and stale sessions, disabled accounts, and separate Member/Staff Users belonging to the same Person.

The current Main behavior rejects sessions that no longer have any authorized workspace. Regression checks now reflect that contract and verify that unrelated authorized access remains usable.

## Why it matters

Main Development can consume a specific, reproducible private Auth snapshot without mixing CRM refinement or deployment work. A dedicated gate checks the pushed commit, rebuilds the production Web application and repeats real-browser verification on that exact revision.

## Verified checkpoint

- Private source: `edf57d2728b35a1029f4394fcbc8b6d5a89cdf08`.
- Canonical API source: `242a395c4cfdd439fae33d9c8740f201d57cf2ee`.
- Postcommit production Web build, route matrix, auth matrix and same-Person isolation: PASS.
- Canonical database compatibility: exactly 17 migrations; migration 018 is not required.
- Auth P0: 0. Auth P1: 0.
- Secret scan: PASS; credentials and private QA artifacts are excluded.

Checks use isolated synthetic QA identities. Login presentation is checked in light and dark themes at mobile, tablet and desktop widths, including keyboard interaction and reduced motion. This evidence does not certify VPS deployment, disaster recovery or unrelated CRM workflows.

Main consumes the private source revision. This public note contains no customer records, credentials, screenshots of private data or infrastructure access details.
