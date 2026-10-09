# Independent Auth/Route checkpoint

## What changed

An independent checkpoint now verifies the existing Member and Staff login experience against the current canonical Main API. The test matrix includes separate login entry points, legacy routing, authorized workspace and branch selection, logout destinations, direct protected routes, revoked and stale sessions, disabled accounts, and separate Member/Staff Users belonging to the same Person.

The current Main behavior rejects sessions that no longer have any authorized workspace. Regression checks now reflect that contract and verify that unrelated authorized access remains usable.

## Why it matters

Main Development can consume a specific, reproducible private Auth snapshot without mixing CRM refinement or deployment work. A dedicated gate checks the pushed commit, rebuilds the production Web application and repeats real-browser verification on that exact revision.

## Verified checkpoint

- Private source: `e996ebc0c548ed460d2388f26feb2e9b2dfbcaa3`.
- Canonical API source: `242a395c4cfdd439fae33d9c8740f201d57cf2ee`.
- Postcommit production Web build, route matrix, auth matrix and same-Person isolation: PASS.
- Canonical database compatibility: exactly 17 migrations; migration 018 is not required.
- Auth P0: 0. Auth P1: 0.
- Secret scan: PASS; credentials and private QA artifacts are excluded.

Checks use isolated synthetic QA identities. Login presentation is checked in light and dark themes at mobile, tablet and desktop widths, including keyboard interaction and reduced motion. This evidence does not certify VPS deployment, disaster recovery or unrelated CRM workflows.

Main consumes the private source revision. This public note contains no customer records, credentials, screenshots of private data or infrastructure access details.

## Final canonical route closure

Reception, CRM, Management and Technical now use their canonical product routes. Historical routes redirect explicitly, preserve branch/query context and share the existing protected implementation. Workspace presentation paths are normalized without changing server grants, permissions or branch authority.

The final independent private commit was pushed before the complete production build and real-browser matrix were repeated on that exact SHA. Authorized Staff can open all four canonical routes; wrong-context and unauthorized Staff are denied. Disabled Staff and revoked sessions are denied across all four direct routes. Existing Member destinations and same-Person separate-User isolation remain intact.

This is a source checkpoint for downstream integration. It has not replaced the VPS deployment. Main Development must run its own integrated disaster-recovery gate after consuming the exact private revision.
