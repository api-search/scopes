---
api_specs:
- filename: getaccept-openapi-original.json
  format: json
  label: GetAccept API
  slug: getaccept-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-openapi-original.json
authorization_urls:
- https://app.getaccept.com/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Getaccept Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'GetAccept publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the GetAccept API on a user''s behalf.


  Tokens are issued from https://app.getaccept.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: GetAccept
provider_slug: getaccept
schemes:
- description: For testing purpose, use client_id **api** and client_secret **app**
  flows:
  - authorizationUrl: https://app.getaccept.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://app.getaccept.com/oauth2/token
  name: Oauth2
  source: openapi/getaccept-openapi-original.json
scope_count: 1
scope_names:
- basic
scopes:
- description: Grants basic access to operations
  flows:
  - authorizationCode
  scope: basic
slug: getaccept-scopes
source_filename: getaccept-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/getaccept-openapi-original.json\nschemes:\n- name: Oauth2\n  source: openapi/getaccept-openapi-original.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.getaccept.com/oauth2/authorize\n    tokenUrl: https://app.getaccept.com/oauth2/token\n  description: For testing purpose, use client_id **api** and client_secret **app**\nscopes:\n- scope: basic\n  description: Grants basic access to operations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/getaccept-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/scopes/getaccept-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Cloud
- Sales Enablement
- Electronic Signature
- E-Signature
- Digital Sales Room
- Document Management
- Contract Management
- Proposals
- SaaS
token_urls:
- https://app.getaccept.com/oauth2/token
---
