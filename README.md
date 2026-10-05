# Sam Fit engineering notes

Work toward a central platform for a multi-branch fitness business begins with understanding the existing reception software and equipment.

## Current work

Track A is a deployed, isolated sports product-validation environment with operator CRM, management and member experiences. The current release adds the approved branch directory, scoped role accounts and realistic synthetic scenarios. Dates use the Jalali calendar and Tehran time. Final independent platform architecture remains a separate future VPS track. Reception software and hardware integration remain outside this release.

The private repository contains implementation tools. This showcase publishes progress and validation notes without credentials, customer records, infrastructure addresses or private implementation details.

## Updates

### 2026-10-06 — Sports validation release 0.5.0

Added branch-aware synthetic profiles, varied wallet scenarios and role-specific testing. Standardized Persian product copy and Jalali reminder scheduling. Verified calendar boundaries, server-side permissions and light/dark interfaces at mobile and desktop widths. No customer production data was imported.

### 2026-10-05 — Discovery groundwork

- Inspected the available hosts and confirmed the owner's choice of a temporary relay.
- Separated the relay role from the future application host.
- Prepared a dedicated public-key access design with no public listener at the branch.
- Created isolated relay account storage without restarting existing services.
- Prepared the reception bootstrap for review, including bounded automatic reconnection.
- Resolved the relay account-profile blocker with an approved account-only correction.
- Verified key authentication, loopback isolation, access restrictions and a fresh relay connection. Removed the test credentials and listener afterward.
- Branch identity and reception-PC bootstrap execution remain pending. Network-loss and reboot recovery have not yet been validated on site.
- Prepared an approved single-paste operator handoff with a dedicated administrator account and key authentication. The owner requested ongoing access with explicit revocation instead of automatic expiry. Reception execution is pending; operational discovery remains read-only first.
- Updated the handoff after operator diagnostics exposed damaged multiline pasting. The new transport preserves the source and waits for central verification before displaying Connected. The owner forwards the initial public-key output once; no second reception command is required for normal enrollment.
- Field execution reached key generation but failed at local SSH startup. Public-key enrollment is complete; a targeted diagnostic repair is prepared. The branch is not yet marked Connected or Ready.

No hardware integration, database access or production connector has been validated yet.
