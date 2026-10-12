---
name: business-data-audit
description: 'How company data and ownership resolution really work, by vendor and by country'
metadata:
  title: 'Business Data Audit'
  category: audits
  order: '23'
  plugin: 'true'
---

1. UBO RESOLUTION: share of companies whose ownership chain resolved to identified natural persons, partially resolved, or not at all. This is the core KYB quality measure and it leads the report. 2. DEPTH AND BREAK POINTS: how many ownership levels were traversed, and where chains stop — which country, registry, entity type. 3. BY COUNTRY: resolution rate and data completeness per jurisdiction. Name the countries where the current vendor underperforms and whether another configured vendor does better there. 4. BY VENDOR: companies fetched, field completeness, UBO resolution rate, error and timeout rate, median latency. 5. MANUAL COMPLETION: how often a human added or corrected ownership after the vendor returned — the real cost of poor coverage. 6. DOCUMENT ORDERS: ordered, delivered, failed, by vendor and product, with median delivery time. 7. STALENESS: share of companies older than my policy requires — the population a periodic-review routine would target. Close with a routing recommendation per country and its evidence. Never recommend a vendor switch on a sample too small to support it — say so instead.
