---
authorization_urls:
- https://clerk.madethis.com/oauth/authorize
description: ''
docs: https://clerk.com/docs/oauth/scoped-access
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Madethis Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'MadeThis publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the MadeThis API on a user''s behalf.


  Tokens are issued from https://clerk.madethis.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: MadeThis
provider_slug: madethis
schemes:
- flows:
  - authorizationUrl: https://clerk.madethis.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://clerk.madethis.com/oauth/token
  name: MadeThisOAuth2
  source: well-known/madethis-oauth-authorization-server.json
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
- description: Request an ID token — the OpenID Connect base scope.
  flows:
  - authorizationCode
  scope: openid
- description: Read the signed-in user's profile claims (name, given_name, family_name, preferred_username, picture).
  flows:
  - authorizationCode
  scope: profile
- description: Read the signed-in user's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Read the user's public metadata on the MadeThis Clerk instance.
  flows:
  - authorizationCode
  scope: public_metadata
- description: Read the user's private metadata on the MadeThis Clerk instance.
  flows:
  - authorizationCode
  scope: private_metadata
- description: Issue a refresh token so the client can act after the access token expires.
  flows:
  - authorizationCode
  scope: offline_access
- description: Read the organization membership of the signed-in user (org_id claim).
  flows:
  - authorizationCode
  scope: user:org:read
slug: madethis-scopes
source_filename: madethis-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://clerk.madethis.com/.well-known/oauth-authorization-server\ndocs: https://clerk.com/docs/oauth/scoped-access\nscope_note: >-\n  Read verbatim from the `scopes_supported` array published by MadeThis's own OAuth 2.0\n  authorization-server metadata (RFC 8414) at clerk.madethis.com. These are the scopes an\n  OAuth client registered against MadeThis's Clerk identity instance can request when a\n  MadeThis user signs in. They are Clerk's standard scoped-access set, not scopes over a\n  MadeThis product API — MadeThis publishes no API reference and no scope documentation of\n  its own. Descriptions below are stated in the terms the OIDC/OAuth specifications and\n  Clerk's scoped-access reference define; MadeThis publishes none.\nschemes:\n- name: MadeThisOAuth2\n  source: well-known/madethis-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://clerk.madethis.com/oauth/authorize\n\
  \    tokenUrl: https://clerk.madethis.com/oauth/token\nscopes:\n- scope: openid\n  description: Request an ID token — the OpenID Connect base scope.\n  flows: [authorizationCode]\n  sources: [well-known/madethis-oauth-authorization-server.json, well-known/madethis-openid-configuration.json]\n- scope: profile\n  description: Read the signed-in user's profile claims (name, given_name, family_name, preferred_username, picture).\n  flows: [authorizationCode]\n  sources: [well-known/madethis-oauth-authorization-server.json, well-known/madethis-openid-configuration.json]\n- scope: email\n  description: Read the signed-in user's email address and email_verified claim.\n  flows: [authorizationCode]\n  sources: [well-known/madethis-oauth-authorization-server.json, well-known/madethis-openid-configuration.json]\n- scope: public_metadata\n  description: Read the user's public metadata on the MadeThis Clerk instance.\n  flows: [authorizationCode]\n  sources: [well-known/madethis-oauth-authorization-server.json,\
  \ well-known/madethis-openid-configuration.json]\n- scope: private_metadata\n  description: Read the user's private metadata on the MadeThis Clerk instance.\n  flows: [authorizationCode]\n  sources: [well-known/madethis-oauth-authorization-server.json, well-known/madethis-openid-configuration.json]\n- scope: offline_access\n  description: Issue a refresh token so the client can act after the access token expires.\n  flows: [authorizationCode]\n  sources: [well-known/madethis-oauth-authorization-server.json, well-known/madethis-openid-configuration.json]\n- scope: 'user:org:read'\n  description: Read the organization membership of the signed-in user (org_id claim).\n  flows: [authorizationCode]\n  sources: [well-known/madethis-oauth-authorization-server.json, well-known/madethis-openid-configuration.json]\nsummary:\n  scope_count: 7\n  flows: [authorizationCode]\n  pkce_required_methods: [S256]\nx-evidence:\n- url: https://clerk.madethis.com/.well-known/oauth-authorization-server\n  http_status:\
  \ 200\n- url: https://clerk.madethis.com/.well-known/openid-configuration\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/madethis/refs/heads/main/scopes/madethis-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Company
- Artificial Intelligence
- AI Agents
- Business Automation
- Software-as-a-Service
- Marketing Automation
- Startup Tools
- Y Combinator
- No-Code
- Website Builder
- E-Commerce
- Small Business
- AI Employees
token_urls:
- https://clerk.madethis.com/oauth/token
---
