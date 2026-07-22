---
authorization_urls: []
description: ''
docs: https://docs.runtm.com/cloud-api/scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Runtime Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Runtime publishes 20 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Runtime API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Runtime
provider_slug: runtime
schemes: []
scope_count: 20
scope_names:
- sessions:read
- sessions:write
- sessions:delete
- sessions:prompt
- sessions:terminal
- context:read
- context:write
- secrets:read
- secrets:write
- deployments:read
- deployments:write
- templates:read
- templates:write
- templates:build
- templates:delete
- integrations:read
- integrations:write
- guardrails:read
- guardrails:write
- activity:read
scopes:
- description: List and view sessions
  flows: []
  scope: sessions:read
- description: Create, pause, resume, rename sessions
  flows: []
  scope: sessions:write
- description: Destroy sessions
  flows: []
  scope: sessions:delete
- description: Send prompts and cancel them
  flows: []
  scope: sessions:prompt
- description: WebSocket terminal access
  flows: []
  scope: sessions:terminal
- description: Read instructions, skills, directives
  flows: []
  scope: context:read
- description: Update instructions, manage skills
  flows: []
  scope: context:write
- description: List secret names (values are never returned)
  flows: []
  scope: secrets:read
- description: Set and delete secrets
  flows: []
  scope: secrets:write
- description: View deploy info and limits
  flows: []
  scope: deployments:read
- description: Run deploys
  flows: []
  scope: deployments:write
- description: List and view templates
  flows: []
  scope: templates:read
- description: Create and update templates
  flows: []
  scope: templates:write
- description: Trigger template builds
  flows: []
  scope: templates:build
- description: Delete templates
  flows: []
  scope: templates:delete
- description: View integrations
  flows: []
  scope: integrations:read
- description: Manage integrations
  flows: []
  scope: integrations:write
- description: View org guardrails
  flows: []
  scope: guardrails:read
- description: Update org guardrails
  flows: []
  scope: guardrails:write
- description: View telemetry and usage
  flows: []
  scope: activity:read
slug: runtime-scopes
source_filename: runtime-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.runtm.com/cloud-api/scopes\ndocs: https://docs.runtm.com/cloud-api/scopes\nnotes: >-\n  Runtime uses API-key scopes (not OAuth), following the pattern `resource:action`. Every key carries\n  a set of scopes that determine which endpoints it can call, bounded by the creating user's org role\n  ceiling. Captured verbatim from the published scope reference.\nmodel: api-key-scopes\nscheme:\n  name: BearerApiKey\n  pattern: \"resource:action\"\n  enforcement: \"403 Insufficient scope: requires <scope> when a key lacks a required scope\"\n  runtime_check: \"GET /api/cloud/auth/verify returns a scopes[] array\"\nscopes:\n- scope: sessions:read\n  description: List and view sessions\n- scope: sessions:write\n  description: Create, pause, resume, rename sessions\n- scope: sessions:delete\n  description: Destroy sessions\n- scope: sessions:prompt\n  description: Send prompts and cancel them\n- scope: sessions:terminal\n\
  \  description: WebSocket terminal access\n- scope: context:read\n  description: Read instructions, skills, directives\n- scope: context:write\n  description: Update instructions, manage skills\n- scope: secrets:read\n  description: List secret names (values are never returned)\n- scope: secrets:write\n  description: Set and delete secrets\n- scope: deployments:read\n  description: View deploy info and limits\n- scope: deployments:write\n  description: Run deploys\n- scope: templates:read\n  description: List and view templates\n- scope: templates:write\n  description: Create and update templates\n- scope: templates:build\n  description: Trigger template builds\n- scope: templates:delete\n  description: Delete templates\n- scope: integrations:read\n  description: View integrations\n- scope: integrations:write\n  description: Manage integrations\n- scope: guardrails:read\n  description: View org guardrails\n- scope: guardrails:write\n  description: Update org guardrails\n- scope: activity:read\n\
  \  description: View telemetry and usage\npresets:\n- name: Session automation\n  scopes: [sessions:read, sessions:write, sessions:delete, sessions:prompt, sessions:terminal, context:read, secrets:read]\n- name: Full access\n  scopes: [all]\n- name: Read-only\n  scopes: [sessions:read, context:read, secrets:read, deployments:read, templates:read, integrations:read, guardrails:read, activity:read]\nrole_ceilings:\n- role: Member\n  ceiling: \"Any scope for member-accessible resources; cannot grant guardrails:write or templates:delete\"\n- role: Admin\n  ceiling: \"All scopes except owner-reserved\"\n- role: Owner\n  ceiling: \"No restrictions\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runtime/refs/heads/main/scopes/runtime-scopes.yml
summary_line: 20 scopes
tags:
- Company
- Coding Agents
- Developer Tools
- AI Infrastructure
- Sandboxes
- Agent Orchestration
- DevOps
- Cloud
token_urls: []
---
