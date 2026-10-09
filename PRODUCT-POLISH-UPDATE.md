# Member and Staff product polish

## What changed

A shared semantic SVG icon system now describes Member navigation and Reception, CRM and Management actions. The Member dashboard has clearer shortcut cards and a visible entry to the seven-step profile question preview. Mobile uses its sticky dock for primary navigation; submenu destinations retain text labels and receive specific icons for exercise, meals, water, sleep, bookings, locker, wallet and account security.

All surfaces retain the existing glass theme, typeface, keyboard access and server-authorized workspace/branch model. Canonical Auth routes are adopted from the independently verified Auth checkpoint. Existing credentials and operational contracts are unchanged.

## Verification

Private UI source: `cad98dc6691c239f7b58b491348acad1bdd5de72` (includes the product polish at `3310893`).

The pushed source passed a rebuilt production Web review against the real canonical API and exactly 17 migrations in isolated synthetic QA. Five Member sections and three Staff panels passed light/dark and 390/1440 reviews, menu open/Escape, step/goal validation, focus restoration, preview clearing, no horizontal overflow, and English LTR rendering. No customer, financial, hardware or onboarding write was executed. Credentials and private screenshots are excluded.

## Backend boundary

Automatic first-login onboarding, saved answers, resuming and true completion remain blocked on the canonical backend contract. The dashboard entry is clearly a preview. Missing profile state is never interpreted as incomplete or complete. The frozen fields, consent boundaries and recovery semantics remain unchanged.

## Hosted release

The staged visual release was checked on the actual HTTPS origin with existing active Member and Staff review accounts across the same 32 route/width/theme cases. A discovered historical-route redirect to the internal listener was corrected to use the configured owning origin, and explicit HTTPS alias assertions were added. Credentials are unchanged and are not published here. Final deployment evidence and release identity are recorded separately from the UI source checkpoint.
