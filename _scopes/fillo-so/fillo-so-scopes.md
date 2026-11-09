---
api_specs:
- filename: fillo-so-agents-api-openapi.yml
  format: yaml
  label: Fillo Agents API
  slug: fillo-so-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-agents-api-openapi.yml
- filename: fillo-so-credentials-api-openapi.yml
  format: yaml
  label: Fillo Credentials API
  slug: fillo-so-credentials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-credentials-api-openapi.yml
- filename: fillo-so-deliveries-api-openapi.yml
  format: yaml
  label: Fillo Deliveries API
  slug: fillo-so-deliveries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-deliveries-api-openapi.yml
- filename: fillo-so-fillo-management-api-api-openapi.yml
  format: yaml
  label: Fillo Fillo Management API
  slug: fillo-so-fillo-management-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-fillo-management-api-api-openapi.yml
- filename: fillo-so-forms-api-openapi.yml
  format: yaml
  label: Fillo Forms API
  slug: fillo-so-forms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-forms-api-openapi.yml
- filename: fillo-so-insights-api-openapi.yml
  format: yaml
  label: Fillo Insights API
  slug: fillo-so-insights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-insights-api-openapi.yml
- filename: fillo-so-integrations-api-openapi.yml
  format: yaml
  label: Fillo Integrations API
  slug: fillo-so-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-integrations-api-openapi.yml
- filename: fillo-so-members-api-openapi.yml
  format: yaml
  label: Fillo Members API
  slug: fillo-so-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-members-api-openapi.yml
- filename: fillo-so-respondents-api-openapi.yml
  format: yaml
  label: Fillo Respondents API
  slug: fillo-so-respondents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-respondents-api-openapi.yml
- filename: fillo-so-responses-api-openapi.yml
  format: yaml
  label: Fillo Responses API
  slug: fillo-so-responses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-responses-api-openapi.yml
- filename: fillo-so-settings-api-openapi.yml
  format: yaml
  label: Fillo Settings API
  slug: fillo-so-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-settings-api-openapi.yml
- filename: fillo-so-storage-api-openapi.yml
  format: yaml
  label: Fillo Storage API
  slug: fillo-so-storage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-storage-api-openapi.yml
- filename: fillo-so-webhooks-api-openapi.yml
  format: yaml
  label: Fillo Webhooks API
  slug: fillo-so-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-webhooks-api-openapi.yml
- filename: fillo-so-workspace-api-openapi.yml
  format: yaml
  label: Fillo Workspace API
  slug: fillo-so-workspace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-workspace-api-openapi.yml
authorization_urls: []
description: ''
docs: https://fillo.so/docs/api#scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Fillo So Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Fillo publishes 17 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Fillo API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Fillo
provider_slug: fillo-so
schemes: []
scope_count: 17
scope_names:
- forms:read
- responses:read
- responses:export
- respondents:read
- forms:write
- forms:publish
- storage:manage
- webhooks:manage
- settings:manage
- integrations:manage
- responses:manage
- members:manage
- workspace:manage
- forms:delete
- responses:delete
- respondents:delete
- workspace:delete
scopes:
- description: List forms and versions; read a form's published schema and settings.
  flows: []
  scope: forms:read
- description: List, read, and summarize responses, including one respondent's history. Insights quotes answers back, so it needs this as well as forms:read.
  flows: []
  scope: responses:read
- description: Export a form's responses as CSV.
  flows: []
  scope: responses:export
- description: Look up living respondent profiles.
  flows: []
  scope: respondents:read
- description: Create and edit a form's schema; rename, duplicate, unpublish, discard staged changes, and change the settings that live in the schema (submit copy, redirect, progress bar).
  flows: []
  scope: forms:write
- description: Take a form's staged changes live.
  flows: []
  scope: forms:publish
- description: Connect and disconnect the workspace's upload destinations, and choose where a form's uploads land (including its Google Drive folder).
  flows: []
  scope: storage:manage
- description: List, add, update, and remove a form's signed webhooks.
  flows: []
  scope: webhooks:manage
