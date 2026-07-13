---
api_specs:
- filename: regions-open-banking-openapi.yml
  format: yaml
  label: Regions Open Banking API
  slug: regions-open-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regions-financial/refs/heads/main/openapi/regions-open-banking-openapi.yml
authorization_urls:
- https://auth.regions.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Regions Financial Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'regions-financial publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the regions-financial API on a user''s behalf.


  Tokens are issued from https://auth.regions.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: regions-financial
provider_slug: regions-financial
schemes:
- description: OAuth 2.0 with customer consent (FDX standard)
  flows:
  - authorizationUrl: https://auth.regions.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://auth.regions.com/oauth/token
  name: OAuth2
  source: openapi/regions-open-banking-openapi.yml
scope_count: 4
scope_names:
- accounts:read
- customers:read
- payments:write
- transactions:read
scopes:
- description: Read account information
  flows:
  - authorizationCode
  scope: accounts:read
- description: Read customer profile
  flows:
  - authorizationCode
  scope: customers:read
- description: Initiate payments
  flows:
  - authorizationCode
  scope: payments:write
- description: Read transaction history
  flows:
  - authorizationCode
  scope: transactions:read
slug: regions-financial-scopes
source_filename: regions-financial-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/regions-open-banking-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/regions-open-banking-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.regions.com/oauth/authorize\n    tokenUrl: https://auth.regions.com/oauth/token\n  description: OAuth 2.0 with customer consent (FDX standard)\nscopes:\n- scope: accounts:read\n  description: Read account information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/regions-open-banking-openapi.yml\n- scope: customers:read\n  description: Read customer profile\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/regions-open-banking-openapi.yml\n- scope: payments:write\n  description: Initiate payments\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/regions-open-banking-openapi.yml\n- scope: transactions:read\n  description: Read transaction history\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/regions-open-banking-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/regions-financial/refs/heads/main/scopes/regions-financial-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Banking
- Financial Services
- Open Banking
- FDX
- Consumer Banking
- Wealth Management
- Fortune 500
token_urls:
- https://auth.regions.com/oauth/token
---
