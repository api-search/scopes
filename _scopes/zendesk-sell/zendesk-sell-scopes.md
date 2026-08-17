---
api_specs:
- filename: zendesk-sell.postman_collection.json
  format: json
  label: Zendesk Sell (Sales CRM) API
  slug: sales-crm-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/zendesk-sell/refs/heads/main/collections/zendesk-sell.postman_collection.json
- filename: zendesk-sell-contacts-api-openapi.yml
  format: yaml
  label: Zendesk Sell Contacts API
  slug: zendesk-sell-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zendesk-sell/refs/heads/main/openapi/zendesk-sell-contacts-api-openapi.yml
- filename: zendesk-sell-deals-api-openapi.yml
  format: yaml
  label: Zendesk Sell Deals API
  slug: zendesk-sell-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zendesk-sell/refs/heads/main/openapi/zendesk-sell-deals-api-openapi.yml
- filename: zendesk-sell-leads-api-openapi.yml
  format: yaml
  label: Zendesk Sell Leads API
  slug: zendesk-sell-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zendesk-sell/refs/heads/main/openapi/zendesk-sell-leads-api-openapi.yml
authorization_urls:
- https://api.getbase.com/oauth2/authorize
description: ''
docs: https://developer.zendesk.com/api-reference/sales-crm/authentication/introduction/
flows:
- authorizationCode
- implicit
- password
kind: oauth-scopes
layout: scope
method: searched
name: Zendesk Sell Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Zendesk Sell publishes 3 OAuth 2.0 scopes via the authorizationCode, implicit, and password flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Zendesk Sell API on a user''s behalf.


  Tokens are issued from https://api.getbase.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Zendesk Sell
provider_slug: zendesk-sell
schemes:
- description: OAuth 2.0 (authorization code, implicit, password, and refresh token grants).
  flows:
  - authorizationUrl: https://api.getbase.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.getbase.com/oauth2/token
  - authorizationUrl: https://api.getbase.com/oauth2/authorize
    flow: implicit
  - flow: password
    tokenUrl: https://api.getbase.com/oauth2/token
  name: oauth2
  source: openapi/_original/zendesk-sell-openapi.yml
scope_count: 3
scope_names:
- read
- write
- profile
scopes:
- description: '"Grant read-only access to all your data, except for the account and user info."'
  flows:
  - authorizationCode
  - implicit
  - password
  scope: read
- description: Write access to all your data, except for the account and user info.
  flows:
  - authorizationCode
  - implicit
  - password
  scope: write
- description: Read-only access to account and user information.
  flows:
  - authorizationCode
  - implicit
  - password
  scope: profile
slug: zendesk-sell-scopes
source_filename: zendesk-sell-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/_original/zendesk-sell-openapi.yml\ndocs: https://developer.zendesk.com/api-reference/sales-crm/authentication/introduction/\nreference: https://developer.zendesk.com/api-reference/sales-crm/authentication/reference/\nschemes:\n- name: oauth2\n  source: openapi/_original/zendesk-sell-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.getbase.com/oauth2/authorize\n    tokenUrl: https://api.getbase.com/oauth2/token\n  - flow: implicit\n    authorizationUrl: https://api.getbase.com/oauth2/authorize\n  - flow: password\n    tokenUrl: https://api.getbase.com/oauth2/token\n  description: >-\n    OAuth 2.0 (authorization code, implicit, password, and refresh token grants).\nscope_count: 3\nscopes:\n- scope: read\n  description: >-\n    \"Grant read-only access to all your data, except for the account and user info.\"\n  flows: [authorizationCode, implicit, password]\n  sources:\n  - https://developer.zendesk.com/api-reference/sales-crm/authentication/introduction/\n\
  \  - openapi/_original/zendesk-sell-openapi.yml\n- scope: write\n  description: >-\n    Write access to all your data, except for the account and user info.\n  flows: [authorizationCode, implicit, password]\n  sources:\n  - https://developer.zendesk.com/api-reference/sales-crm/authentication/introduction/\n  - openapi/_original/zendesk-sell-openapi.yml\n- scope: profile\n  description: >-\n    Read-only access to account and user information.\n  flows: [authorizationCode, implicit, password]\n  sources:\n  - https://developer.zendesk.com/api-reference/sales-crm/authentication/introduction/\n  note: >-\n    Documented by Zendesk but ABSENT from the OpenAPI in openapi/ — found by reading the\n    authentication docs, not the spec.\ngranularity: coarse\ngranularity_note: >-\n  Three account-wide scopes only. There is no per-resource or per-verb scoping (no\n  read:leads / write:deals), so any token that can write a note can also delete every deal.\n  `insufficient_scope` (HTTP 403) is the\
  \ error returned when a token lacks the scope.\nx-evidence:\n- url: https://developer.zendesk.com/api-reference/sales-crm/authentication/introduction/\n  status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zendesk-sell/refs/heads/main/scopes/zendesk-sell-scopes.yml
summary_line: 3 scopes · authorizationCode/implicit/password
tags:
- CRM
- Sales
- Sales Automation
- Leads
- Deals
- Pipeline
- Customer Experience
token_urls:
- https://api.getbase.com/oauth2/token
---
