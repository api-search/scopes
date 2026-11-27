---
api_specs:
- filename: corroborateme-com-agents-api-openapi.yml
  format: yaml
  label: CorroborateMe Agents API
  slug: corroborateme-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corroborateme-com/openapi/corroborateme-com-agents-api-openapi.yml
- filename: corroborateme-com-billing-api-openapi.yml
  format: yaml
  label: CorroborateMe Billing API
  slug: corroborateme-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corroborateme-com/openapi/corroborateme-com-billing-api-openapi.yml
- filename: corroborateme-com-companies-api-openapi.yml
  format: yaml
  label: CorroborateMe Companies API
  slug: corroborateme-com-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corroborateme-com/openapi/corroborateme-com-companies-api-openapi.yml
- filename: corroborateme-com-console-auth-api-openapi.yml
  format: yaml
  label: CorroborateMe Console auth API
  slug: corroborateme-com-console-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corroborateme-com/openapi/corroborateme-com-console-auth-api-openapi.yml
- filename: corroborateme-com-discovery-api-openapi.yml
  format: yaml
  label: CorroborateMe Discovery API
  slug: corroborateme-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corroborateme-com/openapi/corroborateme-com-discovery-api-openapi.yml
- filename: corroborateme-com-integrations-api-openapi.yml
  format: yaml
  label: CorroborateMe Integrations API
  slug: corroborateme-com-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corroborateme-com/openapi/corroborateme-com-integrations-api-openapi.yml
- filename: corroborateme-com-login-link-idp-api-openapi.yml
  format: yaml
  label: CorroborateMe Login-link IdP API
  slug: corroborateme-com-login-link-idp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corroborateme-com/openapi/corroborateme-com-login-link-idp-api-openapi.yml
- filename: corroborateme-com-login-links-api-openapi.yml
  format: yaml
  label: CorroborateMe Login links API
  slug: corroborateme-com-login-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corroborateme-com/openapi/corroborateme-com-login-links-api-openapi.yml
- filename: corroborateme-com-mcp-api-openapi.yml
  format: yaml
  label: CorroborateMe MCP API
  slug: corroborateme-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corroborateme-com/openapi/corroborateme-com-mcp-api-openapi.yml
- filename: corroborateme-com-oidc-api-openapi.yml
  format: yaml
  label: CorroborateMe OIDC API
  slug: corroborateme-com-oidc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corroborateme-com/openapi/corroborateme-com-oidc-api-openapi.yml
authorization_urls: []
description: The OpenAPI declares only an http bearer scheme, so the derive pass finds no scopes. CorroborateMe runs an OAuth 2.0 / OIDC authorization server (issuer https://corroborateme.com/api/auth) whose published metadata lists scopes_supported; the docs say MCP hosts must authorize with a scope including mcp. Descriptions for openid/profile/email/offline_access are not given by the provider beyond their standard OIDC meaning.
docs: https://corroborateme.com/llms-full.txt
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: CorroborateMe Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CorroborateMe publishes 5 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the CorroborateMe API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CorroborateMe
provider_slug: corroborateme-com
schemes:
- authorizationUrl: https://corroborateme.com/api/auth/oauth2/authorize
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  issuer: https://corroborateme.com/api/auth
  name: CorroborateMe OAuth / OIDC
  tokenUrl: https://corroborateme.com/api/auth/oauth2/token
  type: oauth2
scope_count: 5
scope_names:
- openid
- profile
- email
- offline_access
- mcp
scopes:
- description: OIDC sign-in (listed in scopes_supported).
  flows: []
  scope: openid
- description: Listed in scopes_supported.
  flows: []
  scope: profile
- description: Listed in scopes_supported.
  flows: []
  scope: email
- description: Listed in scopes_supported (refresh tokens).
  flows: []
  scope: offline_access
- description: 'Required for MCP host access: "Authorize with resource=https://corroborateme.com/mcp/ and scope including mcp. Access token must have aud=https://corroborateme.com/mcp/ and company_id."'
  flows: []
  scope: mcp
slug: corroborateme-com-scopes
source_filename: corroborateme-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://corroborateme.com/.well-known/oauth-authorization-server\ndocs: https://corroborateme.com/llms-full.txt\ndescription: >-\n  The OpenAPI declares only an http bearer scheme, so the derive pass finds no scopes.\n  CorroborateMe runs an OAuth 2.0 / OIDC authorization server (issuer https://corroborateme.com/api/auth)\n  whose published metadata lists scopes_supported; the docs say MCP hosts must authorize with a scope including mcp.\n  Descriptions for openid/profile/email/offline_access are not given by the provider beyond their standard OIDC meaning.\nschemes:\n- name: CorroborateMe OAuth / OIDC\n  type: oauth2\n  issuer: https://corroborateme.com/api/auth\n  authorizationUrl: https://corroborateme.com/api/auth/oauth2/authorize\n  tokenUrl: https://corroborateme.com/api/auth/oauth2/token\n  grant_types: [authorization_code, client_credentials, refresh_token]\nscopes:\n- scope: openid\n  description: OIDC sign-in (listed\
  \ in scopes_supported).\n- scope: profile\n  description: Listed in scopes_supported.\n- scope: email\n  description: Listed in scopes_supported.\n- scope: offline_access\n  description: Listed in scopes_supported (refresh tokens).\n- scope: mcp\n  description: \"Required for MCP host access: \\\"Authorize with resource=https://corroborateme.com/mcp/ and scope including mcp. Access token must have aud=https://corroborateme.com/mcp/ and company_id.\\\"\"\n  source: https://corroborateme.com/llms-full.txt\n"
source_yaml_url: https://artifacts.apis.io/corroborateme-com/scopes/corroborateme-com-scopes.yml
summary_line: 5 scopes
tags:
- Company
- Authentication
- Identity
- Sign In
- Passkeys
- OpenID Connect
- SSO
- AI Agents
- MCP
token_bound: false
token_urls: []
---
