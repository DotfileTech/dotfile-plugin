---
name: refresh-company
description: 'Re-purchase company data and report only what changed'
metadata:
  title: 'Refresh Business Data'
  category: cases
  order: '14'
  plugin: 'true'
---

No company in context: ask which company, or find it with query_entities, before anything else. 1. buy_company_data — every call is a real billed purchase with no dedup, so check how recent the current data is and skip if fresh enough, saying so. 2. get_company_data_changes: a free deterministic diff of the two latest snapshots. 3. Report only what changed: legal form, status, share capital, directors, ownership, address, registration. 4. Add a note to the case with the diff. 5. If a director, owner or legal status changed, call it material and recommend re-running the affected checks — do not launch them without asking.
