---
api_specs:
- filename: clockrook-account-api-openapi.yml
  format: yaml
  label: Clockrook Account API
  slug: clockrook-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clockrook/openapi/clockrook-account-api-openapi.yml
- filename: clockrook-accounts-api-openapi.yml
  format: yaml
  label: Clockrook Accounts API
  slug: clockrook-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clockrook/openapi/clockrook-accounts-api-openapi.yml
- filename: clockrook-jobs-api-openapi.yml
  format: yaml
  label: Clockrook Jobs API
  slug: clockrook-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clockrook/openapi/clockrook-jobs-api-openapi.yml
- filename: clockrook-pricing-api-openapi.yml
  format: yaml
  label: Clockrook Pricing API
  slug: clockrook-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clockrook/openapi/clockrook-pricing-api-openapi.yml
- filename: clockrook-usage-api-openapi.yml
  format: yaml
  label: Clockrook Usage API
  slug: clockrook-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clockrook/openapi/clockrook-usage-api-openapi.yml
authorization_urls: []
description: ''
docs: https://clockrook.com/.well-known/api-onboarding
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Clockrook Scopes
name_suffix: OAuth Scopes
note: '"API keys are not scoped. OAuth tokens carry these scopes and work only on this site." (api-onboarding). The OpenAPI declares no oauth2 scheme, so scopes are not mapped to operations.'
overview: 'Clockrook publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Clockrook API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Clockrook
provider_slug: clockrook
schemes: []
scope_count: 3
scope_names:
- jobs:read
- jobs:manage
- account:read
scopes:
- description: Listed in scopes_supported; no per-scope description is published.
  flows: []
  scope: jobs:read
- description: Listed in scopes_supported; no per-scope description is published.
  flows: []
  scope: jobs:manage
- description: Listed in scopes_supported; no per-scope description is published.
  flows: []
  scope: account:read
slug: clockrook-scopes
source_filename: clockrook-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: searched\nsource: https://clockrook.com/.well-known/oauth-authorization-server\ndocs: https://clockrook.com/.well-known/api-onboarding\nscopes:\n- name: jobs:read\n  description: Listed in scopes_supported; no per-scope description is published.\n- name: jobs:manage\n  description: Listed in scopes_supported; no per-scope description is published.\n- name: account:read\n  description: Listed in scopes_supported; no per-scope description is published.\nnote: '\"API keys are not scoped. OAuth tokens carry these scopes and work only on this site.\" (api-onboarding). The OpenAPI declares no oauth2 scheme, so scopes are not mapped to operations.'\n"
source_yaml_url: https://artifacts.apis.io/clockrook/scopes/clockrook-scopes.yml
summary_line: 3 scopes
tags:
- Company
- Scheduling
- Cron
- Job
- AI Agents
- Webhook
- Uptime Monitoring
- MCP
token_bound: false
token_urls: []
---
