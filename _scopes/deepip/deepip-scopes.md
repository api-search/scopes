---
authorization_urls:
- https://auth.deepip.ai/authorize
- https://app.deepip.ai/mcp/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Deepip Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'DeepIP publishes 14 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the DeepIP API on a user''s behalf.


  Tokens are issued from https://auth.deepip.ai/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: DeepIP
provider_slug: deepip
schemes:
- flows:
  - authorizationUrl: https://auth.deepip.ai/authorize
    flow: authorizationCode
    tokenUrl: https://auth.deepip.ai/oauth/token
  issuer: https://auth.deepip.ai/
  name: deepip-auth0-oidc
  source: well-known/deepip-auth-openid-configuration.json
- flows:
  - authorizationUrl: https://app.deepip.ai/mcp/authorize
    flow: authorizationCode
    tokenUrl: https://app.deepip.ai/mcp/token
  issuer: https://app.deepip.ai/
  name: mcp-oauth2
  note: The MCP authorization server advertises NO scopes_supported array. An agent connecting to https://app.deepip.ai/mcp therefore cannot discover, before the consent screen, what permissions it is being granted over a patent portfolio. This is a real gap, recorded rather than filled in.
  scopes_declared: false
  source: well-known/deepip-app-oauth-authorization-server.json
scope_count: 14
scope_names:
- openid
- profile
- email
- email_verified
- offline_access
- name
- given_name
- family_name
- nickname
- picture
- created_at
- identities
- phone
- address
scopes:
- description: Standard OIDC — issue an ID token for the authenticated user.
  flows:
  - authorizationCode
  scope: openid
- description: Standard OIDC — basic profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Standard OIDC — email address claim.
  flows:
  - authorizationCode
  scope: email
- description: Standard OIDC — whether the email address is verified.
  flows:
  - authorizationCode
  scope: email_verified
- description: Issue a refresh token for long-lived access.
  flows:
  - authorizationCode
  scope: offline_access
- description: Standard OIDC claim scope — full name.
  flows:
  - authorizationCode
  scope: name
- description: Standard OIDC claim scope — given name.
  flows:
  - authorizationCode
  scope: given_name
- description: Standard OIDC claim scope — family name.
  flows:
  - authorizationCode
  scope: family_name
- description: Standard OIDC claim scope — nickname.
  flows:
  - authorizationCode
  scope: nickname
- description: Standard OIDC claim scope — profile picture URL.
  flows:
  - authorizationCode
  scope: picture
- description: Auth0 claim scope — account creation timestamp.
  flows:
  - authorizationCode
  scope: created_at
- description: Auth0 claim scope — linked identity providers.
  flows:
  - authorizationCode
  scope: identities
- description: Standard OIDC claim scope — phone number.
  flows:
  - authorizationCode
  scope: phone
- description: Standard OIDC claim scope — postal address.
  flows:
  - authorizationCode
  scope: address
slug: deepip-scopes
source_filename: deepip-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: >-\n  https://auth.deepip.ai/.well-known/openid-configuration,\n  https://app.deepip.ai/.well-known/oauth-authorization-server\ndocs: null\ndocs_note: >-\n  DeepIP publishes no scopes/permissions reference page. Both scope facts below\n  were read from discovery metadata the provider serves anonymously.\nschemes:\n- name: deepip-auth0-oidc\n  source: well-known/deepip-auth-openid-configuration.json\n  issuer: https://auth.deepip.ai/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.deepip.ai/authorize\n    tokenUrl: https://auth.deepip.ai/oauth/token\n- name: mcp-oauth2\n  source: well-known/deepip-app-oauth-authorization-server.json\n  issuer: https://app.deepip.ai/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.deepip.ai/mcp/authorize\n    tokenUrl: https://app.deepip.ai/mcp/token\n  scopes_declared: false\n  note: >-\n    The MCP authorization server advertises NO scopes_supported\
  \ array. An agent\n    connecting to https://app.deepip.ai/mcp therefore cannot discover, before the\n    consent screen, what permissions it is being granted over a patent portfolio.\n    This is a real gap, recorded rather than filled in.\nscopes:\n- scope: openid\n  description: Standard OIDC — issue an ID token for the authenticated user.\n  flows: [authorizationCode]\n  sources: [well-known/deepip-auth-openid-configuration.json]\n  kind: identity\n- scope: profile\n  description: Standard OIDC — basic profile claims.\n  flows: [authorizationCode]\n  sources: [well-known/deepip-auth-openid-configuration.json]\n  kind: identity\n- scope: email\n  description: Standard OIDC — email address claim.\n  flows: [authorizationCode]\n  sources: [well-known/deepip-auth-openid-configuration.json]\n  kind: identity\n- scope: email_verified\n  description: Standard OIDC — whether the email address is verified.\n  flows: [authorizationCode]\n  sources: [well-known/deepip-auth-openid-configuration.json]\n\
  \  kind: identity\n- scope: offline_access\n  description: Issue a refresh token for long-lived access.\n  flows: [authorizationCode]\n  sources: [well-known/deepip-auth-openid-configuration.json]\n  kind: identity\n- scope: name\n  description: Standard OIDC claim scope — full name.\n  flows: [authorizationCode]\n  sources: [well-known/deepip-auth-openid-configuration.json]\n  kind: identity\n- scope: given_name\n  description: Standard OIDC claim scope — given name.\n  flows: [authorizationCode]\n  sources: [well-known/deepip-auth-openid-configuration.json]\n  kind: identity\n- scope: family_name\n  description: Standard OIDC claim scope — family name.\n  flows: [authorizationCode]\n  sources: [well-known/deepip-auth-openid-configuration.json]\n  kind: identity\n- scope: nickname\n  description: Standard OIDC claim scope — nickname.\n  flows: [authorizationCode]\n  sources: [well-known/deepip-auth-openid-configuration.json]\n  kind: identity\n- scope: picture\n  description: Standard\
  \ OIDC claim scope — profile picture URL.\n  flows: [authorizationCode]\n  sources: [well-known/deepip-auth-openid-configuration.json]\n  kind: identity\n- scope: created_at\n  description: Auth0 claim scope — account creation timestamp.\n  flows: [authorizationCode]\n  sources: [well-known/deepip-auth-openid-configuration.json]\n  kind: identity\n- scope: identities\n  description: Auth0 claim scope — linked identity providers.\n  flows: [authorizationCode]\n  sources: [well-known/deepip-auth-openid-configuration.json]\n  kind: identity\n- scope: phone\n  description: Standard OIDC claim scope — phone number.\n  flows: [authorizationCode]\n  sources: [well-known/deepip-auth-openid-configuration.json]\n  kind: identity\n- scope: address\n  description: Standard OIDC claim scope — postal address.\n  flows: [authorizationCode]\n  sources: [well-known/deepip-auth-openid-configuration.json]\n  kind: identity\nsummary:\n  total_scopes: 14\n  identity_scopes: 14\n  resource_scopes: 0\n  note:\
  \ >-\n    Every published scope is an OIDC identity/claim scope from the Auth0 tenant.\n    DeepIP publishes ZERO resource scopes — nothing that describes read or write\n    access to inventions, drafts, office actions, or portfolios.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deepip/refs/heads/main/scopes/deepip-scopes.yml
summary_line: 14 scopes · authorizationCode
tags:
- Company
- Intellectual Property
- Patents
- Legal Tech
- Artificial Intelligence
- Patent Drafting
- IP Management
- Document Automation
- Security
- MCP
- Agents
- Prior Art Search
token_urls:
- https://auth.deepip.ai/oauth/token
- https://app.deepip.ai/mcp/token
---
