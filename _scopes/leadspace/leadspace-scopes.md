---
api_specs:
- filename: leadspace-authorization-api-openapi.yml
  format: yaml
  label: Leadspace Authorization API
  slug: leadspace-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leadspace/refs/heads/main/openapi/leadspace-authorization-api-openapi.yml
- filename: leadspace-discovery-api-openapi.yml
  format: yaml
  label: Leadspace Discovery API
  slug: leadspace-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leadspace/refs/heads/main/openapi/leadspace-discovery-api-openapi.yml
- filename: leadspace-enrichment-api-openapi.yml
  format: yaml
  label: Leadspace Enrichment API
  slug: leadspace-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leadspace/refs/heads/main/openapi/leadspace-enrichment-api-openapi.yml
- filename: leadspace-intent-api-openapi.yml
  format: yaml
  label: Leadspace Intent API
  slug: leadspace-intent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leadspace/refs/heads/main/openapi/leadspace-intent-api-openapi.yml
- filename: leadspace-results-api-openapi.yml
  format: yaml
  label: Leadspace Results API
  slug: leadspace-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leadspace/refs/heads/main/openapi/leadspace-results-api-openapi.yml
authorization_urls:
- https://stg-sk.us.auth0.com/authorize
description: 'Leadspace now has exactly one OAuth scope surface, and it belongs to the MCP server — not to the v4 REST gateway. The scopes below are read verbatim from Leadspace''s own RFC 9728 protected-resource metadata. They are pure OIDC identity scopes: there is no Leadspace-specific authorization scope (nothing like `read:contacts` or `reveal:email`), so an MCP client''s token carries identity only and every entitlement decision — plan tier, credit balance, which reveals are permitted — is made server-side against the account.'
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Leadspace Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Leadspace publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Leadspace API on a user''s behalf.


  Tokens are issued from https://stg-sk.us.auth0.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Leadspace
provider_slug: leadspace
schemes:
- applies_to: https://skprod.leadspace.com/mcp/v1
  bearer_methods_supported:
  - header
  flows:
  - authorizationUrl: https://stg-sk.us.auth0.com/authorize
    dynamic_client_registration: true
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    pkce: S256
    registrationUrl: https://stg-sk.us.auth0.com/oidc/register
    tokenUrl: https://stg-sk.us.auth0.com/oauth/token
    token_endpoint_auth_methods:
    - none
    - client_secret_post
  jwks_uri: https://stg-sk.us.auth0.com/.well-known/jwks.json
  name: mcp-oauth
  protocol: OAuth 2.1
  source: https://skprod.leadspace.com/.well-known/oauth-protected-resource
  type: oauth2
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: OIDC — issue an ID token identifying the Leadspace user.
  flows:
  - authorizationCode
  scope: openid
- description: OIDC — basic profile claims for the signed-in Leadspace user.
  flows:
  - authorizationCode
  scope: profile
- description: OIDC — email claim for the signed-in Leadspace user.
  flows:
  - authorizationCode
  scope: email
- description: Issue a refresh token so the MCP client can keep the connector authorized between sessions.
  flows:
  - authorizationCode
  scope: offline_access
slug: leadspace-scopes
source_filename: leadspace-scopes.yml
source_heading: OAuth Scopes
source_url: https://skprod.leadspace.com/.well-known/oauth-protected-resource
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://skprod.leadspace.com/.well-known/oauth-protected-resource\nsources:\n- https://skprod.leadspace.com/.well-known/oauth-protected-resource\n- https://skprod.leadspace.com/.well-known/oauth-authorization-server\n- https://stg-sk.us.auth0.com/.well-known/openid-configuration\ndescription: >-\n  Leadspace now has exactly one OAuth scope surface, and it belongs to the MCP\n  server — not to the v4 REST gateway. The scopes below are read verbatim from\n  Leadspace's own RFC 9728 protected-resource metadata. They are pure OIDC\n  identity scopes: there is no Leadspace-specific authorization scope (nothing\n  like `read:contacts` or `reveal:email`), so an MCP client's token carries\n  identity only and every entitlement decision — plan tier, credit balance,\n  which reveals are permitted — is made server-side against the account.\nscope_count: 4\nschemes:\n- name: mcp-oauth\n  applies_to: https://skprod.leadspace.com/mcp/v1\n\
  \  type: oauth2\n  protocol: OAuth 2.1\n  flows:\n  - flow: authorizationCode\n    pkce: S256\n    authorizationUrl: https://stg-sk.us.auth0.com/authorize\n    tokenUrl: https://stg-sk.us.auth0.com/oauth/token\n    registrationUrl: https://stg-sk.us.auth0.com/oidc/register\n    dynamic_client_registration: true\n    grant_types:\n    - authorization_code\n    - refresh_token\n    token_endpoint_auth_methods:\n    - none\n    - client_secret_post\n  bearer_methods_supported:\n  - header\n  jwks_uri: https://stg-sk.us.auth0.com/.well-known/jwks.json\n  source: https://skprod.leadspace.com/.well-known/oauth-protected-resource\nscopes:\n- scope: openid\n  description: OIDC — issue an ID token identifying the Leadspace user.\n  flows:\n  - authorizationCode\n  standard: true\n- scope: profile\n  description: OIDC — basic profile claims for the signed-in Leadspace user.\n  flows:\n  - authorizationCode\n  standard: true\n- scope: email\n  description: OIDC — email claim for the signed-in Leadspace\
  \ user.\n  flows:\n  - authorizationCode\n  standard: true\n- scope: offline_access\n  description: Issue a refresh token so the MCP client can keep the connector authorized between sessions.\n  flows:\n  - authorizationCode\n  standard: true\nv4_gateway:\n  scopes: []\n  note: >-\n    The enterprise v4 API (apigw.leadspace.com) uses an OAuth 2.0 resource-owner\n    password-credentials exchange with an `audience` of API_GATEWAY and issues a\n    24-hour bearer token. It documents no scopes at all — entitlement is bound to\n    the Program ID. See authentication/leadspace-authentication.yml.\nobservations:\n- No provider-defined authorization scopes exist. An agent holding a Leadspace MCP token cannot be constrained to read-only or to lookups-without-reveals by scope; the only spend control is the plan's credit allowance.\n- The production MCP resource advertises its authorization server as the Auth0 tenant `stg-sk.us.auth0.com`, whose subdomain reads as a staging tenant. Recorded as observed,\
  \ not interpreted.\nx-evidence:\n- url: https://skprod.leadspace.com/.well-known/oauth-protected-resource\n  http_status: 200\n  content_type: application/json\n  fetched: '2026-08-13'\n- url: https://skprod.leadspace.com/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type: application/json\n  fetched: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leadspace/refs/heads/main/scopes/leadspace-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- MCP
- AI Agents
- B2B Data
- Customer Data Platform
- Data Enrichment
- Intent Data
- Sales Intelligence
- Account Based Marketing
- Identity Resolution
- Firmographics
- Lead Scoring
- Company
token_urls:
- https://stg-sk.us.auth0.com/oauth/token
---
