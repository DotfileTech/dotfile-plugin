---
name: document-audit
description: 'How document collection and review really perform: AI coverage, forensics value, and configuration faults'
metadata:
  title: 'Document Audit'
  category: audits
  order: '22'
  plugin: 'true'
---

1. COVERAGE: documents received, analysed by AI, reviewed by a human, as a share per type. Name types where AI review is available but never used, and types where AI runs but always defers to a human — the second is a cost with no benefit. 2. OUTCOME BY TYPE: approved, rejected, awaiting, and the rejection rate; then the worst types and the top rejection reasons behind each, taken from review comments rather than inferred. 3. RE-REQUEST LOOPS: types needing two or more rounds, with the count and the median added delay. The usual fix is the portal instruction, not the check. 4. EXTRACTION FAILURES: documents where extraction produced nothing usable, forcing manual review, per type. 5. DOCUMENT FORENSICS: whether it is enabled, on which types, its finding rate, and — the question that matters — how often a finding actually changed the outcome. If it never changes an outcome, it is paid noise; say so. 6. EXPIRY COVERAGE: share of approved documents with no expiration date, which is silent staleness. 7. CONFIGURATION FAULTS: types defined and never used, types with neither AI review nor forensics, types where the requested and received document routinely differ. Close with three changes, each with its number, and separate a collection problem (the client sends the wrong thing) from a quality problem (unreadable) from a configuration problem (we asked for the wrong thing) — different fixes, different owners.
