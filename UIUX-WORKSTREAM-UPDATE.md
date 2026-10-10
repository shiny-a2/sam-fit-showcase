# Track B UI-00 / UI-01 — independent frontend checkpoint

The Track B frontend now has a source-first workspace audit and a shared, industry-neutral modal navigation helper. Existing Member and Staff menus reuse the accepted visual tokens and components.

The change moves focus into an open menu, contains forward and reverse keyboard navigation, isolates background content, restores focus after closing and cleans up the modal state when switching to desktop layout. Member header and dock report the menu state consistently. This is an interaction correction, not a new backend authorization mechanism.

Production-mode browser review passed 48 representative surface cases: five workspaces at 390/768/1366/1440 in both themes, plus English Member presentation. Branch Manager and CRM-only Users also passed explicit workspace and foreign-branch denial checks. The matched before/after root images had no dimension changes; open-menu interactions were reviewed separately. Before/after screenshots and sensitive QA evidence remain private. Full product accessibility, commercial workflows, newer canonical backend adoption and production acceptance remain separate requirements.

The checkpoint is prepared independently for selective review. Existing staging services, backend models, migrations, financial records, source systems and physical devices are unchanged. No automatic Main merge or deployment is included.

Developer: [a2 sport](https://amiraliyaghouti.com).
