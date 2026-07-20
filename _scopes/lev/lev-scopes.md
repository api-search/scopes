---
api_specs:
- filename: lev-openapi-original.json
  format: json
  label: Lev API
  slug: lev-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lev/refs/heads/main/openapi/lev-openapi-original.json
authorization_urls:
- https://auth.lev.com/authorize
description: ''
docs: https://www.lev.com/docs/build/authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Lev Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Lev publishes 11 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Lev API on a user''s behalf.


  Tokens are issued from https://auth.lev.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Lev
provider_slug: lev
schemes:
- kind: api-key
  name: apiKeyScopes
  note: Each API key carries a scopes list controlling which endpoints it can access. Keys are issued at one of two permission levels — full_access (default, all scopes) or read_only (read scopes only). The authenticated scope list is returned by postAuthValidateApiKey and by getMe.
  source: https://www.lev.com/docs/build/authentication
- flows:
  - authorizationUrl: https://auth.lev.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.lev.com/oauth/token
  kind: oauth2
  name: mcpOAuth
  source: well-known/lev-oauth-authorization-server.json
scope_count: 11
scope_names:
- deals:read
- deals:write
- contacts:read
- contacts:write
- companies:read
- companies:write
- lenders:read
- ai:actions
- openid
- email
- offline_access
scopes:
- description: Read access to deals and their sub-resources (financials, properties, team, documents, vaults, checklists, memos, notes, indexed facts).
  flows: []
  scope: deals:read
- description: Create, update, archive deals and write deal sub-resources including notes, checklist tasks, and recorded index facts.
  flows: []
  scope: deals:write
- description: Read access to CRM contacts and contact notes.
  flows: []
  scope: contacts:read
- description: Create and update CRM contacts and contact notes.
  flows: []
  scope: contacts:write
- description: Read access to CRM companies and company notes.
  flows: []
  scope: companies:read
- description: Create and update CRM companies and company notes.
  flows: []
  scope: companies:write
- description: Read access to the lender directory, individual lender records, and their lending programs. Read-only — the docs list no lenders:write counterpart.
  flows: []
  scope: lenders:read
- description: Gates AI-powered, credit-consuming actions separately from ordinary reads and writes. Required by postContactsContactIdActionsUnlock, which reveals an AI-recommended lender contact and charges credits.
  flows: []
  scope: ai:actions
- description: Standard OIDC scope requested by MCP clients during the Auth0 authorization-code flow.
  flows: []
  scope: openid
- description: Standard OIDC scope granting the user's email address to the MCP client.
  flows: []
  scope: email
- description: Requests a refresh token so the MCP client can silently refresh without re-prompting the user.
  flows: []
  scope: offline_access
slug: lev-scopes
source_filename: lev-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.lev.com/docs/build/authentication\ndocs: https://www.lev.com/docs/build/authentication\nsummary: Lev runs two distinct scope surfaces. The REST API uses a domain-based\n  read/write scope list attached to each API key (the OpenAPI does not declare an\n  oauth2 securityScheme, so these scopes are documented rather than machine-readable\n  in the spec). The hosted MCP server uses OAuth 2.1 against Auth0 with standard\n  OIDC scopes; per-user Lev permissions are enforced behind the token rather than\n  expressed as OAuth scopes.\nschemes:\n- name: apiKeyScopes\n  kind: api-key\n  source: https://www.lev.com/docs/build/authentication\n  note: Each API key carries a scopes list controlling which endpoints it can access.\n    Keys are issued at one of two permission levels — full_access (default, all\n    scopes) or read_only (read scopes only). The authenticated scope list is\n    returned by postAuthValidateApiKey and\
  \ by getMe.\n- name: mcpOAuth\n  kind: oauth2\n  source: well-known/lev-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.lev.com/authorize\n    tokenUrl: https://auth.lev.com/oauth/token\nscopes:\n- scope: deals:read\n  description: Read access to deals and their sub-resources (financials, properties,\n    team, documents, vaults, checklists, memos, notes, indexed facts).\n  domain: deals\n  access: read\n  schemes:\n  - apiKeyScopes\n- scope: deals:write\n  description: Create, update, archive deals and write deal sub-resources including\n    notes, checklist tasks, and recorded index facts.\n  domain: deals\n  access: write\n  schemes:\n  - apiKeyScopes\n- scope: contacts:read\n  description: Read access to CRM contacts and contact notes.\n  domain: contacts\n  access: read\n  schemes:\n  - apiKeyScopes\n- scope: contacts:write\n  description: Create and update CRM contacts and contact notes.\n  domain: contacts\n  access: write\n\
  \  schemes:\n  - apiKeyScopes\n- scope: companies:read\n  description: Read access to CRM companies and company notes.\n  domain: companies\n  access: read\n  schemes:\n  - apiKeyScopes\n- scope: companies:write\n  description: Create and update CRM companies and company notes.\n  domain: companies\n  access: write\n  schemes:\n  - apiKeyScopes\n- scope: lenders:read\n  description: Read access to the lender directory, individual lender records, and\n    their lending programs. Read-only — the docs list no lenders:write counterpart.\n  domain: lenders\n  access: read\n  schemes:\n  - apiKeyScopes\n- scope: ai:actions\n  description: Gates AI-powered, credit-consuming actions separately from ordinary\n    reads and writes. Required by postContactsContactIdActionsUnlock, which reveals\n    an AI-recommended lender contact and charges credits.\n  domain: ai\n  access: action\n  schemes:\n  - apiKeyScopes\n- scope: openid\n  description: Standard OIDC scope requested by MCP clients during\
  \ the Auth0\n    authorization-code flow.\n  domain: oidc\n  access: identity\n  schemes:\n  - mcpOAuth\n- scope: email\n  description: Standard OIDC scope granting the user's email address to the MCP\n    client.\n  domain: oidc\n  access: identity\n  schemes:\n  - mcpOAuth\n- scope: offline_access\n  description: Requests a refresh token so the MCP client can silently refresh\n    without re-prompting the user.\n  domain: oidc\n  access: identity\n  schemes:\n  - mcpOAuth\nrelated:\n  authentication: authentication/lev-authentication.yml\n  well_known: well-known/lev-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lev/refs/heads/main/scopes/lev-scopes.yml
summary_line: 11 scopes · authorizationCode
tags:
- Company
- Commercial Real Estate
- Real Estate
- Proptech
- CRE Financing
- Lending
- CRM
- Artificial Intelligence
- AI Agents
- Deal Management
- Market Data
- Documents
token_urls:
- https://auth.lev.com/oauth/token
---
