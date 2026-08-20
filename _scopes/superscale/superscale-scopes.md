---
authorization_urls:
- https://superscale.ai/__clerk/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Superscale Scopes
name_suffix: OAuth Scopes
note: 'Read from the live OAuth discovery documents Superscale serves anonymously in front of its MCP server, not from an OpenAPI oauth2 flow block (there is no OpenAPI). Superscale publishes no human-readable scopes reference page — the discovery metadata is the only scope surface, so descriptions below are the standard OIDC / Clerk meanings of each identifier, marked as such. No Superscale-specific product scopes (create-ads, read-performance, publish, etc.) are advertised: the authorization server is a Clerk identity tenant and the scopes are identity scopes, with product entitlement enforced separately by subscription plan.'
overview: 'Superscale publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Superscale API on a user''s behalf.


  Tokens are issued from https://superscale.ai/__clerk/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Superscale
provider_slug: superscale
schemes:
- flows:
  - authorizationUrl: https://superscale.ai/__clerk/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://superscale.ai/__clerk/oauth/token
  issuer: https://superscale.ai/__clerk
  name: superscale-mcp-oauth2
  source: https://mcp.superscale.ai/.well-known/oauth-authorization-server
scope_count: 7
scope_names:
- openid
- profile
- email
- public_metadata
- private_metadata
- offline_access
- user:org:read
scopes:
- description: OIDC — request an ID token for the authenticating user (standard OIDC scope).
  flows:
  - authorizationCode
  scope: openid
- description: OIDC — basic profile claims (name) for the authenticating user (standard OIDC scope).
  flows:
  - authorizationCode
  scope: profile
- description: OIDC — the authenticating user's email address (standard OIDC scope).
  flows:
  - authorizationCode
  scope: email
- description: Clerk — read the user's public metadata object.
  flows:
  - authorizationCode
  scope: public_metadata
- description: Clerk — read the user's private metadata object.
  flows:
  - authorizationCode
  scope: private_metadata
- description: OAuth — issue a refresh token so the client can act without the user present.
  flows:
  - authorizationCode
  scope: offline_access
- description: Clerk — read the organizations the user belongs to (maps to the org_id claim).
  flows:
  - authorizationCode
  scope: user:org:read
slug: superscale-scopes
source_filename: superscale-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  https://mcp.superscale.ai/.well-known/oauth-authorization-server,\n  https://mcp.superscale.ai/.well-known/oauth-protected-resource/mcp\nnote: >-\n  Read from the live OAuth discovery documents Superscale serves anonymously in\n  front of its MCP server, not from an OpenAPI oauth2 flow block (there is no\n  OpenAPI). Superscale publishes no human-readable scopes reference page — the\n  discovery metadata is the only scope surface, so descriptions below are the\n  standard OIDC / Clerk meanings of each identifier, marked as such. No\n  Superscale-specific product scopes (create-ads, read-performance, publish,\n  etc.) are advertised: the authorization server is a Clerk identity tenant and\n  the scopes are identity scopes, with product entitlement enforced separately\n  by subscription plan.\ndocs: null\ndocs_note: >-\n  No scopes/permissions reference page exists. Searched the full 340KB docs\n  corpus (docs.superscale.ai/llms-full.txt)\
  \ — zero matches for \"scope\",\n  \"permission\" in an API-authorization sense.\nschemes:\n- name: superscale-mcp-oauth2\n  source: https://mcp.superscale.ai/.well-known/oauth-authorization-server\n  issuer: https://superscale.ai/__clerk\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://superscale.ai/__clerk/oauth/authorize\n    tokenUrl: https://superscale.ai/__clerk/oauth/token\nscopes:\n- scope: openid\n  description: OIDC — request an ID token for the authenticating user (standard OIDC scope).\n  flows: [authorizationCode]\n  advertised_by: [authorization-server]\n  standard: true\n- scope: profile\n  description: OIDC — basic profile claims (name) for the authenticating user (standard OIDC scope).\n  flows: [authorizationCode]\n  advertised_by: [authorization-server, protected-resource]\n  standard: true\n- scope: email\n  description: OIDC — the authenticating user's email address (standard OIDC scope).\n  flows: [authorizationCode]\n  advertised_by: [authorization-server,\
  \ protected-resource]\n  standard: true\n- scope: public_metadata\n  description: Clerk — read the user's public metadata object.\n  flows: [authorizationCode]\n  advertised_by: [authorization-server]\n  standard: false\n  vendor: Clerk\n- scope: private_metadata\n  description: Clerk — read the user's private metadata object.\n  flows: [authorizationCode]\n  advertised_by: [authorization-server]\n  standard: false\n  vendor: Clerk\n- scope: offline_access\n  description: OAuth — issue a refresh token so the client can act without the user present.\n  flows: [authorizationCode]\n  advertised_by: [authorization-server]\n  standard: true\n- scope: user:org:read\n  description: Clerk — read the organizations the user belongs to (maps to the org_id claim).\n  flows: [authorizationCode]\n  advertised_by: [authorization-server]\n  standard: false\n  vendor: Clerk\nresource_scopes:\n  resource: https://mcp.superscale.ai/mcp\n  scopes_supported: [profile, email]\n  note: >-\n    The protected-resource\
  \ document narrows to two of the seven scopes the\n    authorization server advertises. It declares\n    authorization_data_types_supported [oauth_scope] and accepts authorization\n    data in header or body.\ncoverage:\n  scopes_total: 7\n  product_specific: 0\n  identity_only: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superscale/refs/heads/main/scopes/superscale-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Company
- Artificial Intelligence
- Marketing
- Advertising
- Generative AI
- Creative
- AdTech
- Software-as-a-Service
- Agents
- MCP
- A2A
- Agent Skills
- Advertising Technology
- Video Generation
- Media Buying
token_urls:
- https://superscale.ai/__clerk/oauth/token
---
