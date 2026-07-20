---
authorization_urls:
- https://sso.alien-api.com/oauth/authorize
description: ''
docs: https://docs.alien.org/sso-guide/oauth2-clients
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Alien Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Alien publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Alien API on a user''s behalf.


  Tokens are issued from https://sso.alien-api.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Alien
provider_slug: alien
schemes:
- flows:
  - authorizationUrl: https://sso.alien-api.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://sso.alien-api.com/oauth/token
  name: OAuth2
  source: https://sso.alien-api.com/.well-known/oauth-authorization-server
scope_count: 1
scope_names:
- openid
scopes:
- description: OpenID Connect authentication. Returns a verified, unique-human subject (sub) tied to an Alien ID without exposing name, email, or documents.
  flows:
  - authorizationCode
  scope: openid
slug: alien-scopes
source_filename: alien-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://sso.alien-api.com/.well-known/openid-configuration\ndocs: https://docs.alien.org/sso-guide/oauth2-clients\nschemes:\n- name: OAuth2\n  source: https://sso.alien-api.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sso.alien-api.com/oauth/authorize\n    tokenUrl: https://sso.alien-api.com/oauth/token\nscopes:\n- scope: openid\n  description: >-\n    OpenID Connect authentication. Returns a verified, unique-human subject\n    (sub) tied to an Alien ID without exposing name, email, or documents.\n  flows: [authorizationCode]\n  sources: [https://sso.alien-api.com/.well-known/openid-configuration]\nnotes: >-\n  The authorization server advertises a single supported scope (openid) in its\n  discovery document (scopes_supported). Alien SSO deliberately minimizes scope\n  surface: it asserts proof-of-humanity, not personal-data claims.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alien/refs/heads/main/scopes/alien-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Crypto
- Identity
- Authentication
- OAuth
- OpenID Connect
- Proof of Humanity
- Blockchain
- Solana
- Agents
token_urls:
- https://sso.alien-api.com/oauth/token
---
