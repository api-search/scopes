---
api_specs:
- filename: aol-oauth2-api-openapi.yml
  format: yaml
  label: AOL OAuth2 API
  slug: aol-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aol/refs/heads/main/openapi/aol-oauth2-api-openapi.yml
- filename: aol-openid-connect-api-openapi.yml
  format: yaml
  label: AOL OpenID Connect API
  slug: aol-openid-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aol/refs/heads/main/openapi/aol-openid-connect-api-openapi.yml
authorization_urls:
- https://api.login.aol.com/oauth2/request_auth
description: ''
docs: https://developer.yahoo.com/oauth2/guide/openid_connect/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Aol Scopes
name_suffix: OAuth Scopes
note: Upgraded from derived (three scopes read out of this repo's OpenAPI) to probed against AOL's own OpenID Connect discovery document, which advertises a fourth scope, `openid2`, that the spec omits. AOL publishes no separate scope / permissions reference page; `scopes_supported` in the discovery document is the authoritative published list.
overview: 'AOL publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the AOL API on a user''s behalf.


  Tokens are issued from https://api.login.aol.com/oauth2/get_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AOL
provider_slug: aol
schemes:
- flows:
  - authorizationUrl: https://api.login.aol.com/oauth2/request_auth
    flow: authorizationCode
    tokenUrl: https://api.login.aol.com/oauth2/get_token
  name: oauth2
  source: https://api.login.aol.com/.well-known/openid-configuration
scope_count: 4
scope_names:
- openid
- openid2
- profile
- email
scopes:
- description: OpenID Connect authentication. Requesting it makes the token response carry a signed `id_token` and enables the userinfo endpoint.
  flows:
  - authorizationCode
  scope: openid
- description: Legacy OpenID 2.0 compatibility scope advertised by the AOL discovery document for applications migrated from the pre-OIDC AOL/Oath identity stack. Not present in this repo's OpenAPI; discovered by probe.
  flows:
  - authorizationCode
  scope: openid2
- description: Basic profile claims — name, given_name, family_name, locale, birthdate.
  flows:
  - authorizationCode
  scope: profile
- description: Email address and the `email_verified` claim.
  flows:
  - authorizationCode
  scope: email
slug: aol-scopes
source_filename: aol-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: https://api.login.aol.com/.well-known/openid-configuration\ndocs: https://developer.yahoo.com/oauth2/guide/openid_connect/\nnote: >-\n  Upgraded from derived (three scopes read out of this repo's OpenAPI) to probed\n  against AOL's own OpenID Connect discovery document, which advertises a fourth\n  scope, `openid2`, that the spec omits. AOL publishes no separate scope /\n  permissions reference page; `scopes_supported` in the discovery document is the\n  authoritative published list.\nschemes:\n- name: oauth2\n  source: https://api.login.aol.com/.well-known/openid-configuration\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.login.aol.com/oauth2/request_auth\n    tokenUrl: https://api.login.aol.com/oauth2/get_token\nscopes:\n- scope: openid\n  description: >-\n    OpenID Connect authentication. Requesting it makes the token response carry a\n    signed `id_token` and enables the userinfo endpoint.\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - https://api.login.aol.com/.well-known/openid-configuration\n  - openapi/aol-oauth2-api-openapi.yml\n- scope: openid2\n  description: >-\n    Legacy OpenID 2.0 compatibility scope advertised by the AOL discovery\n    document for applications migrated from the pre-OIDC AOL/Oath identity stack.\n    Not present in this repo's OpenAPI; discovered by probe.\n  flows:\n  - authorizationCode\n  sources:\n  - https://api.login.aol.com/.well-known/openid-configuration\n- scope: profile\n  description: >-\n    Basic profile claims — name, given_name, family_name, locale, birthdate.\n  flows:\n  - authorizationCode\n  sources:\n  - https://api.login.aol.com/.well-known/openid-configuration\n  - openapi/aol-oauth2-api-openapi.yml\n- scope: email\n  description: Email address and the `email_verified` claim.\n  flows:\n  - authorizationCode\n  sources:\n  - https://api.login.aol.com/.well-known/openid-configuration\n  - openapi/aol-oauth2-api-openapi.yml\n\
  evidence:\n- url: https://api.login.aol.com/.well-known/openid-configuration\n  status: 200\n  fetched: '2026-09-02'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aol/refs/heads/main/scopes/aol-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Digital Media
- News
- Entertainment
- Advertising
- Identity
- OpenID Connect
- Authentication
- Email
- Consumer Internet
- Fortune 1000
token_urls:
- https://api.login.aol.com/oauth2/get_token
---
