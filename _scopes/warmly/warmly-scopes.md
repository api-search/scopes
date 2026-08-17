---
authorization_urls:
- https://vigorous-paper-03.authkit.app/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
- deviceCode
- refreshToken
- clientCredentials
kind: oauth-scopes
layout: scope
method: probed
name: Warmly Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Warmly publishes 4 OAuth 2.0 scopes via the authorizationCode, deviceCode, refreshToken, and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Warmly API on a user''s behalf.


  Tokens are issued from https://vigorous-paper-03.authkit.app/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Warmly
provider_slug: warmly
schemes:
- client_id_metadata_document_supported: true
  dynamic_client_registration: true
  endpoints:
    introspection_endpoint: https://vigorous-paper-03.authkit.app/oauth2/introspection
    jwks_uri: https://vigorous-paper-03.authkit.app/oauth2/jwks
    registration_endpoint: https://vigorous-paper-03.authkit.app/oauth2/register
    userinfo_endpoint: https://vigorous-paper-03.authkit.app/oauth2/userinfo
  first_party: false
  first_party_note: A managed AuthKit tenant. Recorded here because Warmly's own RFC 9728 metadata names it as the authorization server for the Warmly MCP resource.
  flows:
  - authorizationUrl: https://vigorous-paper-03.authkit.app/oauth2/authorize
    flow: authorizationCode
    pkce:
    - S256
    tokenUrl: https://vigorous-paper-03.authkit.app/oauth2/token
  - deviceAuthorizationUrl: https://vigorous-paper-03.authkit.app/oauth2/device_authorization
    flow: deviceCode
  - flow: refreshToken
    tokenUrl: https://vigorous-paper-03.authkit.app/oauth2/token
  - flow: clientCredentials
    note: Advertised in openid-configuration only; absent from the RFC 8414 document.
    tokenUrl: https://vigorous-paper-03.authkit.app/oauth2/token
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://vigorous-paper-03.authkit.app
  name: WarmlyMcpOAuth
  platform: WorkOS AuthKit
  token_endpoint_auth_methods_supported:
  - none
  - client_secret_post
  - client_secret_basic
  type: oauth2
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: OIDC subject identifier. Generic AuthKit scope, not Warmly-specific.
  flows:
  - authorizationCode
  scope: openid
- description: Basic profile claims. Generic AuthKit scope, not Warmly-specific.
  flows:
  - authorizationCode
  scope: profile
- description: Email claim. Generic AuthKit scope, not Warmly-specific.
  flows:
  - authorizationCode
  scope: email
- description: Issues a refresh token for long-running agent sessions.
  flows:
  - authorizationCode
  - refreshToken
  scope: offline_access
slug: warmly-scopes
source_filename: warmly-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://opps-api.getwarmly.com/.well-known/oauth-protected-resource\nauthorization_server: https://vigorous-paper-03.authkit.app\ndiscovery:\n- {url: 'https://opps-api.getwarmly.com/.well-known/oauth-protected-resource', spec: RFC 9728, status: 200}\n- {url: 'https://vigorous-paper-03.authkit.app/.well-known/oauth-authorization-server', spec: RFC 8414, status: 200}\n- {url: 'https://vigorous-paper-03.authkit.app/.well-known/openid-configuration', spec: OIDC Discovery 1.0, status: 200}\nsummary: >-\n  Warmly's MCP server is an OAuth 2.0 protected resource, but it publishes NO\n  API-specific scopes. Its RFC 9728 metadata declares scopes_supported: [] — an\n  explicitly empty list — and the delegated WorkOS AuthKit authorization server\n  offers only the four generic OIDC scopes. There is therefore no way for an agent\n  or an administrator to request least-privilege access to a subset of Warmly's\n  tools: a token is all-or-nothing\
  \ across every tool the organization can reach,\n  including the async write tools that push contacts into HubSpot and Salesforce.\n  Authorization is scoped by organization, not by capability.\nresource:\n  identifier: https://opps-api.getwarmly.com/api/mcp\n  bearer_methods_supported: [header]\n  scopes_supported: []\n  resource_documentation: https://docs.getwarmly.com/mcp\n  documentation_note: The declared documentation host does not resolve in DNS (NXDOMAIN); the live docs are on help.warmly.ai.\nschemes:\n- name: WarmlyMcpOAuth\n  type: oauth2\n  issuer: https://vigorous-paper-03.authkit.app\n  platform: WorkOS AuthKit\n  first_party: false\n  first_party_note: >-\n    A managed AuthKit tenant. Recorded here because Warmly's own RFC 9728 metadata\n    names it as the authorization server for the Warmly MCP resource.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://vigorous-paper-03.authkit.app/oauth2/authorize\n    tokenUrl: https://vigorous-paper-03.authkit.app/oauth2/token\n\
  \    pkce: [S256]\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://vigorous-paper-03.authkit.app/oauth2/device_authorization\n  - flow: refreshToken\n    tokenUrl: https://vigorous-paper-03.authkit.app/oauth2/token\n  - flow: clientCredentials\n    tokenUrl: https://vigorous-paper-03.authkit.app/oauth2/token\n    note: Advertised in openid-configuration only; absent from the RFC 8414 document.\n  endpoints:\n    jwks_uri: https://vigorous-paper-03.authkit.app/oauth2/jwks\n    introspection_endpoint: https://vigorous-paper-03.authkit.app/oauth2/introspection\n    userinfo_endpoint: https://vigorous-paper-03.authkit.app/oauth2/userinfo\n    registration_endpoint: https://vigorous-paper-03.authkit.app/oauth2/register\n  dynamic_client_registration: true\n  client_id_metadata_document_supported: true\n  token_endpoint_auth_methods_supported: [none, client_secret_post, client_secret_basic]\n  id_token_signing_alg_values_supported: [RS256]\nscopes:\n- scope: openid\n  description:\
  \ OIDC subject identifier. Generic AuthKit scope, not Warmly-specific.\n  flows: [authorizationCode]\n  source: authorization-server\n- scope: profile\n  description: Basic profile claims. Generic AuthKit scope, not Warmly-specific.\n  flows: [authorizationCode]\n  source: authorization-server\n- scope: email\n  description: Email claim. Generic AuthKit scope, not Warmly-specific.\n  flows: [authorizationCode]\n  source: authorization-server\n- scope: offline_access\n  description: Issues a refresh token for long-running agent sessions.\n  flows: [authorizationCode, refreshToken]\n  source: authorization-server\napi_scopes:\n  count: 0\n  note: >-\n    Zero resource-specific scopes exist. No read-vs-write separation, no per-tool\n    scope, and no scope that distinguishes reading warm visitors from writing\n    contacts into a connected CRM.\norganization_scoping:\n  mechanism: Out-of-band, not via scope\n  query_param: organization_id\n  header: X-Warmly-Organization-Id\n  reference:\
  \ authentication/warmly-authentication.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/warmly/refs/heads/main/scopes/warmly-scopes.yml
summary_line: 4 scopes · authorizationCode/deviceCode/refreshToken/clientCredentials
tags:
- Company
- Sales
- Marketing
- Intent Data
- Revenue Orchestration
- Website Visitor Identification
- AI Agents
- Go To Market
- MCP
- Lead Generation
- CRM
token_urls:
- https://vigorous-paper-03.authkit.app/oauth2/token
---
