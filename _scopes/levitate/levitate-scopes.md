---
api_specs:
- filename: levitate-companies-api-openapi.yml
  format: yaml
  label: Levitate Companies API
  slug: levitate-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/levitate/refs/heads/main/openapi/levitate-companies-api-openapi.yml
- filename: levitate-contacts-api-openapi.yml
  format: yaml
  label: Levitate Contacts API
  slug: levitate-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/levitate/refs/heads/main/openapi/levitate-contacts-api-openapi.yml
- filename: levitate-notes-api-openapi.yml
  format: yaml
  label: Levitate Notes API
  slug: levitate-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/levitate/refs/heads/main/openapi/levitate-notes-api-openapi.yml
authorization_urls:
- https://login.levitate.ai/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Levitate Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Levitate publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Levitate API on a user''s behalf.


  Tokens are issued from https://login.levitate.ai/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Levitate
provider_slug: levitate
schemes:
- description: Levitate OAuth2 Authorization Flow
  flows:
  - authorizationUrl: https://login.levitate.ai/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.levitate.ai/oauth2/token
  name: OAuth2
  source: openapi/levitate-public-v1-openapi.json
scope_count: 2
scope_names:
- levitate:campaigns
- levitate:contacts
scopes:
- description: Access Levitate campaigns and related operations
  flows:
  - authorizationCode
  scope: levitate:campaigns
- description: Access Levitate contacts and related operations
  flows:
  - authorizationCode
  scope: levitate:contacts
slug: levitate-scopes
source_filename: levitate-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: derived\nsource: openapi/levitate-public-v1-openapi.json\nschemes:\n- name: OAuth2\n  source: openapi/levitate-public-v1-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.levitate.ai/oauth2/authorize\n    tokenUrl: https://login.levitate.ai/oauth2/token\n  description: Levitate OAuth2 Authorization Flow\nscopes:\n- scope: levitate:campaigns\n  description: Access Levitate campaigns and related operations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/levitate-public-v1-openapi.json\n- scope: levitate:contacts\n  description: Access Levitate contacts and related operations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/levitate-public-v1-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/levitate/refs/heads/main/scopes/levitate-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- relationship-marketing
- CRM
- Email Marketing
- Contacts
- Small Business
- Insurance
- Financial-Services
- Non-Profit
- Marketing Automation
- MCP
- agent-native
- Software-as-a-Service
token_urls:
- https://login.levitate.ai/oauth2/token
---
