---
name: onboarding-status
description: 'Where this workspace stands in its setup, what blocks progress, and the next action'
metadata:
  title: 'Onboarding Status'
  category: configuration
  order: '25'
  plugin: 'true'
---

1. Read the configuration: templates and rules, checks and controls per template, document types, custom properties, portals, enabled check types and vendor credentials, AI review policy, users and roles, webhooks and API keys. 2. Score it stage by stage against a complete setup: entities and templates defined; checks wired per entity type; a live collection channel (portal or API); review policy set; risk configured; team and permissions; integration and notifications. For each stage say done, partial or not started — and for partial, exactly what is missing. 3. Then verify it works rather than merely exists: has each template ever been applied, has each portal received a submission, has each check type ever run, has anything ever been approved. Configured but never exercised is not done. 4. Report the stage we are on, the three things blocking progress in order, and the single next action with who owns it — us or the customer. 5. Name anything configured in a way that will cause trouble later: a portal with no template, a control nobody can complete, a check type enabled without vendor credentials, auto-approval on with no risk rules. Keep it to one screen. This gets run repeatedly — if I give you the previous state, lead with what changed.
