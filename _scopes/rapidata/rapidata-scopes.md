---
api_specs:
- filename: rapidata-openapi-original.json
  format: json
  label: Rapidata API
  slug: rapidata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rapidata/refs/heads/main/openapi/rapidata-openapi-original.json
authorization_urls: []
description: ''
docs: https://docs.rapidata.ai/latest/authentication/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Rapidata Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Rapidata publishes 9 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Rapidata API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Rapidata
provider_slug: rapidata
schemes:
- authorizationUrl: https://auth.rapidata.ai/connect/authorize
  grant_types:
  - client_credentials
  - authorization_code
  - refresh_token
  issuer: https://auth.rapidata.ai/
  name: OpenIdConnect
  source: openapi/rapidata-openapi-original.json
  tokenUrl: https://auth.rapidata.ai/connect/token
  type: openIdConnect
scope_count: 9
scope_names:
- openid
- profile
- email
- offline_access
- roles
- groups
- api
- rtb
- mcp
scopes:
- description: OpenID Connect authentication; returns a subject identifier.
  flows: []
  scope: openid
- description: Access to the authenticated user's basic profile claims.
  flows: []
  scope: profile
- description: Access to the authenticated user's email claim.
  flows: []
  scope: email
- description: Issue a refresh token for long-lived, offline access.
  flows: []
  scope: offline_access
- description: Include the user's role claims in the token.
  flows: []
  scope: roles
- description: Include the user's group membership claims in the token.
  flows: []
  scope: groups
- description: Access to the Rapidata REST API surface.
  flows: []
  scope: api
- description: Real-time bidding / online RLHF real-time feedback access.
  flows: []
  scope: rtb
- description: Model Context Protocol access scope.
  flows: []
  scope: mcp
slug: rapidata-scopes
source_filename: rapidata-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://auth.rapidata.ai/.well-known/openid-configuration\ndocs: https://docs.rapidata.ai/latest/authentication/\nschemes:\n- name: OpenIdConnect\n  type: openIdConnect\n  source: openapi/rapidata-openapi-original.json\n  issuer: https://auth.rapidata.ai/\n  authorizationUrl: https://auth.rapidata.ai/connect/authorize\n  tokenUrl: https://auth.rapidata.ai/connect/token\n  grant_types: [client_credentials, authorization_code, refresh_token]\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; returns a subject identifier.\n- scope: profile\n  description: Access to the authenticated user's basic profile claims.\n- scope: email\n  description: Access to the authenticated user's email claim.\n- scope: offline_access\n  description: Issue a refresh token for long-lived, offline access.\n- scope: roles\n  description: Include the user's role claims in the token.\n- scope: groups\n  description: Include the user's\
  \ group membership claims in the token.\n- scope: api\n  description: Access to the Rapidata REST API surface.\n- scope: rtb\n  description: Real-time bidding / online RLHF real-time feedback access.\n- scope: mcp\n  description: Model Context Protocol access scope.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rapidata/refs/heads/main/scopes/rapidata-scopes.yml
summary_line: 9 scopes
tags:
- Company
- Human Feedback
- Data Labeling
- Annotation
- RLHF
- Model Evaluation
- Machine Learning
- AI
- Crowdsourcing
- Preference Data
token_urls: []
---
