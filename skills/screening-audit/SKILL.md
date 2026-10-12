---
name: screening-audit
description: 'What your AML screening produces, how much is noise, and which lever fixes it'
metadata:
  title: 'Screening Audit'
  category: audits
  order: '20'
  plugin: 'true'
---

1. VOLUME AND SHAPE: searches run, and the distribution of hits per search — not the average. Share of searches with 0, 1-5, 6-20, 21-50, 50+ hits, and which entity types generate the largest counts. 2. OUTCOME: confirmed, dismissed, undecided, with the true-positive rate, broken down by list type — the tuning lever differs per list. 3. AI COVERAGE AND AGREEMENT: what share of hits the AI analysed, and where it did, how often the human agreed. Three separate numbers: AI said false positive and the human agreed; AI said false positive and the human disagreed; no AI analysis at all. The third is a configuration gap, not a workload. 4. THRESHOLD EVIDENCE: relate the match score to the outcome. High-scoring hits routinely dismissed means matching is too loose; low-scoring hits routinely confirmed means too tight. State which, or state that the data does not support either. 5. REPEAT NOISE: the same subject returning the same dismissed hit on every re-screen. 6. ONGOING MONITORING: separate monitoring hits from initial screening and give their rates separately — mixing them misleads. 7. VENDOR: if more than one is in use, compare hits per search and true-positive rate on comparable populations. 8. BACKLOG: undecided hits by age, oldest first. Close with the two or three configuration changes the data supports, each with its number and the detection risk it carries. Never recommend narrowing a list or raising a threshold without naming that risk.
