---
api_specs:
- filename: leadiq-graphql-api-openapi.yml
  format: yaml
  label: LeadIQ GraphQL API
  slug: leadiq-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leadiq/refs/heads/main/openapi/leadiq-graphql-api-openapi.yml
- filename: leadiq-account-api-openapi.yml
  format: yaml
  label: LeadIQ Account API
  slug: leadiq-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leadiq/refs/heads/main/openapi/leadiq-account-api-openapi.yml
- filename: leadiq-lists-api-openapi.yml
  format: yaml
  label: LeadIQ Lists API
  slug: leadiq-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leadiq/refs/heads/main/openapi/leadiq-lists-api-openapi.yml
- filename: leadiq-prospects-api-openapi.yml
  format: yaml
  label: LeadIQ Prospects API
  slug: leadiq-prospects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leadiq/refs/heads/main/openapi/leadiq-prospects-api-openapi.yml
authorization_urls:
- https://leadiq-mcp-prod.us.auth0.com/authorize
description: ''
docs: https://developer.leadiq.com/
flows:
- authorizationCode
- clientCredentials
- deviceCode
kind: oauth-scopes
layout: scope
method: probed
name: Leadiq Scopes
name_suffix: OAuth Scopes
note: LeadIQ's OpenAPI and GraphQL surfaces declare no oauth2 security scheme — they are API-key surfaces (Basic for GraphQL, X-API-Key for Prospector REST). The only OAuth surface on the estate is the MCP connector at mcp.leadiq.com, and its scopes are published anonymously in RFC 9728 protected-resource metadata rather than in a spec or a docs page. `derive-oauth-scopes.py` found zero oauth2 schemes across the specs; everything below comes from the live well-known probe.
overview: 'LeadIQ publishes 2 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the LeadIQ API on a user''s behalf.


  Tokens are issued from https://leadiq-mcp-prod.us.auth0.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: LeadIQ
provider_slug: leadiq
schemes:
- authorization_server: https://leadiq-mcp-prod.us.auth0.com/
  bearer_methods_supported:
  - header
  dynamic_client_registration: true
  flows:
  - authorizationUrl: https://leadiq-mcp-prod.us.auth0.com/authorize
    flow: authorizationCode
    pkce:
    - S256
    - plain
    tokenUrl: https://leadiq-mcp-prod.us.auth0.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://leadiq-mcp-prod.us.auth0.com/oauth/token
  - deviceAuthorizationUrl: https://leadiq-mcp-prod.us.auth0.com/oauth/device/code
    flow: deviceCode
    tokenUrl: https://leadiq-mcp-prod.us.auth0.com/oauth/token
  jwks_uri: https://leadiq-mcp-prod.us.auth0.com/.well-known/jwks.json
  name: LeadIQ MCP OAuth 2.0
  registration_endpoint: https://leadiq-mcp-prod.us.auth0.com/oidc/register
  resource: https://mcp.leadiq.com/mcp
  revocation_endpoint: https://leadiq-mcp-prod.us.auth0.com/oauth/revoke
  source: https://mcp.leadiq.com/.well-known/oauth-protected-resource
scope_count: 2
scope_names:
- leadiq:api
- offline_access
scopes:
- description: The single LeadIQ resource scope. Grants an MCP client access to the LeadIQ API surface behind mcp.leadiq.com/mcp with the signed-in user's own account permissions and credit balance. LeadIQ publishes no finer-grained per-tool or read/write split — all seventeen MCP tools, including the Salesforce export write, sit behind this one scope.
  flows:
  - authorizationCode
  scope: leadiq:api
- description: Issues a refresh token so the MCP client can keep the connection alive without re-prompting the user.
  flows:
  - authorizationCode
  scope: offline_access
