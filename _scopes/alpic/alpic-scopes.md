---
api_specs:
- filename: alpic-openapi-original.json
  format: json
  label: Alpic API
  slug: alpic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpic/refs/heads/main/openapi/alpic-openapi-original.json
authorization_urls: []
description: ''
docs: https://docs.alpic.ai/api-reference
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Alpic Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Alpic publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Alpic API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Alpic
provider_slug: alpic
schemes:
- name: bearerAuth
  scheme: bearer
  source: openapi/alpic-openapi-original.json
  type: http
scope_count: 3
scope_names:
- openid
- email
- profile
scopes:
- description: OIDC — issue an ID token for the authenticated user.
  flows: []
  scope: openid
- description: OIDC — include the user's email in the ID token.
  flows: []
  scope: email
- description: OIDC — include the user's profile claims in the ID token.
  flows: []
  scope: profile
slug: alpic-scopes
source_filename: alpic-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://api.alpic.ai/.well-known/oauth-protected-resource\ndocs: https://docs.alpic.ai/api-reference\nnotes: >-\n  The Alpic OpenAPI declares a single http/bearer scheme (API key or OAuth access token) and\n  no oauth2 flow with an authorization-scope map, so there is no API-authorization scope surface\n  to derive from the spec. The scopes below are the OIDC login scopes advertised on the\n  protected-resource metadata (used for user authentication via the Amazon Cognito authorization\n  server), not per-endpoint API permissions. Access to the REST API is all-or-nothing per token.\nschemes:\n  - name: bearerAuth\n    source: openapi/alpic-openapi-original.json\n    type: http\n    scheme: bearer\nscopes:\n  - scope: openid\n    description: OIDC — issue an ID token for the authenticated user.\n    source: well-known/alpic-oauth-protected-resource.json\n  - scope: email\n    description: OIDC — include the user's email in the\
  \ ID token.\n    source: well-known/alpic-oauth-protected-resource.json\n  - scope: profile\n    description: OIDC — include the user's profile claims in the ID token.\n    source: well-known/alpic-oauth-protected-resource.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alpic/refs/heads/main/scopes/alpic-scopes.yml
summary_line: 3 scopes
tags:
- Company
- Ai/Ml
- MCP
- Model Context Protocol
- Cloud Platform
- Developer Tools
- Deployment
- ChatGPT Apps
- Agentic
token_urls: []
---
