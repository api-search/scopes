---
authorization_urls:
- https://login.abatable.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Abatable Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Abatable publishes 14 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Abatable API on a user''s behalf.


  Tokens are issued from https://login.abatable.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Abatable
provider_slug: abatable
schemes:
- flows:
  - authorizationUrl: https://login.abatable.com/authorize
    flow: authorizationCode
    tokenUrl: https://login.abatable.com/oauth/token
  issuer: https://login.abatable.com/
  name: Auth0 OIDC
  source: well-known/abatable-login-openid-configuration.json
- issuer: https://abatable.cloudflareaccess.com
  name: Cloudflare Access (MCP)
  scopes_supported_published: false
  source: well-known/abatable-mcp-oauth-authorization-server.json
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
- phone
- address
- created_at
- identities
scopes:
- description: OIDC authentication; issue an ID token
  flows:
  - authorizationCode
  scope: openid
- description: Basic profile claims
  flows:
  - authorizationCode
  scope: profile
- description: Email address claim
  flows:
  - authorizationCode
  scope: email
- description: Email verification status claim
  flows:
  - authorizationCode
  scope: email_verified
- description: Issue a refresh token
  flows:
  - authorizationCode
  scope: offline_access
- description: Full name claim
  flows:
  - authorizationCode
  scope: name
- description: Given name claim
  flows:
  - authorizationCode
  scope: given_name
- description: Family name claim
  flows:
  - authorizationCode
  scope: family_name
- description: Nickname claim
  flows:
  - authorizationCode
  scope: nickname
- description: Profile picture claim
  flows:
  - authorizationCode
  scope: picture
- description: Phone number claim
  flows:
  - authorizationCode
  scope: phone
- description: Address claim
  flows:
  - authorizationCode
  scope: address
- description: Account creation timestamp claim
  flows:
  - authorizationCode
  scope: created_at
- description: Linked identity provider records claim
  flows:
  - authorizationCode
  scope: identities
slug: abatable-scopes
source_filename: abatable-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: https://login.abatable.com/.well-known/openid-configuration\ndocs: null\ndocs_note: >-\n  Abatable publishes no scopes or permissions reference. The scopes below are the\n  `scopes_supported` array its Auth0 OIDC discovery document advertises — the standard OIDC claim\n  scopes plus Auth0's profile-claim scopes. They are identity scopes, not API authorisation\n  scopes: no Abatable-specific resource scope (read:*, write:*) is published anywhere, and the\n  Cloudflare Access authorization server that guards the MCP endpoint publishes no\n  `scopes_supported` at all.\nschemes:\n- name: Auth0 OIDC\n  source: well-known/abatable-login-openid-configuration.json\n  issuer: https://login.abatable.com/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.abatable.com/authorize\n    tokenUrl: https://login.abatable.com/oauth/token\n- name: Cloudflare Access (MCP)\n  source: well-known/abatable-mcp-oauth-authorization-server.json\n\
  \  issuer: https://abatable.cloudflareaccess.com\n  scopes_supported_published: false\nscopes:\n- {scope: openid, description: OIDC authentication; issue an ID token, flows: [authorizationCode], sources: [well-known/abatable-login-openid-configuration.json]}\n- {scope: profile, description: Basic profile claims, flows: [authorizationCode], sources: [well-known/abatable-login-openid-configuration.json]}\n- {scope: email, description: Email address claim, flows: [authorizationCode], sources: [well-known/abatable-login-openid-configuration.json]}\n- {scope: email_verified, description: Email verification status claim, flows: [authorizationCode], sources: [well-known/abatable-login-openid-configuration.json]}\n- {scope: offline_access, description: Issue a refresh token, flows: [authorizationCode], sources: [well-known/abatable-login-openid-configuration.json]}\n- {scope: name, description: Full name claim, flows: [authorizationCode], sources: [well-known/abatable-login-openid-configuration.json]}\n\
  - {scope: given_name, description: Given name claim, flows: [authorizationCode], sources: [well-known/abatable-login-openid-configuration.json]}\n- {scope: family_name, description: Family name claim, flows: [authorizationCode], sources: [well-known/abatable-login-openid-configuration.json]}\n- {scope: nickname, description: Nickname claim, flows: [authorizationCode], sources: [well-known/abatable-login-openid-configuration.json]}\n- {scope: picture, description: Profile picture claim, flows: [authorizationCode], sources: [well-known/abatable-login-openid-configuration.json]}\n- {scope: phone, description: Phone number claim, flows: [authorizationCode], sources: [well-known/abatable-login-openid-configuration.json]}\n- {scope: address, description: Address claim, flows: [authorizationCode], sources: [well-known/abatable-login-openid-configuration.json]}\n- {scope: created_at, description: Account creation timestamp claim, flows: [authorizationCode], sources: [well-known/abatable-login-openid-configuration.json]}\n\
  - {scope: identities, description: Linked identity provider records claim, flows: [authorizationCode], sources: [well-known/abatable-login-openid-configuration.json]}\nresource_scopes:\n  published: false\n  note: >-\n    No resource/permission scope vocabulary is published. An integrator cannot tell from any public\n    surface what an Abatable access token is authorised to do.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abatable/refs/heads/main/scopes/abatable-scopes.yml
summary_line: 14 scopes · authorizationCode
tags:
- Carbon Markets
- Carbon Credits
- Carbon Offsets
- Environmental Assets
- Voluntary Carbon Market
- CORSIA
- Climate
- Sustainability
- Net Zero
- Procurement
- Market Intelligence
- Due Diligence
- ESG
- MCP
token_urls:
- https://login.abatable.com/oauth/token
---
