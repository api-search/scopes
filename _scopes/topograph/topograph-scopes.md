---
api_specs:
- filename: topograph-openapi-original.json
  format: json
  label: Topograph API
  slug: topograph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/topograph/refs/heads/main/openapi/topograph-openapi-original.json
- filename: topograph-x402-openapi.json
  format: json
  label: Topograph x402 (agentic commerce)
  slug: topograph-x402-agentic-commerce
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/topograph/refs/heads/main/openapi/topograph-x402-openapi.json
authorization_urls: []
description: ''
docs: https://topograph.co/developers/mcp
flows:
- authorizationCode
- refreshToken
kind: oauth-scopes
layout: scope
method: searched
name: Topograph Scopes
name_suffix: OAuth Scopes
note: The Topograph REST API authenticates with an x-api-key header and declares no OAuth2 scopes. These OAuth 2.1 / OIDC scopes govern the designer / MCP surface, whose authorization server is Clerk (clerk.topograph.co). Captured verbatim from the RFC 8414 metadata.
overview: 'Topograph publishes 7 OAuth 2.0 scopes via the authorizationCode and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Topograph API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Topograph
provider_slug: topograph
schemes:
- authorizationUrl: https://clerk.topograph.co/oauth/authorize
  flows:
  - authorizationCode
  - refreshToken
  issuer: https://clerk.topograph.co
  name: OAuth2.1
  pkce: S256
  tokenUrl: https://clerk.topograph.co/oauth/token
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
- description: OpenID Connect authentication; issue an ID token.
  flows: []
  scope: openid
- description: Access to the user's basic profile claims.
  flows: []
  scope: profile
- description: Access to the user's email address.
  flows: []
  scope: email
- description: Read the user's public metadata.
  flows: []
  scope: public_metadata
- description: Read the user's private metadata.
  flows: []
  scope: private_metadata
- description: Issue a refresh token for offline access.
  flows: []
  scope: offline_access
- description: Read the user's organization membership.
  flows: []
  scope: user:org:read
slug: topograph-scopes
source_filename: topograph-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://api.topograph.co/.well-known/oauth-authorization-server\ndocs: https://topograph.co/developers/mcp\nnote: >-\n  The Topograph REST API authenticates with an x-api-key header and declares no OAuth2 scopes.\n  These OAuth 2.1 / OIDC scopes govern the designer / MCP surface, whose authorization server is\n  Clerk (clerk.topograph.co). Captured verbatim from the RFC 8414 metadata.\nschemes:\n- name: OAuth2.1\n  issuer: https://clerk.topograph.co\n  authorizationUrl: https://clerk.topograph.co/oauth/authorize\n  tokenUrl: https://clerk.topograph.co/oauth/token\n  flows: [authorizationCode, refreshToken]\n  pkce: S256\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token.\n- scope: profile\n  description: Access to the user's basic profile claims.\n- scope: email\n  description: Access to the user's email address.\n- scope: public_metadata\n  description: Read the user's public metadata.\n\
  - scope: private_metadata\n  description: Read the user's private metadata.\n- scope: offline_access\n  description: Issue a refresh token for offline access.\n- scope: user:org:read\n  description: Read the user's organization membership.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/topograph/refs/heads/main/scopes/topograph-scopes.yml
summary_line: 7 scopes · authorizationCode/refreshToken
tags:
- Company
- KYB
- Company Data
- Business Registers
- Compliance
- Identity Verification
- Beneficial Ownership
- AML
- Due Diligence
- Fintech
token_urls: []
---
