---
authorization_urls:
- https://id.articulate.com/oauth2/v1/authorize
description: ''
docs: https://id.articulate.com/.well-known/openid-configuration
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Articulate Scopes
name_suffix: OAuth Scopes
note: OpenID Connect scopes advertised by the Articulate identity provider (id.articulate.com) for user authentication / SSO. These are the standard OIDC claim scopes, not permissions on a public Articulate REST API (Articulate does not publish one). The oauth-authorization-server document additionally advertises the default Okta management scopes (okta.*), which govern the underlying Okta org rather than an Articulate product API, and are omitted here.
overview: 'Articulate publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Articulate API on a user''s behalf.


  Tokens are issued from https://id.articulate.com/oauth2/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Articulate
provider_slug: articulate
schemes:
- flows:
  - authorizationUrl: https://id.articulate.com/oauth2/v1/authorize
    flow: authorizationCode
    tokenUrl: https://id.articulate.com/oauth2/v1/token
  name: OAuth2
  source: well-known/articulate-openid-configuration.json
scope_count: 7
scope_names:
- openid
- email
- profile
- address
- phone
- groups
- offline_access
scopes:
- description: Authenticate the user and issue an ID token (OpenID Connect).
  flows: []
  scope: openid
- description: Access the user's email address and verification status.
  flows: []
  scope: email
- description: Access the user's basic profile claims (name, locale, etc.).
  flows: []
  scope: profile
- description: Access the user's address claim.
  flows: []
  scope: address
- description: Access the user's phone number claim.
  flows: []
  scope: phone
- description: Access the user's group memberships.
  flows: []
  scope: groups
- description: Issue a refresh token for long-lived access.
  flows: []
  scope: offline_access
slug: articulate-scopes
source_filename: articulate-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://id.articulate.com/.well-known/openid-configuration\ndocs: https://id.articulate.com/.well-known/openid-configuration\nnote: >-\n  OpenID Connect scopes advertised by the Articulate identity provider\n  (id.articulate.com) for user authentication / SSO. These are the standard\n  OIDC claim scopes, not permissions on a public Articulate REST API (Articulate\n  does not publish one). The oauth-authorization-server document additionally\n  advertises the default Okta management scopes (okta.*), which govern the\n  underlying Okta org rather than an Articulate product API, and are omitted here.\nschemes:\n- name: OAuth2\n  source: well-known/articulate-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://id.articulate.com/oauth2/v1/authorize\n    tokenUrl: https://id.articulate.com/oauth2/v1/token\nscopes:\n- scope: openid\n  description: Authenticate the user and issue an ID token\
  \ (OpenID Connect).\n- scope: email\n  description: Access the user's email address and verification status.\n- scope: profile\n  description: Access the user's basic profile claims (name, locale, etc.).\n- scope: address\n  description: Access the user's address claim.\n- scope: phone\n  description: Access the user's phone number claim.\n- scope: groups\n  description: Access the user's group memberships.\n- scope: offline_access\n  description: Issue a refresh token for long-lived access.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/articulate/refs/heads/main/scopes/articulate-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Company
- Edtech
- E-Learning
- Learning Management
- Training
- Course Authoring
- SSO
- OpenID Connect
token_urls:
- https://id.articulate.com/oauth2/v1/token
---
