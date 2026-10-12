---
name: team-load
description: 'How the open workload is spread across the team right now'
metadata:
  title: 'Team Load'
  category: queue
  order: '8'
  plugin: 'true'
---

1. show_analytic_widget with open cases broken down by assignee, then by risk. 2. show_analytic_widget with the checks pending review broken down by type. 3. Per member, an exact count of open cases: query_entities with perPage 1, read the total, never paginate. Same for unassigned. 4. Report open cases per member split by risk, the unassigned pile, the review queue by type. Name who carries the most high-and-above risk, not who holds the most cases. 5. State what you cannot see: how much each person processed, how fast, when they last touched their cases. Do not infer productivity from case counts.
