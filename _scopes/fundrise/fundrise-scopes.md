---
api_specs:
- filename: fundrise-acknowledgments-api-openapi.yml
  format: yaml
  label: Fundrise Acknowledgments API
  slug: fundrise-acknowledgments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundrise/refs/heads/main/openapi/fundrise-acknowledgments-api-openapi.yml
- filename: fundrise-authentication-api-openapi.yml
  format: yaml
  label: Fundrise Authentication API
  slug: fundrise-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundrise/refs/heads/main/openapi/fundrise-authentication-api-openapi.yml
- filename: fundrise-clients-api-openapi.yml
  format: yaml
  label: Fundrise Clients API
  slug: fundrise-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundrise/refs/heads/main/openapi/fundrise-clients-api-openapi.yml
- filename: fundrise-holdings-api-openapi.yml
  format: yaml
  label: Fundrise Holdings API
  slug: fundrise-holdings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundrise/refs/heads/main/openapi/fundrise-holdings-api-openapi.yml
- filename: fundrise-investments-api-openapi.yml
  format: yaml
  label: Fundrise Investments API
  slug: fundrise-investments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundrise/refs/heads/main/openapi/fundrise-investments-api-openapi.yml
- filename: fundrise-liquidations-api-openapi.yml
  format: yaml
  label: Fundrise Liquidations API
  slug: fundrise-liquidations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundrise/refs/heads/main/openapi/fundrise-liquidations-api-openapi.yml
- filename: fundrise-offerings-api-openapi.yml
  format: yaml
  label: Fundrise Offerings API
  slug: fundrise-offerings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundrise/refs/heads/main/openapi/fundrise-offerings-api-openapi.yml
- filename: fundrise-tax-forms-api-openapi.yml
  format: yaml
  label: Fundrise Tax Forms API
  slug: fundrise-tax-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundrise/refs/heads/main/openapi/fundrise-tax-forms-api-openapi.yml
- filename: fundrise-transactions-api-openapi.yml
  format: yaml
  label: Fundrise Transactions API
  slug: fundrise-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundrise/refs/heads/main/openapi/fundrise-transactions-api-openapi.yml
authorization_urls: []
description: ''
docs: https://connect.fundrise.com/#tag/Authentication
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Fundrise Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Fundrise publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Fundrise API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Fundrise
provider_slug: fundrise
schemes: []
scope_count: 2
scope_names:
- openid
- offline_access
scopes:
- description: OpenID Connect authentication — requests an ID token asserting the end user's identity. Published in scopes_supported of the Fundrise OIDC discovery document.
  flows:
  - authorizationCode
  scope: openid
- description: Requests a refresh token so the client can obtain new access tokens without the end user being present. Published in scopes_supported of the Fundrise OIDC discovery document, and consistent with the non-expiring refresh token the Connect API issues at Client creation.
  flows:
  - authorizationCode
  scope: offline_access
slug: fundrise-scopes
source_filename: fundrise-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://fundrise.com/.well-known/openid-configuration\ndocs: https://connect.fundrise.com/#tag/Authentication\nnotes: >-\n  The Fundrise Connect OpenAPI declares no oauth2 securityScheme — both schemes are\n  HTTP (basic for Partners, bearer for Clients) — so 0-working/derive-oauth-scopes.py\n  produced nothing. Fundrise nevertheless runs a real OAuth surface, published two\n  ways, and this file records both rather than leaving the provider with no scope\n  artifact.\n\n  1. The consumer OAuth authorization server, advertised anonymously at\n     https://fundrise.com/.well-known/openid-configuration, publishes an explicit\n     scopes_supported list.\n  2. The Connect partner API issues Client-scoped access tokens from a non-expiring\n     refresh token via POST /v1/oauth/token (operationId GetAccessToken). Its\n     OAuth2AccessTokenResponse schema carries a `scope` field, but the OpenAPI does\n     not enumerate the permitted\
  \ values, so no named partner scopes are asserted here.\nauthorization_server:\n  issuer_host: fundrise.com\n  discovery: https://fundrise.com/.well-known/openid-configuration\n  authorization_endpoint: https://fundrise.com/oauth/authorize\n  token_endpoint: https://api.fundrise.com/oauth/token\n  response_types_supported:\n  - code\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  grant_types_observed:\n  - authorization_code\n  - refresh_token\nscopes:\n- scope: openid\n  description: >-\n    OpenID Connect authentication — requests an ID token asserting the end user's\n    identity. Published in scopes_supported of the Fundrise OIDC discovery document.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/fundrise-openid-configuration.json\n- scope: offline_access\n  description: >-\n    Requests a refresh token so the client can obtain new access tokens without the\n    end user being present. Published in scopes_supported of the Fundrise OIDC\n    discovery document,\
  \ and consistent with the non-expiring refresh token the\n    Connect API issues at Client creation.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/fundrise-openid-configuration.json\nconnect_api_tokens:\n  operation: GetAccessToken\n  path: /v1/oauth/token\n  grant: refresh_token\n  response_schema: OAuth2AccessTokenResponse\n  scope_field_present: true\n  named_scopes_published: false\n  note: >-\n    Access tokens are scoped to a single Client rather than to named permission\n    scopes. Endpoint-level authorization is expressed instead by which of the two\n    security schemes an operation requires (PartnerBasicAuthentication vs\n    ClientBearerAuthentication), and Fundrise applies additional per-partner access\n    controls out of band — the Authentication tag states that documented capabilities\n    may be inaccessible until permissions are granted by connect@fundrise.com.\nx-evidence:\n- fetched: '2026-08-04'\n  url: https://fundrise.com/.well-known/openid-configuration\n\
  \  http_status: 200\n  content_type: application/json\n- fetched: '2026-08-04'\n  url: https://connect.fundrise.com/\n  http_status: 200\n  note: OpenAPI 3.1.0 extracted from the published Redocly documentation bundle.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fundrise/refs/heads/main/scopes/fundrise-scopes.yml
summary_line: 2 scopes
tags:
- Company
- Financial Services
- Investing
- Real Estate
- Private Credit
- Venture Capital
- Alternative Assets
- Wealth Management
- Fintech
- Embedded Investing
token_urls: []
---
