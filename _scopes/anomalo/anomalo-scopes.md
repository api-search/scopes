---
api_specs:
- filename: anomalo-public-api-openapi.yml
  format: yaml
  label: Anomalo Public API
  slug: anomalo-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/openapi/anomalo-public-api-openapi.yml
authorization_urls:
- https://app.anomalo.com/oauth/authorize/
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Anomalo Scopes
name_suffix: OAuth Scopes
note: 'IMPORTANT SCOPE BOUNDARY: these OAuth 2.0 / OIDC scopes govern USER SIGN-ON to the Anomalo web application, not access to the Anomalo Public API. The Public API authenticates with an `X-Anomalo-Token` API secret token and has NO scope model at all — no OAuth flow, no token endpoint, no per-scope authorization. API authorization is instead enforced through access groups and policies (see the Access Groups operations in openapi/anomalo-public-api-openapi.yml). This file exists because the OIDC discovery document is real and anonymously retrievable, not because the API is OAuth-secured. Nothing here was derived from the OpenAPI, which declares no oauth2 security scheme.'
overview: 'Anomalo publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Anomalo API on a user''s behalf.


  Tokens are issued from https://app.anomalo.com/oauth/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Anomalo
provider_slug: anomalo
schemes:
- flows:
  - authorizationUrl: https://app.anomalo.com/oauth/authorize/
    flow: authorizationCode
    pkce: true
    pkce_methods:
    - S256
    tokenUrl: https://app.anomalo.com/oauth/token/
    userinfoUrl: https://app.anomalo.com/oauth/userinfo/
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://app.anomalo.com
  jwks_note: Advertised in the discovery document but returns 404 anonymously, so a relying party cannot complete key discovery without additional access.
  jwks_status: 404
  jwks_uri: https://app.anomalo.com/oauth/.well-known/jwks.json
  name: Anomalo OIDC
  response_types_supported:
  - code
  spec: OpenID Connect Discovery 1.0
  subject_types_supported:
  - public
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
scope_count: 3
scope_names:
- openid
- profile
- email
scopes:
- description: Standard OIDC scope. Requests an ID token identifying the authenticated Anomalo user.
  flows:
  - authorizationCode
  scope: openid
- description: Standard OIDC scope. Requests the user's basic profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Standard OIDC scope. Requests the user's email address and its verification status.
  flows:
  - authorizationCode
  scope: email
slug: anomalo-scopes
source_filename: anomalo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: https://app.anomalo.com/.well-known/openid-configuration\nraw: well-known/anomalo-openid-configuration.json\nnote: >-\n  IMPORTANT SCOPE BOUNDARY: these OAuth 2.0 / OIDC scopes govern USER SIGN-ON to the Anomalo web\n  application, not access to the Anomalo Public API. The Public API authenticates with an\n  `X-Anomalo-Token` API secret token and has NO scope model at all — no OAuth flow, no token endpoint,\n  no per-scope authorization. API authorization is instead enforced through access groups and policies\n  (see the Access Groups operations in openapi/anomalo-public-api-openapi.yml). This file exists because\n  the OIDC discovery document is real and anonymously retrievable, not because the API is OAuth-secured.\n  Nothing here was derived from the OpenAPI, which declares no oauth2 security scheme.\napplies_to: web application single sign-on\napi_authorization_model: api-key + access groups (see authentication/anomalo-authentication.yml)\n\
  schemes:\n  - name: Anomalo OIDC\n    spec: OpenID Connect Discovery 1.0\n    issuer: https://app.anomalo.com\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://app.anomalo.com/oauth/authorize/\n        tokenUrl: https://app.anomalo.com/oauth/token/\n        userinfoUrl: https://app.anomalo.com/oauth/userinfo/\n        pkce: true\n        pkce_methods: [S256]\n    response_types_supported: [code]\n    subject_types_supported: [public]\n    id_token_signing_alg_values_supported: [RS256]\n    token_endpoint_auth_methods_supported:\n      - client_secret_basic\n      - client_secret_post\n    jwks_uri: https://app.anomalo.com/oauth/.well-known/jwks.json\n    jwks_status: 404\n    jwks_note: >-\n      Advertised in the discovery document but returns 404 anonymously, so a relying party cannot\n      complete key discovery without additional access.\nscopes:\n  - scope: openid\n    description: >-\n      Standard OIDC scope. Requests an ID token identifying the authenticated\
  \ Anomalo user.\n    flows: [authorizationCode]\n    standard: true\n    sources: [well-known/anomalo-openid-configuration.json]\n  - scope: profile\n    description: >-\n      Standard OIDC scope. Requests the user's basic profile claims.\n    flows: [authorizationCode]\n    standard: true\n    sources: [well-known/anomalo-openid-configuration.json]\n  - scope: email\n    description: >-\n      Standard OIDC scope. Requests the user's email address and its verification status.\n    flows: [authorizationCode]\n    standard: true\n    sources: [well-known/anomalo-openid-configuration.json]\nscope_count: 3\ncustom_scopes: 0\ncustom_scopes_note: >-\n  Anomalo declares only the three standard OIDC scopes. There are no Anomalo-specific scopes — no\n  read/write split, no per-resource scopes for tables, checks, warehouses or organizations.\ndocs: null\ndocs_note: Anomalo publishes no scopes or permissions reference page; its documentation is customer-gated.\nx-evidence:\n  fetched: '2026-07-31'\n\
  \  url: https://app.anomalo.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/scopes/anomalo-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- data-quality
- data-observability
- data-monitoring
- anomaly-detection
- data-governance
- data-lineage
- data-profiling
- data-validation
- data-engineering
- machine-learning
- snowflake
- databricks
- bigquery
- enterprise-data
- mcp
- agent-native
token_urls:
- https://app.anomalo.com/oauth/token/
---
