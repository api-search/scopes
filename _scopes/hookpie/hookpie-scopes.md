---
api_specs:
- filename: hookpie-account-api-openapi.yml
  format: yaml
  label: Hookpie Account API
  slug: hookpie-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hookpie/openapi/hookpie-account-api-openapi.yml
- filename: hookpie-accounts-api-openapi.yml
  format: yaml
  label: Hookpie Accounts API
  slug: hookpie-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hookpie/openapi/hookpie-accounts-api-openapi.yml
- filename: hookpie-i-api-openapi.yml
  format: yaml
  label: Hookpie I API
  slug: hookpie-i-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hookpie/openapi/hookpie-i-api-openapi.yml
- filename: hookpie-inboxes-api-openapi.yml
  format: yaml
  label: Hookpie Inboxes API
  slug: hookpie-inboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hookpie/openapi/hookpie-inboxes-api-openapi.yml
- filename: hookpie-pricing-api-openapi.yml
  format: yaml
  label: Hookpie Pricing API
  slug: hookpie-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hookpie/openapi/hookpie-pricing-api-openapi.yml
- filename: hookpie-usage-api-openapi.yml
  format: yaml
  label: Hookpie Usage API
  slug: hookpie-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hookpie/openapi/hookpie-usage-api-openapi.yml
authorization_urls: []
description: ''
docs: https://hookpie.com/.well-known/api-onboarding
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Hookpie Scopes
name_suffix: OAuth Scopes
note: Scopes are published in the RFC 8414 metadata (scopes_supported) and the api-onboarding descriptor; the OpenAPI declares only bearer API-key auth. The descriptor says "API keys are not scoped. OAuth tokens carry these scopes and work only on this site." No per-scope descriptions are published.
overview: 'Hookpie publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Hookpie API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hookpie
provider_slug: hookpie
schemes: []
scope_count: 3
scope_names:
- inbox:read
- inbox:manage
- account:read
scopes:
- description: ''
  flows: []
  scope: inbox:read
- description: ''
  flows: []
  scope: inbox:manage
- description: ''
  flows: []
  scope: account:read
slug: hookpie-scopes
source_filename: hookpie-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: searched\nsource: https://hookpie.com/.well-known/oauth-authorization-server\ndocs: https://hookpie.com/.well-known/api-onboarding\nnote: Scopes are published in the RFC 8414 metadata (scopes_supported) and the api-onboarding descriptor; the OpenAPI declares only bearer API-key auth. The descriptor says \"API keys are not scoped. OAuth tokens carry these scopes and work only on this site.\" No per-scope descriptions are published.\nscopes:\n- name: inbox:read\n  description: null\n- name: inbox:manage\n  description: null\n- name: account:read\n  description: null\n"
source_yaml_url: https://artifacts.apis.io/hookpie/scopes/hookpie-scopes.yml
summary_line: 3 scopes
tags:
- Company
- Webhook
- AI Agents
- MCP
- Event Inbox
- Developer Tools
- Pay-as-you-go
token_bound: false
token_urls: []
---
