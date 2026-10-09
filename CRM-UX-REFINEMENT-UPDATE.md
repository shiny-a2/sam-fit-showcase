# CRM experience refinement

2026-10-09 · Web source release 0.1.0-local.8 · Source checkpoint f04b0dc

## What changed

- Compared the established CRM reference with the canonical product UI before changing the experience. Reused compact record scanning, focused detail and action locality while preserving the canonical identity and authorization boundaries.
- Refined Today and Lead lists with smaller operational headings, clearer record facts and a focused right-side detail drawer that preserves list position.
- Distinguished unavailable summaries, queues and optional commercial context from successful empty results and real zero counts. Unsupported search and optional actions are explained rather than made executable.
- Retained separate Lead and Member context, server-owned stage transitions and existing uncertain-command receipt protection. Added visible active filter context to supported candidate queues.
- Reviewed desktop, tablet and mobile in both themes, including keyboard form interaction, modal focus return, offline clearing, branch denial and session logout. Corrected the light-theme primary-action text contrast.

## Why it matters

Operators can scan records and inspect a sales prospect without losing context. Missing integration data is communicated honestly, and a polished screen does not imply backend authority or business completion.

## Evidence and limits

Bounded real-browser review uses an isolated synthetic environment with the existing canonical 17-migration baseline. Temporary visual QA records are removed afterward. Seven explicit contract requests cover the missing full search, Member commercial view, workload lists, Opportunity, Pipeline, contact availability and freshness metadata.

CRM remains **CANONICAL_ADOPTION_WATCH**. Deep commercial views and human operator acceptance remain pending the owning contracts. This source/design release does not deploy staging, promote candidate migrations or claim REAL_PILOT/product completion. No legacy backend port, new domain, business semantics, financial records, hardware actions or permission expansion were introduced.

Public material contains sanitized notes only; production source and detailed evidence remain private.
