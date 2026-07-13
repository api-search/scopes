---
api_specs:
- filename: civic-pass-customer-api.yaml
  format: yaml
  label: Civic Pass API
  slug: civic-pass-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/civic/refs/heads/main/openapi/civic-pass-customer-api.yaml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Civic Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Civic publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Civic API on a user''s behalf.


  Tokens are issued from https://auth0.civic.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Civic
provider_slug: civic
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth0.civic.com/oauth/token
  name: pass_auth
  source: openapi/civic-pass-customer-api.yaml
scope_count: 2
scope_names:
- read:token
- write:token
scopes:
- description: ''
  flows: []
  scope: read:token
- description: ''
  flows: []
  scope: write:token
slug: civic-scopes
source_filename: civic-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/civic-pass-customer-api.yaml\nschemes:\n- name: pass_auth\n  source: openapi/civic-pass-customer-api.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth0.civic.com/oauth/token\nscopes:\n- scope: read:token\n  sources:\n  - openapi/civic-pass-customer-api.yaml\n- scope: write:token\n  sources:\n  - openapi/civic-pass-customer-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/civic/refs/heads/main/scopes/civic-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- AI Agents
- Authentication
- Digital Identity
- Identity Verification
- KYC
- MCP
- OAuth
- Security
- Solana
- Web3
- Wallets
token_urls:
- https://auth0.civic.com/oauth/token
---
