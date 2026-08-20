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
name: Enigma Scopes
name_suffix: OAuth Scopes
note: Enigma's OAuth surface exists only for the remote MCP server. The GraphQL Data API, KYB v2 API and Screening API authenticate with a static x-api-key header and have no OAuth or scope surface at all — see authentication/enigma-authentication.yml. Scopes below are read verbatim from the RFC 8414 authorization-server metadata document; Enigma publishes no human-facing scope/permission reference page.
overview: 'Enigma publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Enigma API on a user''s behalf.


  Tokens are issued from https://oauth.enigma.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Enigma
provider_slug: enigma
schemes:
- dynamic_client_registration: true
  flows:
  - authorizationUrl: https://oauth.enigma.com/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    pkce: required
    tokenUrl: https://oauth.enigma.com/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  identity_provider: Amazon Cognito (us-east-1)
  introspection_endpoint: https://oauth.enigma.com/introspect
  issuer: https://oauth.enigma.com
  jwks_uri: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_00OC0VOa2/.well-known/jwks.json
  name: oauth2.1
  registration_endpoint: https://oauth.enigma.com/register
  response_modes_supported:
  - query
  - fragment
  response_types_supported:
  - code
  revocation_endpoint: https://oauth.enigma.com/revoke
  service_documentation: https://modelcontextprotocol.io/authorization
  source: https://mcp.enigma.com/.well-known/oauth-authorization-server
  token_endpoint_auth_methods_supported:
  - client_secret_basic
scope_count: 1
scope_names:
- openid
scopes:
- description: The only scope advertised in scopes_supported. Enigma does not publish granular per-tool or per-dataset scopes; authorization is coarse-grained at the identity level and entitlement is enforced by account plan and per-tool rate limits rather than by OAuth scope.
  flows:
  - authorizationCode
  scope: openid
slug: enigma-scopes
source_filename: enigma-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://mcp.enigma.com/.well-known/oauth-authorization-server\ndocs: https://documentation.enigma.com/guides/ai-mcp\napplies_to: Enigma MCP server (https://mcp.enigma.com/mcp)\nnote: >-\n  Enigma's OAuth surface exists only for the remote MCP server. The GraphQL Data API, KYB\n  v2 API and Screening API authenticate with a static x-api-key header and have no OAuth\n  or scope surface at all — see authentication/enigma-authentication.yml. Scopes below\n  are read verbatim from the RFC 8414 authorization-server metadata document; Enigma\n  publishes no human-facing scope/permission reference page.\nschemes:\n- name: oauth2.1\n  source: https://mcp.enigma.com/.well-known/oauth-authorization-server\n  issuer: https://oauth.enigma.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth.enigma.com/authorize\n    tokenUrl: https://oauth.enigma.com/token\n    pkce: required\n    code_challenge_methods: [S256]\n\
  \  grant_types_supported: [authorization_code, refresh_token]\n  response_types_supported: [code]\n  response_modes_supported: [query, fragment]\n  token_endpoint_auth_methods_supported: [client_secret_basic]\n  registration_endpoint: https://oauth.enigma.com/register\n  dynamic_client_registration: true\n  revocation_endpoint: https://oauth.enigma.com/revoke\n  introspection_endpoint: https://oauth.enigma.com/introspect\n  jwks_uri: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_00OC0VOa2/.well-known/jwks.json\n  identity_provider: Amazon Cognito (us-east-1)\n  service_documentation: https://modelcontextprotocol.io/authorization\nscopes:\n- scope: openid\n  description: >-\n    The only scope advertised in scopes_supported. Enigma does not publish granular\n    per-tool or per-dataset scopes; authorization is coarse-grained at the identity level\n    and entitlement is enforced by account plan and per-tool rate limits rather than by\n    OAuth scope.\n  flows: [authorizationCode]\n\
  \  sources: [https://mcp.enigma.com/.well-known/oauth-authorization-server]\nprotected_resource:\n  source: https://mcp.enigma.com/.well-known/oauth-protected-resource\n  resource: https://mcp.enigma.com/http\n  authorization_servers: [https://oauth.enigma.com]\nx-evidence:\n  fetched: '2026-08-14'\n  urls:\n  - {url: 'https://mcp.enigma.com/.well-known/oauth-authorization-server', http_status: 200}\n  - {url: 'https://mcp.enigma.com/.well-known/oauth-protected-resource', http_status: 200}\n  - {url: 'https://oauth.enigma.com/.well-known/oauth-authorization-server', http_status: 200}\n  - {url: 'https://oauth.enigma.com/.well-known/openid-configuration', http_status: 404}\n  files:\n  - well-known/enigma-mcp-oauth-authorization-server.json\n  - well-known/enigma-mcp-oauth-protected-resource.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enigma/refs/heads/main/scopes/enigma-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Business Data
- Identity Resolution
- KYB
- Compliance
- Fraud
- GraphQL
- Data Enrichment
- Financial-Services
- MCP
- Sanctions Screening
- Agent Skills
token_urls:
- https://oauth.enigma.com/token
---