- description: Read and patch a form's operational settings. The six presentation keys live in the schema and additionally need forms:write.
  flows: []
  scope: settings:manage
- description: Turn a form's Sheets, Notion, HubSpot, or Slack destination on or off, choose the account a project uses, and manage connected accounts.
  flows: []
  scope: integrations:manage
- description: Read held submissions and drafts, release held submissions, and retry or re-send deliveries.
  flows: []
  scope: responses:manage
- description: List members and invitations, change a role, and remove a member.
  flows: []
  scope: members:manage
- description: Rename the workspace or project and manage sync tokens, connector tokens, code-sync policy, allowed origins, identity verification, and agent access.
  flows: []
  scope: workspace:manage
- description: Delete a form with its responses and files.
  flows: []
  scope: forms:delete
- description: Delete a response and its uploaded files.
  flows: []
  scope: responses:delete
- description: Forget a respondent, optionally with every response they submitted.
  flows: []
  scope: respondents:delete
- description: Schedule the workspace itself for deletion.
  flows: []
  scope: workspace:delete
slug: fillo-so-scopes
source_filename: fillo-so-scopes.yml
source_heading: OAuth Scopes
source_url: https://fillo.so/docs/api
source_yaml: "generated: '2026-11-07'\nmethod: searched\nsource: https://fillo.so/docs/api#scopes\nsources:\n- https://fillo.so/docs/api\ndocs: https://fillo.so/docs/api#scopes\nsummary:\n  model: project-secret-key\n  presets:\n    read: [forms:read, responses:read, respondents:read]\n    agent: [forms:read, responses:read, respondents:read, forms:write, forms:publish, responses:export]\n    full: all scopes except the three delete scopes\n  delete_tier: [responses:delete, forms:delete, respondents:delete, workspace:delete]\nscopes:\n- name: forms:read\n  description: List forms and versions; read a form's published schema and settings.\n- name: responses:read\n  description: List, read, and summarize responses, including one respondent's history. Insights quotes answers back, so it needs this as well as forms:read.\n- name: responses:export\n  description: Export a form's responses as CSV.\n- name: respondents:read\n  description: Look up living respondent profiles.\n- name: forms:write\n\
  \  description: Create and edit a form's schema; rename, duplicate, unpublish, discard staged changes, and change the settings that live in the schema (submit copy, redirect, progress bar).\n- name: forms:publish\n  description: Take a form's staged changes live.\n- name: storage:manage\n  description: Connect and disconnect the workspace's upload destinations, and choose where a form's uploads land (including its Google Drive folder).\n- name: webhooks:manage\n  description: List, add, update, and remove a form's signed webhooks.\n- name: settings:manage\n  description: Read and patch a form's operational settings. The six presentation keys live in the schema and additionally need forms:write.\n- name: integrations:manage\n  description: Turn a form's Sheets, Notion, HubSpot, or Slack destination on or off, choose the account a project uses, and manage connected accounts.\n- name: responses:manage\n  description: Read held submissions and drafts, release held submissions, and retry or\
  \ re-send deliveries.\n- name: members:manage\n  description: List members and invitations, change a role, and remove a member.\n- name: workspace:manage\n  description: Rename the workspace or project and manage sync tokens, connector tokens, code-sync policy, allowed origins, identity verification, and agent access.\n- name: forms:delete\n  description: Delete a form with its responses and files.\n- name: responses:delete\n  description: Delete a response and its uploaded files.\n- name: respondents:delete\n  description: Forget a respondent, optionally with every response they submitted.\n- name: workspace:delete\n  description: Schedule the workspace itself for deletion.\n"
source_yaml_url: https://artifacts.apis.io/fillo-so/scopes/fillo-so-scopes.yml
summary_line: 17 scopes
tags:
- Forms
- Form Builder
- Developer Tools
- Embeddable Widgets
- Webhooks
- Validation
- File Uploads
- SDK
- CLI
- Management API
token_bound: false
token_urls: []
---
