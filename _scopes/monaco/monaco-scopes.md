---
api_specs:
- filename: monaco-accounts-api-openapi.yml
  format: yaml
  label: Monaco Accounts API
  slug: monaco-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/openapi/monaco-accounts-api-openapi.yml
- filename: monaco-audiences-api-openapi.yml
  format: yaml
  label: Monaco Audiences API
  slug: monaco-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/openapi/monaco-audiences-api-openapi.yml
- filename: monaco-auth-api-openapi.yml
  format: yaml
  label: Monaco Auth API
  slug: monaco-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/openapi/monaco-auth-api-openapi.yml
- filename: monaco-campaigns-api-openapi.yml
  format: yaml
  label: Monaco Campaigns API
  slug: monaco-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/openapi/monaco-campaigns-api-openapi.yml
- filename: monaco-contacts-api-openapi.yml
  format: yaml
  label: Monaco Contacts API
  slug: monaco-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/openapi/monaco-contacts-api-openapi.yml
- filename: monaco-meetings-api-openapi.yml
  format: yaml
  label: Monaco Meetings API
  slug: monaco-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/openapi/monaco-meetings-api-openapi.yml
- filename: monaco-opportunities-api-openapi.yml
  format: yaml
  label: Monaco Opportunities API
  slug: monaco-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/openapi/monaco-opportunities-api-openapi.yml
- filename: monaco-schemas-api-openapi.yml
  format: yaml
  label: Monaco Schemas API
  slug: monaco-schemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/openapi/monaco-schemas-api-openapi.yml
- filename: monaco-sequence-templates-api-openapi.yml
  format: yaml
  label: Monaco Sequence Templates API
  slug: monaco-sequence-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/openapi/monaco-sequence-templates-api-openapi.yml
- filename: monaco-sequences-api-openapi.yml
  format: yaml
  label: Monaco Sequences API
  slug: monaco-sequences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/openapi/monaco-sequences-api-openapi.yml
- filename: monaco-tags-api-openapi.yml
  format: yaml
  label: Monaco Tags API
  slug: monaco-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/openapi/monaco-tags-api-openapi.yml
- filename: monaco-tasks-api-openapi.yml
  format: yaml
  label: Monaco Tasks API
  slug: monaco-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/openapi/monaco-tasks-api-openapi.yml
- filename: monaco-users-api-openapi.yml
  format: yaml
  label: Monaco Users API
  slug: monaco-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/openapi/monaco-users-api-openapi.yml
authorization_urls:
- https://monaco-inc.us.auth0.com/authorize
description: ''
docs: https://docs.monaco.com/mcp/overview
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Monaco Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Monaco uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://monaco-inc.us.auth0.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Monaco
provider_slug: monaco
schemes:
- authorization_server: https://monaco-inc.us.auth0.com/
  dynamic_client_registration: https://monaco-inc.us.auth0.com/oidc/register
  flows:
  - authorizationUrl: https://monaco-inc.us.auth0.com/authorize
    flow: authorizationCode
    pkce:
    - S256
    - plain
    tokenUrl: https://monaco-inc.us.auth0.com/oauth/token
  jwks_uri: https://monaco-inc.us.auth0.com/.well-known/jwks.json
  name: oauth2Mcp
  source: https://mcp.monaco.com/.well-known/oauth-protected-resource/mcp
scope_count: 0
scope_names: []
scopes: []
slug: monaco-scopes
source_filename: monaco-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://mcp.monaco.com/.well-known/oauth-protected-resource/mcp\ndocs: https://docs.monaco.com/mcp/overview\napplies_to: >-\n  The hosted Monaco MCP server (https://mcp.monaco.com/mcp) only. The public REST\n  API at api.monaco.com uses API-key bearer authentication (prefix mks_) and has\n  no OAuth scope surface — see authentication/monaco-authentication.yml.\nprotected_resource:\n  resource: https://mcp.monaco.com/mcp\n  resource_name: Monaco Public MCP\n  authorization_servers:\n  - https://monaco-inc.us.auth0.com/\n  bearer_methods_supported: [header]\n  scopes_supported: []\n  spec: RFC 9728 OAuth 2.0 Protected Resource Metadata\n  file: well-known/monaco-oauth-protected-resource.json\nschemes:\n- name: oauth2Mcp\n  source: https://mcp.monaco.com/.well-known/oauth-protected-resource/mcp\n  authorization_server: https://monaco-inc.us.auth0.com/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://monaco-inc.us.auth0.com/authorize\n\
  \    tokenUrl: https://monaco-inc.us.auth0.com/oauth/token\n    pkce: [S256, plain]\n  dynamic_client_registration: https://monaco-inc.us.auth0.com/oidc/register\n  jwks_uri: https://monaco-inc.us.auth0.com/.well-known/jwks.json\nscopes: []\nscopes_note: >-\n  Monaco's MCP resource metadata declares an EMPTY scopes_supported array, so the\n  provider publishes no granular API scopes. Authorization is not scope-based:\n  the docs state every request is authenticated as the user who completed the\n  login and every tool call respects that user's existing Monaco permissions —\n  authority is carried by the user's in-product role, not by an OAuth scope. The\n  scopes advertised by the Auth0 authorization server below are Auth0's stock\n  OIDC identity scopes, not Monaco API permissions, and are recorded separately\n  so they are not mistaken for a Monaco scope catalog.\nauthorization_server_scopes:\n  issuer: https://monaco-inc.us.auth0.com/\n  source: https://monaco-inc.us.auth0.com/.well-known/openid-configuration\n\
  \  kind: oidc-standard-claims\n  values: [openid, profile, offline_access, name, given_name, family_name, nickname,\n    email, email_verified, picture, created_at, identities, phone, address]\npermission_model:\n  basis: user-permission-inheritance\n  detail: >-\n    Every MCP request runs as the authenticated Monaco user and inherits that\n    user's product permissions. Reads are auto-approved by the AI client; writes\n    and deletes prompt for confirmation by default.\n  source: https://docs.monaco.com/mcp/overview\nx-evidence:\n- {url: 'https://mcp.monaco.com/.well-known/oauth-protected-resource/mcp', status: 200, content_type: application/json}\n- {url: 'https://monaco-inc.us.auth0.com/.well-known/openid-configuration', status: 200}\n- {url: 'https://mcp.monaco.com/mcp', status: 401, note: 'tools/list POST returns WWW-Authenticate Bearer error=\"invalid_token\" with resource_metadata pointer — live schema is auth-gated'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/scopes/monaco-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- CRM
- Sales
- Revenue Operations
- Artificial Intelligence
- Contacts
- Account
- Opportunities
- Pipeline
- Go-To-Market
- MCP
- Campaigns
- Audiences
- Sales Engagement
- Agents
token_urls:
- https://monaco-inc.us.auth0.com/oauth/token
---
