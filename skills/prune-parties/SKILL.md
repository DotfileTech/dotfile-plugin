---
name: prune-parties
description: 'Propose which parties are out of scope, with a reason and the threshold applied'
metadata:
  title: 'Prune Parties'
  category: cases
  order: '15'
  plugin: 'true'
---

No case in context: ask which case, or find it with query_entities, before anything else. 1. List every individual and company with role and ownership percentage. 2. Propose which are out of scope: below the ownership threshold, non-controlling roles, duplicates. 3. One-line reason each, and state the threshold you applied. 4. Flag separately anyone you are unsure about rather than defaulting to excluding them, and never mark anything without my confirmation.
