---
authorization_urls:
- https://api.sorare.com/oauth/authorize
description: ''
docs: https://github.com/sorare/api#oauth
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Sorare Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Sorare publishes 1 OAuth 2.0 scope via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Sorare API on a user''s behalf.


  Tokens are issued from https://api.sorare.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Sorare
provider_slug: sorare
schemes:
- flows:
  - authorizationUrl: https://api.sorare.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.sorare.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://api.sorare.com/oauth/token
  name: oauth2
  source: https://github.com/sorare/api
scope_count: 1
scope_names:
- default
scopes:
- description: Single default scope granted to OAuth applications. Provides read access to basic user information (nickname, avatar, wallet address), the user's cards, achievements and favorites, and the user's auctions, offers and notifications.
  flows:
  - authorizationCode
  - clientCredentials
  scope: default
slug: sorare-scopes
source_filename: sorare-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://github.com/sorare/api\ndocs: https://github.com/sorare/api#oauth\napi: GraphQL (https://api.sorare.com/graphql)\nschemes:\n  - name: oauth2\n    source: https://github.com/sorare/api\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://api.sorare.com/oauth/authorize\n        tokenUrl: https://api.sorare.com/oauth/token\n      - flow: clientCredentials\n        tokenUrl: https://api.sorare.com/oauth/token\nscopes:\n  - scope: default\n    description: >-\n      Single default scope granted to OAuth applications. Provides read access to basic\n      user information (nickname, avatar, wallet address), the user's cards, achievements\n      and favorites, and the user's auctions, offers and notifications.\n    flows: [authorizationCode, clientCredentials]\n    sources: [https://github.com/sorare/api]\nexcluded_from_default_scope:\n  - Access to the user's email address\n  - Future / upcoming lineups\n\
  \  - Claiming rewards\n  - Bidding, selling or other write/trading operations\nnotes:\n  - Sorare's OAuth model exposes a single coarse default scope rather than a granular\n    scope taxonomy; trading and reward actions are intentionally out of OAuth reach and\n    require JWT (user-owned) sessions plus Starkware signing.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sorare/refs/heads/main/scopes/sorare-scopes.yml
summary_line: 1 scope · authorizationCode/clientCredentials
tags:
- Company
- Crypto
- GraphQL
- Fantasy Sports
- NFT
- Blockchain
- Gaming
- Sports
- Web3
token_urls:
- https://api.sorare.com/oauth/token
---
