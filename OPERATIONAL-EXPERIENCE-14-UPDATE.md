# Operational Experience 14 — source-backed daily work

This independent Track B candidate builds on the UI-13 changes already adopted by the latest inspected Main RC. It sharpens the existing workflow instead of replacing the interface.

- CRM Today now places four verified workload signals before its paged work lists. Missing data is labeled unavailable, and a denied child queue closes the whole Today view.
- The CRM work list shares the operator roster already read by Today, avoids a duplicate request, and does not mistake an unavailable roster for an unassigned owner.
- Branch management can refresh its CRM overview; Reception shows a clear focus location after opening a member profile; Member home can refresh accepted account reads in Persian or English.
- Existing FollowUp, Opportunity, Member360 and Reception commands remain on their accepted APIs, with receipt recovery and software/hardware boundaries intact.

Local Chromium review covers responsive light/dark screens, keyboard, failures, denial, retry and the existing end-to-end synthetic workflows. The candidate was not deployed or automatically merged. Reservation and notification account surfaces remain gated by their owning contracts.
