---
api_specs:
- filename: amdocs-connectx-openapi.yml
  format: yaml
  label: Amdocs connectX BSS API
  slug: amdocs-connectx-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amdocs/refs/heads/main/openapi/amdocs-connectx-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Amdocs Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Amdocs publishes 4 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Amdocs API on a user''s behalf.


  Tokens are issued from https://auth.amdocs-dbs.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Amdocs
provider_slug: amdocs
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.amdocs-dbs.com/oauth/token
  name: oauth2
  source: openapi/amdocs-connectx-openapi.yml
scope_count: 4
scope_names:
- read:billing
- read:customers
- write:customers
- write:subscriptions
scopes:
- description: Read billing data
  flows:
  - clientCredentials
  scope: read:billing
- description: Read customer data
  flows:
  - clientCredentials
  scope: read:customers
- description: Manage customers
  flows:
  - clientCredentials
  scope: write:customers
- description: Manage subscriptions
  flows:
  - clientCredentials
  scope: write:subscriptions
slug: amdocs-scopes
source_filename: amdocs-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amdocs-connectx-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/amdocs-connectx-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.amdocs-dbs.com/oauth/token\nscopes:\n- scope: read:billing\n  description: Read billing data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/amdocs-connectx-openapi.yml\n- scope: read:customers\n  description: Read customer data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/amdocs-connectx-openapi.yml\n- scope: write:customers\n  description: Manage customers\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/amdocs-connectx-openapi.yml\n- scope: write:subscriptions\n  description: Manage subscriptions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/amdocs-connectx-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amdocs/refs/heads/main/scopes/amdocs-scopes.yml
summary_line: 4 scopes · clientCredentials
tags:
- Telecom
- BSS
- OSS
- Billing
- Customer Management
- MVNO
- 5G
- SaaS
token_urls:
- https://auth.amdocs-dbs.com/oauth/token
---
