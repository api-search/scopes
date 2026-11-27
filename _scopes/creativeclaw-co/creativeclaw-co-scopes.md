---
api_specs:
- filename: creativeclaw-co-health-api-openapi.yml
  format: yaml
  label: CreativeClaw Health API
  slug: creativeclaw-co-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creativeclaw-co/openapi/creativeclaw-co-health-api-openapi.yml
- filename: creativeclaw-co-mcp-api-openapi.yml
  format: yaml
  label: CreativeClaw MCP API
  slug: creativeclaw-co-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creativeclaw-co/openapi/creativeclaw-co-mcp-api-openapi.yml
- filename: creativeclaw-co-oauth-api-openapi.yml
  format: yaml
  label: CreativeClaw OAuth API
  slug: creativeclaw-co-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creativeclaw-co/openapi/creativeclaw-co-oauth-api-openapi.yml
authorization_urls:
- https://clerk.creativeclaw.co/oauth/authorize
description: ''
docs: https://creativeclaw.co/auth.md
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: CreativeClaw Scopes
name_suffix: OAuth Scopes
note: 'Docs: "Scopes are exactly `profile email`. Never request `openid` — Clerk rejects that scope for dynamically registered MCP clients."'
overview: 'CreativeClaw publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the CreativeClaw API on a user''s behalf.


  Tokens are issued from https://clerk.creativeclaw.co/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CreativeClaw
provider_slug: creativeclaw-co
schemes:
- description: OAuth 2.1 authorization code with PKCE S256. Dynamic client registration is supported. Request only `profile` and `email`.
  flows:
  - authorizationUrl: https://clerk.creativeclaw.co/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://clerk.creativeclaw.co/oauth/token
  name: oauth2
  source: openapi/creativeclaw-co-openapi.yml
scope_count: 2
scope_names:
- email
- profile
scopes:
- description: Read the authenticated user email
  flows:
  - authorizationCode
  scope: email
- description: Read the authenticated user profile
  flows:
  - authorizationCode
  scope: profile
slug: creativeclaw-co-scopes
source_filename: creativeclaw-co-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://creativeclaw.co/auth.md\nschemes:\n- name: oauth2\n  source: openapi/creativeclaw-co-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://clerk.creativeclaw.co/oauth/authorize\n    tokenUrl: https://clerk.creativeclaw.co/oauth/token\n  description: OAuth 2.1 authorization code with PKCE S256. Dynamic client registration is supported. Request only `profile`\n    and `email`.\nscopes:\n- scope: email\n  description: Read the authenticated user email\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/creativeclaw-co-openapi.yml\n- scope: profile\n  description: Read the authenticated user profile\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/creativeclaw-co-openapi.yml\nderived_from: openapi/creativeclaw-co-openapi.yml\ndocs: https://creativeclaw.co/auth.md\nnote: 'Docs: \"Scopes are exactly `profile email`. Never request `openid` — Clerk rejects that scope for dynamically\
  \ registered\n  MCP clients.\"'\n"
source_yaml_url: https://artifacts.apis.io/creativeclaw-co/scopes/creativeclaw-co-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Artificial Intelligence
- Generative AI
- Image Generation
- Video Generation
- Audio
- MCP
- Marketing
token_bound: false
token_urls:
- https://clerk.creativeclaw.co/oauth/token
---
