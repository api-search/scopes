---
api_specs:
- filename: sitefire-book-demo-api-openapi.yml
  format: yaml
  label: Sitefire Book Demo API
  slug: sitefire-book-demo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitefire/refs/heads/main/openapi/sitefire-book-demo-api-openapi.yml
authorization_urls:
- https://qhfesxmsojjleewjufcn.supabase.co/auth/v1/oauth/authorize
description: ''
docs: https://sitefire.ai/docs/mcp.md
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Sitefire Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Sitefire publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Sitefire API on a user''s behalf.


  Tokens are issued from https://qhfesxmsojjleewjufcn.supabase.co/auth/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Sitefire
provider_slug: sitefire
schemes:
- flows:
  - authorizationUrl: https://qhfesxmsojjleewjufcn.supabase.co/auth/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://qhfesxmsojjleewjufcn.supabase.co/auth/v1/oauth/token
  name: mcp-oauth
  source: https://app.sitefire.ai/api/mcp/oauth-metadata
scope_count: 5
scope_names:
- openid
- profile
- email
- phone
- offline_access
scopes:
- description: OpenID Connect sign-in; issues an ID token identifying the Sitefire user.
  flows:
  - authorizationCode
  scope: openid
- description: Basic profile claims (name, picture, preferred_username, updated_at).
  flows:
  - authorizationCode
  scope: profile
- description: Email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Phone number and phone_number_verified claim.
  flows:
  - authorizationCode
  scope: phone
- description: Issues a refresh token so an agent can keep a long-lived MCP session.
  flows:
  - authorizationCode
  scope: offline_access
slug: sitefire-scopes
source_filename: sitefire-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://qhfesxmsojjleewjufcn.supabase.co/auth/v1/.well-known/oauth-authorization-server\ndocs: https://sitefire.ai/docs/mcp.md\nnotes: >-\n  Sitefire publishes no scope or permission reference page. The scopes below were\n  read from the RFC 8414 authorization-server metadata that Sitefire's own MCP\n  protected-resource document points at. They are the identity scopes of the\n  Supabase authorization server Sitefire delegates sign-in to - openid/profile/\n  email/phone/offline_access - not Sitefire-defined resource scopes. In other\n  words the MCP server authenticates the user but does not appear to publish a\n  granular authorization surface: there is no read-vs-write split between the\n  seven read tools and the three write tools (create_action, write_article) in\n  mcp/sitefire-mcp.yml. Recorded as an honest measurement of what is published,\n  not as a claim that Sitefire ships scoped authorization.\n  derive-oauth-scopes.py\
  \ returned zero, because the only OpenAPI in the repo\n  declares no oauth2 securityScheme.\nresource: https://app.sitefire.ai/api/mcp\nschemes:\n- name: mcp-oauth\n  source: https://app.sitefire.ai/api/mcp/oauth-metadata\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://qhfesxmsojjleewjufcn.supabase.co/auth/v1/oauth/authorize\n    tokenUrl: https://qhfesxmsojjleewjufcn.supabase.co/auth/v1/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect sign-in; issues an ID token identifying the Sitefire user.\n  flows: [authorizationCode]\n  sources: [authorization-server-metadata]\n  provider_defined: false\n- scope: profile\n  description: Basic profile claims (name, picture, preferred_username, updated_at).\n  flows: [authorizationCode]\n  sources: [authorization-server-metadata]\n  provider_defined: false\n- scope: email\n  description: Email address and email_verified claim.\n  flows: [authorizationCode]\n  sources: [authorization-server-metadata]\n  provider_defined:\
  \ false\n- scope: phone\n  description: Phone number and phone_number_verified claim.\n  flows: [authorizationCode]\n  sources: [authorization-server-metadata]\n  provider_defined: false\n- scope: offline_access\n  description: Issues a refresh token so an agent can keep a long-lived MCP session.\n  flows: [authorizationCode]\n  sources: [authorization-server-metadata]\n  provider_defined: false\nresource_scopes: []\nresource_scopes_note: >-\n  No Sitefire-defined resource scopes were found. The protected-resource\n  metadata at /api/mcp/oauth-metadata carries no scopes_supported member, and no\n  scope reference page exists in the docs or in the sitefire-ai/skills repo.\nx-evidence:\n- url: https://qhfesxmsojjleewjufcn.supabase.co/auth/v1/.well-known/oauth-authorization-server\n  http_status: 200\n  checked: '2026-08-13'\n- url: https://app.sitefire.ai/api/mcp/oauth-metadata\n  http_status: 200\n  checked: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sitefire/refs/heads/main/scopes/sitefire-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Company
- Generative Engine Optimization
- AI Visibility
- Marketing
- SEO
- Analytics
- Artificial Intelligence
- Content Generation
- MCP
- Agents
token_urls:
- https://qhfesxmsojjleewjufcn.supabase.co/auth/v1/oauth/token
---
