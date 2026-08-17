---
authorization_urls:
- https://oauth.enigma.com/authorize
description: ''
docs: https://documentation.enigma.com/guides/ai-mcp
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Enigma Analytics Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Enigma Analytics uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://oauth.enigma.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Enigma Analytics
provider_slug: enigma-analytics
schemes:
- dynamic_client_registration:
    note: RFC 7591 dynamic client registration is open, which is what lets an arbitrary MCP client onboard without a pre-provisioned client_id — the mechanism the MCP authorization spec relies on.
    registration_endpoint: https://oauth.enigma.com/register
    supported: true
  flows:
  - authorizationUrl: https://oauth.enigma.com/authorize
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    pkce_required_methods:
    - S256
    response_modes:
    - query
    - fragment
    response_types:
    - code
    tokenUrl: https://oauth.enigma.com/token
    token_endpoint_auth_methods:
    - client_secret_basic
  identity_provider: Amazon Cognito (us-east-1)
  introspection_endpoint: https://oauth.enigma.com/introspect
  issuer: https://oauth.enigma.com
  jwks_uri: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_00OC0VOa2/.well-known/jwks.json
  name: EnigmaMCPOAuth
  protected_resource: https://mcp.enigma.com/http
  revocation_endpoint: https://oauth.enigma.com/revoke
  service_documentation: https://modelcontextprotocol.io/authorization
  type: oauth2
  version: OAuth 2.1 (MCP authorization profile)
scope_count: 0
scope_names: []
scopes: []
slug: enigma-analytics-scopes
source_filename: enigma-analytics-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://mcp.enigma.com/.well-known/oauth-authorization-server\ndocs: https://documentation.enigma.com/guides/ai-mcp\nnotes: >-\n  Enigma's OAuth surface exists for ONE purpose: authorizing MCP clients against\n  https://mcp.enigma.com/mcp. The GraphQL API, the KYB REST API and the Screen API are all API-key\n  (x-api-key) authenticated and have no OAuth or scope surface at all — do not read this file as a\n  scope model for them. The authorization-server metadata was fetched anonymously (RFC 8414) and is\n  saved verbatim at well-known/enigma-analytics-oauth-authorization-server.json; the protected\n  resource metadata (RFC 9728) is at well-known/enigma-analytics-oauth-protected-resource.json.\nschemes:\n- name: EnigmaMCPOAuth\n  type: oauth2\n  version: OAuth 2.1 (MCP authorization profile)\n  issuer: https://oauth.enigma.com\n  protected_resource: https://mcp.enigma.com/http\n  service_documentation: https://modelcontextprotocol.io/authorization\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth.enigma.com/authorize\n    tokenUrl: https://oauth.enigma.com/token\n    pkce_required_methods: [S256]\n    response_types: [code]\n    response_modes: [query, fragment]\n    grant_types: [authorization_code, refresh_token]\n    token_endpoint_auth_methods: [client_secret_basic]\n  dynamic_client_registration:\n    supported: true\n    registration_endpoint: https://oauth.enigma.com/register\n    note: >-\n      RFC 7591 dynamic client registration is open, which is what lets an arbitrary MCP client\n      onboard without a pre-provisioned client_id — the mechanism the MCP authorization spec relies on.\n  revocation_endpoint: https://oauth.enigma.com/revoke\n  introspection_endpoint: https://oauth.enigma.com/introspect\n  jwks_uri: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_00OC0VOa2/.well-known/jwks.json\n  identity_provider: Amazon Cognito (us-east-1)\nscopes:\n- name: openid\n  description: >-\n  \
  \  The only scope advertised in `scopes_supported`. There is no per-tool, per-dataset or\n    read/write scope decomposition — an authorized MCP client receives the whole tool surface, and\n    access is bounded by plan and by the per-tool rate limits rather than by scope.\n  source: https://mcp.enigma.com/.well-known/oauth-authorization-server\nscope_count: 1\ngaps:\n- >-\n    No granular scopes. A KYB/sanctions dataset is exactly the surface where an agent operator would\n    want to grant `screening:read` without `card-analytics:read`; today that separation does not\n    exist at the token layer.\n- No OpenID Connect discovery document (/.well-known/openid-configuration 404s on every host) despite `openid` being the advertised scope.\nx-evidence:\n  fetched: '2026-08-14'\n  url: https://mcp.enigma.com/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enigma-analytics/refs/heads/main/scopes/enigma-analytics-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Business Data
- KYB
- Identity Verification
- Compliance
- Sanctions Screening
- GraphQL
- Fintech
- Data Enrichment
- MCP
- Agent Skills
- Payments Risk
token_urls:
- https://oauth.enigma.com/token
---
