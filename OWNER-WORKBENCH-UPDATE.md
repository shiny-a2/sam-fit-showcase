# Owner workbench — staging 0.1.0-staging.11

The staging owner review account now has explicit backend grants for the currently executable Member, Reception, CRM, Management and Technical experiences. Staff workbench navigation includes a separate Member login entry only when the authenticated User has the canonical Member grant. Sharing a Person with another Member User does not expose this entry.

Branch access is explicitly assigned to currently active branches; no wildcard authorization is introduced. Member and Staff sessions remain isolated. Specialist destinations are clearly marked pending and have no executable navigation or grant controls.

The account bootstrap is restricted to the isolated staging database and the canonical 17-migration baseline. Credentials, customer records and private implementation evidence are excluded from this showcase. No financial, service-order or hardware operations are performed by this update.

Verification: production Web build, canonical authorization checks and browser review of both themes at phone and desktop widths. Actual HTTPS owner login passed in both contexts, all five available panels opened, and the workbench passed four phone/desktop light/dark cases without horizontal overflow. Nine pending specialist entries remained noninteractive. Postcommit verification passed on the exact deployed source, including the Staff-only User negative check.
