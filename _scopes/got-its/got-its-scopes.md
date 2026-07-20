---
api_specs:
- filename: got-its-openapi-original.yml
  format: yaml
  label: Reelables API
  slug: reelables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/got-its/refs/heads/main/openapi/got-its-openapi-original.yml
- filename: got-its-gateway-openapi-original.yml
  format: yaml
  label: Reelables Gateway API
  slug: reelables-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/got-its/refs/heads/main/openapi/got-its-gateway-openapi-original.yml
authorization_urls: []
description: ''
docs: https://docs.reelables.com/authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Got Its Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Reelables publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Reelables API on a user''s behalf.


  Tokens are issued from https://auth.reelables.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Reelables
provider_slug: got-its
schemes:
- flows:
  - authScheme: Basic base64(CLIENT_ID:CLIENT_SECRET)
    flow: clientCredentials
    tokenLifetimeSeconds: 3600
    tokenUrl: https://auth.reelables.com/oauth2/token
  name: AuthEndpoint
  source: openapi/got-its-openapi-original.yml
scope_count: 1
scope_names:
- https://auth.reelables.com/full-access
scopes:
- description: Full access to the Public API
  flows:
  - clientCredentials
  scope: https://auth.reelables.com/full-access
slug: got-its-scopes
source_filename: got-its-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/got-its-openapi-original.yml\ndocs: https://docs.reelables.com/authentication\nnotes: >-\n  Reelables uses a single coarse-grained OAuth 2.0 client-credentials scope granting full\n  access to the Public API. Credentials (CLIENT_ID/CLIENT_SECRET) are provisioned by contacting\n  support@reelables.com; access tokens are valid for 1 hour. No finer-grained scope catalog is\n  published.\nschemes:\n- name: AuthEndpoint\n  source: openapi/got-its-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.reelables.com/oauth2/token\n    authScheme: 'Basic base64(CLIENT_ID:CLIENT_SECRET)'\n    tokenLifetimeSeconds: 3600\nscopes:\n- scope: https://auth.reelables.com/full-access\n  description: Full access to the Public API\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/got-its-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/got-its/refs/heads/main/scopes/got-its-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Company
- Supply Chain
- Logistics
- Asset Tracking
- IoT
- Smart Labels
- Bluetooth
- Cellular
- Track and Trace
- Location
token_urls:
- https://auth.reelables.com/oauth2/token
---
