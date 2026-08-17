---
authorization_urls:
- https://app.brand.ai/api/auth/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Brandai Scopes
name_suffix: OAuth Scopes
note: 'Derived from Brand.ai''s own live RFC 8414 authorization server metadata, not from an OpenAPI (Brand.ai publishes none) and not from documentation (Brand.ai publishes no developer docs). The `scopes_supported` array is the provider''s own published claim about its authorization surface. Descriptions below are NOT provider-supplied — Brand.ai publishes no scope reference page — so each carries an explicit description_source so a reader can tell the scope STRING (provider-published) from the gloss (ours, read against Brand.ai''s own product vocabulary on brand.ai/product/ and brand.ai/brand-os/). The scope names map cleanly onto the marketed Brand OS / Brand Studio objects: Brands, Brand Rules (the "machine-readable rules" of Brand Foundation), Brand Check, Artifacts and Projects.'
overview: 'Brand.ai publishes 13 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Brand.ai API on a user''s behalf.


  Tokens are issued from https://app.brand.ai/api/auth/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Brand.ai
provider_slug: brandai
schemes:
- flows:
  - authorizationUrl: https://app.brand.ai/api/auth/oauth2/authorize
    flow: authorizationCode
    pkce: S256
    refreshUrl: https://app.brand.ai/api/auth/oauth2/token
    tokenUrl: https://app.brand.ai/api/auth/oauth2/token
  name: OAuth2
  source: https://app.brand.ai/.well-known/oauth-authorization-server
  type: oauth2
scope_count: 13
scope_names:
- openid
- profile
- email
- offline_access
- mcp:identify
- brands:read
- brand_rules:read
- brand_checks:read
- brand_checks:write
- artifacts:read
- artifacts:write
- projects:write
- help:read
scopes:
- description: OpenID Connect — request an ID token.
  flows:
  - authorizationCode
  scope: openid
- description: Standard OIDC profile claims (name, given_name, family_name, picture).
  flows: []
  scope: profile
- description: Standard OIDC email + email_verified claims.
  flows: []
  scope: email
- description: Issue a refresh token so the client can act without the user present.
  flows: []
  scope: offline_access
- description: Identify the calling MCP client to the Brand.ai MCP server.
  flows: []
  scope: mcp:identify
- description: Read the brands (brandspaces) available to the authorizing user.
  flows: []
  scope: brands:read
- description: Read the machine-readable brand rules produced by Brand Foundation.
  flows: []
  scope: brand_rules:read
- description: Read Brand Check validation results and reports.
  flows: []
  scope: brand_checks:read
- description: Run a Brand Check — submit content for validation against brand rules.
  flows: []
  scope: brand_checks:write
- description: Read brand artifacts / assets in the library.
  flows: []
  scope: artifacts:read
- description: Create or update brand artifacts / assets.
  flows: []
  scope: artifacts:write
- description: Create or update Projects (briefs, research, team workspaces).
  flows: []
  scope: projects:write
- description: Read Brand.ai product help / guidance content.
  flows: []
  scope: help:read
slug: brandai-scopes
source_filename: brandai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://app.brand.ai/.well-known/oauth-authorization-server\ndocs: null\nnote: >-\n  Derived from Brand.ai's own live RFC 8414 authorization server metadata, not from\n  an OpenAPI (Brand.ai publishes none) and not from documentation (Brand.ai publishes\n  no developer docs). The `scopes_supported` array is the provider's own published\n  claim about its authorization surface. Descriptions below are NOT provider-supplied\n  — Brand.ai publishes no scope reference page — so each carries an explicit\n  description_source so a reader can tell the scope STRING (provider-published) from\n  the gloss (ours, read against Brand.ai's own product vocabulary on brand.ai/product/\n  and brand.ai/brand-os/). The scope names map cleanly onto the marketed Brand OS /\n  Brand Studio objects: Brands, Brand Rules (the \"machine-readable rules\" of Brand\n  Foundation), Brand Check, Artifacts and Projects.\nschemes:\n- name: OAuth2\n  type: oauth2\n\
  \  source: https://app.brand.ai/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.brand.ai/api/auth/oauth2/authorize\n    tokenUrl: https://app.brand.ai/api/auth/oauth2/token\n    refreshUrl: https://app.brand.ai/api/auth/oauth2/token\n    pkce: S256\nscopes:\n- scope: openid\n  description: OpenID Connect — request an ID token.\n  description_source: standard\n  flows: [authorizationCode]\n- scope: profile\n  description: Standard OIDC profile claims (name, given_name, family_name, picture).\n  description_source: standard\n- scope: email\n  description: Standard OIDC email + email_verified claims.\n  description_source: standard\n- scope: offline_access\n  description: Issue a refresh token so the client can act without the user present.\n  description_source: standard\n- scope: mcp:identify\n  description: Identify the calling MCP client to the Brand.ai MCP server.\n  description_source: apievangelist-gloss\n- scope: brands:read\n\
  \  description: Read the brands (brandspaces) available to the authorizing user.\n  description_source: apievangelist-gloss\n- scope: brand_rules:read\n  description: Read the machine-readable brand rules produced by Brand Foundation.\n  description_source: apievangelist-gloss\n- scope: brand_checks:read\n  description: Read Brand Check validation results and reports.\n  description_source: apievangelist-gloss\n- scope: brand_checks:write\n  description: Run a Brand Check — submit content for validation against brand rules.\n  description_source: apievangelist-gloss\n- scope: artifacts:read\n  description: Read brand artifacts / assets in the library.\n  description_source: apievangelist-gloss\n- scope: artifacts:write\n  description: Create or update brand artifacts / assets.\n  description_source: apievangelist-gloss\n- scope: projects:write\n  description: Create or update Projects (briefs, research, team workspaces).\n  description_source: apievangelist-gloss\n- scope: help:read\n\
  \  description: Read Brand.ai product help / guidance content.\n  description_source: apievangelist-gloss\nsummary:\n  scope_count: 13\n  standard_oidc: 4\n  product_scopes: 9\n  read_write_split:\n    read: 5\n    write: 3\n  asymmetry_note: >-\n    brands and brand_rules are read-only (no :write scope is offered) while\n    brand_checks, artifacts and projects are writable — the authorization model\n    lets an agent produce and validate work but not rewrite the brand definition\n    itself. projects has a :write scope with no matching :read scope.\nx-evidence:\n- url: https://app.brand.ai/.well-known/oauth-authorization-server\n  http_status: 200\n  fetched: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brandai/refs/heads/main/scopes/brandai-scopes.yml
summary_line: 13 scopes · authorizationCode
tags:
- Company
- Brand Management
- Artificial Intelligence
- Marketing
- SaaS
- Brand Operating System
- AI Agents
- Design
- Model Context Protocol
- Brand Governance
- Brand Intelligence
token_urls:
- https://app.brand.ai/api/auth/oauth2/token
---
