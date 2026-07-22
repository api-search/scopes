---
authorization_urls:
- https://start.gg/oauth/authorize
description: ''
docs: https://developer.start.gg/docs/oauth/scopes
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Smashgg Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Smashgg publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Smashgg API on a user''s behalf.


  Tokens are issued from https://api.start.gg/oauth/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Smashgg
provider_slug: smashgg
schemes:
- flows:
  - authorizationUrl: https://start.gg/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.start.gg/oauth/access_token
  name: OAuth2
  source: https://developer.start.gg/docs/oauth/oauth-overview
scope_count: 4
scope_names:
- user.identity
- user.email
- tournament.manager
- tournament.reporter
scopes:
- description: Allows use of the currentUser query and all public fields for the user. Any private fields require additional scopes.
  flows:
  - authorizationCode
  scope: user.identity
- description: Allows use of the email field in the currentUser query. The user.identity scope is also required for this to work.
  flows:
  - authorizationCode
  scope: user.email
- description: Allows access to tournament seeding and bracket setup for tournaments the current user has access to.
  flows:
  - authorizationCode
  scope: tournament.manager
- description: Allows access to set reporting for tournaments the current user has access to.
  flows:
  - authorizationCode
  scope: tournament.reporter
slug: smashgg-scopes
source_filename: smashgg-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.start.gg/docs/oauth/scopes\ndocs: https://developer.start.gg/docs/oauth/scopes\nschemes:\n  - name: OAuth2\n    source: https://developer.start.gg/docs/oauth/oauth-overview\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://start.gg/oauth/authorize\n        tokenUrl: https://api.start.gg/oauth/access_token\nscopes:\n  - scope: user.identity\n    description: >-\n      Allows use of the currentUser query and all public fields for the user.\n      Any private fields require additional scopes.\n    flows: [authorizationCode]\n  - scope: user.email\n    description: >-\n      Allows use of the email field in the currentUser query. The\n      user.identity scope is also required for this to work.\n    flows: [authorizationCode]\n  - scope: tournament.manager\n    description: >-\n      Allows access to tournament seeding and bracket setup for tournaments\n      the current user has\
  \ access to.\n    flows: [authorizationCode]\n  - scope: tournament.reporter\n    description: >-\n      Allows access to set reporting for tournaments the current user has\n      access to.\n    flows: [authorizationCode]\nnotes: >-\n  start.gg notes that new scopes are still actively being developed, so this\n  list may grow. Scopes are requested by the third-party application and\n  approved by the resource owner at authentication time.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smashgg/refs/heads/main/scopes/smashgg-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Consumer
- Esports
- Gaming
- Tournaments
- GraphQL
- Events
- Developer API
token_urls:
- https://api.start.gg/oauth/access_token
---
