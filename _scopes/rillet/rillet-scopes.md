---
api_specs:
- filename: rillet-accounting-api-openapi.json
  format: json
  label: Rillet Accounting API
  slug: rillet-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rillet/refs/heads/main/openapi/rillet-accounting-api-openapi.json
authorization_urls:
- https://api.rillet.com/oauth2/authorize
description: ''
docs: https://docs.api.rillet.com/docs/mcp
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Rillet Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Rillet publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Rillet API on a user''s behalf.


  Tokens are issued from https://api.rillet.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Rillet
provider_slug: rillet
schemes:
- flows:
  - authorizationUrl: https://api.rillet.com/oauth2/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://api.rillet.com/oauth2/token
  name: oauth2
  source: well-known/rillet-oauth-authorization-server.json
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read access to Rillet resources (list/retrieve operations).
  flows:
  - authorizationCode
  scope: read
- description: Write access to Rillet resources (create/update/delete operations).
  flows:
  - authorizationCode
  scope: write
slug: rillet-scopes
source_filename: rillet-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: well-known/rillet-oauth-protected-resource.json\ndocs: https://docs.api.rillet.com/docs/mcp\nschemes:\n- name: oauth2\n  source: well-known/rillet-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.rillet.com/oauth2/authorize\n    tokenUrl: https://api.rillet.com/oauth2/token\n    pkce: S256\nscopes:\n- scope: read\n  description: Read access to Rillet resources (list/retrieve operations).\n  flows: [authorizationCode]\n  sources: [well-known/rillet-oauth-protected-resource.json]\n- scope: write\n  description: Write access to Rillet resources (create/update/delete operations).\n  flows: [authorizationCode]\n  sources: [well-known/rillet-oauth-protected-resource.json]\nnotes: >-\n  Coarse-grained read/write scopes advertised in RFC 9728 protected-resource\n  metadata. Effective authorization is further constrained by the connected\n  user's role within Rillet (Owner / Admin\
  \ / Accountant / view-only). Direct\n  API-key (Bearer) access is not scope-limited at the token level.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rillet/refs/heads/main/scopes/rillet-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Fintech
- ERP
- Accounting
- Finance
- General Ledger
- Accounts Receivable
- Accounts Payable
- Invoicing
- SaaS
token_urls:
- https://api.rillet.com/oauth2/token
---
