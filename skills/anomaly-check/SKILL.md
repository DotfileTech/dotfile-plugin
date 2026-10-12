---
name: anomaly-check
description: 'What moved in this workspace recently'
metadata:
  title: 'Trends'
  category: queue
  order: '5'
  plugin: 'true'
---

An anomaly is a number that MOVED, not one that is high. 1. Baseline: show_analytic_widget with cases created per day over the recent weeks — compare the last 7 days to the daily average of the weeks before. 2. Distributions, not totals: show_analytic_widget breakdowns of cases by risk and by assignee, checks by type and by status. The signal is a shift in the mix. 3. To compare two periods, call query_entities with perPage 1 and read the total, twice, with the two date ranges. NEVER paginate to count. 4. At most 5 findings: what moved with both numbers and periods; whether this is normal variation at these volumes; the likely cause only if data supports it; what to look at, linked. 5. A mandatory 'what I could not check' section. If nothing moved, say Nothing abnormal, add the blind spots, stop.
