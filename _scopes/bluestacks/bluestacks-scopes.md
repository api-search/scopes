---
api_specs:
- filename: bluestacks-payments-asyncapi.yml
  format: yaml
  label: now.gg Payments Server API
  slug: nowgg-payments-server-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluestacks/refs/heads/main/asyncapi/bluestacks-payments-asyncapi.yml
authorization_urls: []
description: ''
docs: https://docs.now.gg/user-account-service/api-reference
flows:
- authorizationCode
- refreshToken
kind: oauth-scopes
layout: scope
method: searched
name: Bluestacks Scopes
name_suffix: OAuth Scopes
note: 'now.gg publishes no scopes or permissions reference page. The scope vocabulary below is what the API reference itself documents: the `scope` claim inside a decoded now.gg `token` is described as "Scope of authorization: email/profile/authorization". Those three values are the entire published surface. No per-scope description, no scope-request parameter, and no mapping from scope to endpoint is documented anywhere, so the descriptions below are the docs'' own wording and nothing more.'
overview: 'Bluestacks publishes 3 OAuth 2.0 scopes via the authorizationCode and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Bluestacks API on a user''s behalf.


  Tokens are issued from https://now.gg/accounts/oauth2/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bluestacks
provider_slug: bluestacks
schemes:
- flows:
  - flow: authorizationCode
    tokenUrl: https://now.gg/accounts/oauth2/v1/token
  - flow: refreshToken
    tokenUrl: https://now.gg/accounts/oauth2/v1/token
  name: nowggOAuth2
  source: https://docs.now.gg/user-account-service/api-reference
scope_count: 3
scope_names:
- email
- profile
- authorization
scopes:
- description: Scope of authorization covering the player's email address.
  flows:
  - authorizationCode
  scope: email
- description: Scope of authorization covering the player's profile information.
  flows:
  - authorizationCode
  scope: profile
- description: Scope of authorization covering authorization itself.
  flows:
  - authorizationCode
  scope: authorization
slug: bluestacks-scopes
source_filename: bluestacks-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: searched\nsource: https://docs.now.gg/user-account-service/api-reference\ndocs: https://docs.now.gg/user-account-service/api-reference\nnote: >-\n  now.gg publishes no scopes or permissions reference page. The scope vocabulary below\n  is what the API reference itself documents: the `scope` claim inside a decoded\n  now.gg `token` is described as \"Scope of authorization: email/profile/authorization\".\n  Those three values are the entire published surface. No per-scope description, no\n  scope-request parameter, and no mapping from scope to endpoint is documented\n  anywhere, so the descriptions below are the docs' own wording and nothing more.\nschemes:\n- name: nowggOAuth2\n  source: https://docs.now.gg/user-account-service/api-reference\n  flows:\n  - flow: authorizationCode\n    tokenUrl: https://now.gg/accounts/oauth2/v1/token\n  - flow: refreshToken\n    tokenUrl: https://now.gg/accounts/oauth2/v1/token\nscopes:\n- scope: email\n  description:\
  \ Scope of authorization covering the player's email address.\n  evidence: '`scope` claim sample value in the decoded-token reference'\n  flows:\n  - authorizationCode\n- scope: profile\n  description: Scope of authorization covering the player's profile information.\n  evidence: enumerated in the `scope` claim description (email/profile/authorization)\n  flows:\n  - authorizationCode\n- scope: authorization\n  description: Scope of authorization covering authorization itself.\n  evidence: enumerated in the `scope` claim description (email/profile/authorization)\n  flows:\n  - authorizationCode\ngaps:\n- No scopes/permissions reference page exists; the vocabulary is only visible as a\n  sample claim value inside the token reference.\n- No documented way for a client to REQUEST a scope — no scope parameter appears in\n  the token or verify-token request bodies.\n- No mapping from scope to the endpoints it authorizes (userinfo vs sessioninfo).\n- The Payments API is key-authorized, not OAuth-scoped,\
  \ so none of these scopes apply\n  to it.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bluestacks/refs/heads/main/scopes/bluestacks-scopes.yml
summary_line: 3 scopes · authorizationCode/refreshToken
tags:
- Company
- Gaming
- Cloud Gaming
- Android
- Mobile
- Payments
- In-App Purchases
- Subscription
- Developer Platform
- App Distribution
- Advertising
- Authentication
token_urls:
- https://now.gg/accounts/oauth2/v1/token
---
