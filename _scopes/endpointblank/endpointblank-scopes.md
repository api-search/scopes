---
api_specs:
- filename: endpointblank-openapi-generated.yml
  format: yaml
  label: Bengal Technologies API
  slug: endpointblank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endpointblank/refs/heads/main/openapi/_ae-authored/endpointblank-openapi-generated.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Endpointblank Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Bengal Technologies uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://app.endpointblank.com/agent-oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bengal Technologies
provider_slug: endpointblank
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://app.endpointblank.com/agent-oauth/token
  name: Token_endpoint
  source: openapi/endpointblank-openapi-generated.yml
scope_count: 0
scope_names: []
scopes: []
slug: endpointblank-scopes
source_filename: endpointblank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: derived\nsource: openapi/endpointblank-openapi-generated.yml\nschemes:\n- name: Token_endpoint\n  source: openapi/endpointblank-openapi-generated.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://app.endpointblank.com/agent-oauth/token\nscopes:\n  - default\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/endpointblank/refs/heads/main/scopes/endpointblank-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- API Management
- Versioning
- Authentication
- Monitoring
token_bound: false
token_urls:
- https://app.endpointblank.com/agent-oauth/token
---
