---
api_specs:
- filename: zendesk-sell-openapi.yml
  format: yaml
  label: Zendesk Sell (Sales CRM) API
  slug: sales-crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zendesk-sell/refs/heads/main/openapi/zendesk-sell-openapi.yml
authorization_urls:
- https://api.getbase.com/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Zendesk Sell Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Zendesk Sell publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Zendesk Sell API on a user''s behalf.


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
  name: oauth2
  source: openapi/zendesk-sell-openapi.yml
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read access to Sell data
  flows:
  - authorizationCode
  scope: read
- description: Write access to Sell data
  flows:
  - authorizationCode
  scope: write
slug: zendesk-sell-scopes
source_filename: zendesk-sell-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zendesk-sell-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/zendesk-sell-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.getbase.com/oauth2/authorize\n    tokenUrl: https://api.getbase.com/oauth2/token\n  description: OAuth 2.0 (authorization code, implicit, password, and refresh token grants).\nscopes:\n- scope: read\n  description: Read access to Sell data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zendesk-sell-openapi.yml\n- scope: write\n  description: Write access to Sell data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zendesk-sell-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zendesk-sell/refs/heads/main/scopes/zendesk-sell-scopes.yml
summary_line: 2 scopes · authorizationCode
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