slug: leadiq-scopes
source_filename: leadiq-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://mcp.leadiq.com/.well-known/oauth-protected-resource\ndocs: https://developer.leadiq.com/\nnote: >-\n  LeadIQ's OpenAPI and GraphQL surfaces declare no oauth2 security scheme — they are\n  API-key surfaces (Basic for GraphQL, X-API-Key for Prospector REST). The only OAuth\n  surface on the estate is the MCP connector at mcp.leadiq.com, and its scopes are\n  published anonymously in RFC 9728 protected-resource metadata rather than in a spec\n  or a docs page. `derive-oauth-scopes.py` found zero oauth2 schemes across the specs;\n  everything below comes from the live well-known probe.\nschemes:\n- name: LeadIQ MCP OAuth 2.0\n  source: https://mcp.leadiq.com/.well-known/oauth-protected-resource\n  resource: https://mcp.leadiq.com/mcp\n  authorization_server: https://leadiq-mcp-prod.us.auth0.com/\n  bearer_methods_supported: [header]\n  dynamic_client_registration: true\n  registration_endpoint: https://leadiq-mcp-prod.us.auth0.com/oidc/register\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://leadiq-mcp-prod.us.auth0.com/authorize\n    tokenUrl: https://leadiq-mcp-prod.us.auth0.com/oauth/token\n    pkce: [S256, plain]\n  - flow: clientCredentials\n    tokenUrl: https://leadiq-mcp-prod.us.auth0.com/oauth/token\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://leadiq-mcp-prod.us.auth0.com/oauth/device/code\n    tokenUrl: https://leadiq-mcp-prod.us.auth0.com/oauth/token\n  revocation_endpoint: https://leadiq-mcp-prod.us.auth0.com/oauth/revoke\n  jwks_uri: https://leadiq-mcp-prod.us.auth0.com/.well-known/jwks.json\nscopes:\n- scope: leadiq:api\n  description: >-\n    The single LeadIQ resource scope. Grants an MCP client access to the LeadIQ API\n    surface behind mcp.leadiq.com/mcp with the signed-in user's own account\n    permissions and credit balance. LeadIQ publishes no finer-grained per-tool or\n    read/write split — all seventeen MCP tools, including the Salesforce export write,\n    sit behind\
  \ this one scope.\n  flows: [authorizationCode]\n  sources: ['https://mcp.leadiq.com/.well-known/oauth-protected-resource']\n- scope: offline_access\n  description: Issues a refresh token so the MCP client can keep the connection alive without re-prompting the user.\n  flows: [authorizationCode]\n  sources: ['https://mcp.leadiq.com/.well-known/oauth-protected-resource']\nauthorization_server_scopes_supported:\n- openid\n- profile\n- offline_access\n- name\n- given_name\n- family_name\n- nickname\n- email\n- email_verified\n- picture\n- created_at\n- identities\n- phone\n- address\nauthorization_server_note: >-\n  Those are the Auth0 tenant's standard OIDC scopes advertised at\n  leadiq-mcp-prod.us.auth0.com/.well-known/oauth-authorization-server. They are\n  identity scopes, not LeadIQ resource scopes; only `leadiq:api` and `offline_access`\n  are named by the protected-resource document as required for the MCP resource.\nfindings:\n- >-\n  Coarse authorization. One resource scope covers\
  \ everything an agent can do,\n  including ExportProspectToSalesforce, which writes an irreversible record into the\n  customer's Salesforce org. There is no read-only scope an operator could grant to a\n  research agent.\nx-evidence:\n  fetched: '2026-08-13'\n  probes:\n  - {url: 'https://mcp.leadiq.com/.well-known/oauth-protected-resource', http_status: 200}\n  - {url: 'https://leadiq-mcp-prod.us.auth0.com/.well-known/oauth-authorization-server', http_status: 200}\n  - {url: 'https://mcp.leadiq.com/.well-known/oauth-authorization-server', http_status: 404}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leadiq/refs/heads/main/scopes/leadiq-scopes.yml
summary_line: 2 scopes · authorizationCode/clientCredentials/deviceCode
tags:
- Sales Intelligence
- B2B Data
- Contact Data
- Lead Generation
- Prospecting
- CRM Enrichment
- Sales Engagement
- GraphQL
- MCP
- Revenue Operations
- Go-To-Market
token_urls:
- https://leadiq-mcp-prod.us.auth0.com/oauth/token
---
