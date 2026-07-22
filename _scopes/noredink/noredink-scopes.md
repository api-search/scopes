---
authorization_urls:
- https://www.noredink.com/oauth/authorize
description: ''
docs: https://www.noredink.com/.well-known/openid-configuration
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Noredink Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'NoRedInk publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the NoRedInk API on a user''s behalf.


  Tokens are issued from https://www.noredink.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: NoRedInk
provider_slug: noredink
schemes:
- flows:
  - authorizationUrl: https://www.noredink.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://www.noredink.com/oauth/token
  name: OAuth2
  source: well-known/noredink-openid-configuration.json
scope_count: 1
scope_names:
- openid
scopes:
- description: OpenID Connect authentication scope. Requests an ID token asserting the user's identity (iss, sub, aud, exp, iat, roles claims) via the userinfo endpoint.
  flows:
  - authorizationCode
  scope: openid
slug: noredink-scopes
source_filename: noredink-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: well-known/noredink-openid-configuration.json\ndocs: https://www.noredink.com/.well-known/openid-configuration\nschemes:\n- name: OAuth2\n  source: well-known/noredink-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.noredink.com/oauth/authorize\n    tokenUrl: https://www.noredink.com/oauth/token\nscopes:\n- scope: openid\n  description: >-\n    OpenID Connect authentication scope. Requests an ID token asserting the\n    user's identity (iss, sub, aud, exp, iat, roles claims) via the userinfo\n    endpoint.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/noredink-openid-configuration.json\nnotes: >-\n  NoRedInk's discovery document advertises a single OAuth 2.0 scope (`openid`).\n  Any additional partner/rostering scopes are not published in the public\n  discovery metadata.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/noredink/refs/heads/main/scopes/noredink-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Education
- EdTech
- English Language Arts
- Grammar
- Writing
- Literacy
- K-12
- OAuth
- OpenID Connect
- Single Sign-On
- Rostering
- Identity
token_urls:
- https://www.noredink.com/oauth/token
---
