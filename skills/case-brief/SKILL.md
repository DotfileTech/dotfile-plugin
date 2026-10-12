---
name: case-brief
description: 'Where this case stands: what is done, what blocks it, and the single next action'
metadata:
  title: 'Case Brief'
  category: cases
  order: '7'
  plugin: 'true'
---

No case in context: ask which case, or find it with query_entities, before anything else. 1. Start from the case context, then query_entities on checks, with a case__default__id rule for this case since it reads the whole workspace, and get_check on every check that is not approved, so you read the real result and any review comment. 2. list_case_controls and list_notes. 3. Report: status, risk, template, assignee on one line; what is done; what is blocking — each non-approved check with type, entity, status and the concrete reason from its result, cited not paraphrased, then each incomplete manual control; what is missing that nobody has requested; one next action and who must do it. Link every entity you name. If the next step is a human decision, say so — never invent an escalation path you have no tool for.
