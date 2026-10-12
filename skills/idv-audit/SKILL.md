---
name: idv-audit
description: 'IDV, ID document and eKYC performance end to end, with a fair vendor comparison'
metadata:
  title: 'Identity Verification Audit'
  category: audits
  order: '21'
  plugin: 'true'
---

METHOD, and state it in the output — the naive version of this comparison is usually wrong. Exclude batch-created checks: bulk re-verification campaigns measure outreach, not vendor quality, so detect them (many created in one or two days, most never engaged) and report them separately. Count only checks old enough to have completed, and only the latest attempt per check. When vendors have different tenure, compare at equal cohort age — approval within 1 hour, 24 hours, 7 days, 14 days side by side, not final rates. Segment by how old the case was when the check was created: population mix usually moves the numbers more than the vendor. REPORT: 1. The funnel per check type — created, never started, started, completed, auto-approved, human-approved, vendor-declined. 2. The two metrics that decide it: straight-through rate, and how often a human overruled a vendor decline. 3. Median and 90th-percentile time to approval. 4. Never-started rate — a drop-off before the subject begins, so a portal problem, not a vendor one. 5. Retry behaviour: attempts per check, and whether a retry usually succeeds. If it does, a first failure is a usability problem, not a fraud signal. 6. Where failures concentrate: document type, issuing country, verification mode. 7. Where both eKYC and IDV run on comparable people, which performs better. 8. EXPOSURE: approved identity documents already expired or expiring within 90 days. Close with a recommendation per check type, and say plainly when a difference is inside noise.
