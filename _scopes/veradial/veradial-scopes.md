---
api_specs:
- filename: veradial-openapi-generated.yml
  format: yaml
  label: VeraDial Zapier Integration API
  slug: zapier-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veradial/refs/heads/main/openapi/_ae-authored/veradial-openapi-generated.yml
authorization_urls:
- https://rrmjstsbidgkqibvzvzo.supabase.co/auth/v1/oauth/authorize
description: ''
docs: https://veradial.com/for-agents
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Veradial Scopes
name_suffix: OAuth Scopes
note: The MCP server advertises only OpenID Connect identity scopes; access is read-only and scoped to the signed-in customer's own account rather than by fine-grained scopes.
overview: 'VeraDial publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the VeraDial API on a user''s behalf.


  Tokens are issued from https://rrmjstsbidgkqibvzvzo.supabase.co/auth/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: VeraDial
provider_slug: veradial
schemes:
- flows:
  - authorizationUrl: https://rrmjstsbidgkqibvzvzo.supabase.co/auth/v1/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://rrmjstsbidgkqibvzvzo.supabase.co/auth/v1/oauth/token
  name: mcpOAuth
  source: well-known/api-veradial-com-oauth-authorization-server.json
scope_count: 3
scope_names:
- openid
- email
- profile
scopes:
- description: OpenID Connect sign-in with the customer's VeraDial login.
  flows:
  - authorizationCode
  scope: openid
- description: The signed-in customer's email address.
  flows:
  - authorizationCode
  scope: email
- description: The signed-in customer's basic profile.
  flows:
  - authorizationCode
  scope: profile
slug: veradial-scopes
source_filename: veradial-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: searched\nsource: https://api.veradial.com/.well-known/oauth-protected-resource\ndocs: https://veradial.com/for-agents\nnote: The MCP server advertises only OpenID Connect identity scopes; access is read-only and scoped to the\n  signed-in customer's own account rather than by fine-grained scopes.\nschemes:\n- name: mcpOAuth\n  source: well-known/api-veradial-com-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://rrmjstsbidgkqibvzvzo.supabase.co/auth/v1/oauth/authorize\n    tokenUrl: https://rrmjstsbidgkqibvzvzo.supabase.co/auth/v1/oauth/token\n    pkce: S256\nscopes:\n- scope: openid\n  description: OpenID Connect sign-in with the customer's VeraDial login.\n  flows: [authorizationCode]\n  sources: [well-known/api-veradial-com-oauth-protected-resource.json]\n- scope: email\n  description: The signed-in customer's email address.\n  flows: [authorizationCode]\n  sources: [well-known/api-veradial-com-oauth-protected-resource.json]\n\
  - scope: profile\n  description: The signed-in customer's basic profile.\n  flows: [authorizationCode]\n  sources: [well-known/api-veradial-com-oauth-protected-resource.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veradial/refs/heads/main/scopes/veradial-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- AI Receptionist
- Business Phone
- Telephony
- Voice AI
- SMS
- Webhook
- MCP
- Small Business
token_urls:
- https://rrmjstsbidgkqibvzvzo.supabase.co/auth/v1/oauth/token
---
