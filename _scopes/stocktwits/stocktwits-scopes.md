---
api_specs:
- filename: stocktwits-openapi-original.json
  format: json
  label: StockTwits API v2
  slug: stocktwits-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stocktwits/refs/heads/main/openapi/stocktwits-openapi-original.json
authorization_urls:
- https://api.stocktwits.com/api/2/oauth/authorize
description: ''
docs: https://api.stocktwits.com/developers/docs
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Stocktwits Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'StockTwits publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the StockTwits API on a user''s behalf.


  Tokens are issued from https://api.stocktwits.com/api/2/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: StockTwits
provider_slug: stocktwits
schemes:
- description: StockTwits uses OAuth 2.0 for authentication. Some endpoints are available without authentication using just an access_token query parameter.
  flows:
  - authorizationUrl: https://api.stocktwits.com/api/2/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.stocktwits.com/api/2/oauth/token
  name: oauth2
  source: openapi/stocktwits-openapi-original.json
scope_count: 6
scope_names:
- follow_stocks
- follow_users
- publish_messages
- publish_watch_lists
- read
- watchlists
scopes:
- description: Follow and unfollow stocks
  flows:
  - authorizationCode
  scope: follow_stocks
- description: Follow and unfollow users
  flows:
  - authorizationCode
  scope: follow_users
- description: Create and interact with messages
  flows:
  - authorizationCode
  scope: publish_messages
- description: Create and manage watchlists
  flows:
  - authorizationCode
  scope: publish_watch_lists
- description: Read access to public data
  flows:
  - authorizationCode
  scope: read
- description: ''
  flows: []
  scope: watchlists
slug: stocktwits-scopes
source_filename: stocktwits-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/stocktwits-openapi-original.json\ndocs: https://api.stocktwits.com/developers/docs\nnotes: 'StockTwits OAuth 2.0 authorization-code scopes. `read` covers public data;\n  publish_messages / publish_watch_lists / follow_users / follow_stocks gate the write\n  operations. `watchlists` appears as an operation-level security requirement in the\n  spec. Some endpoints work unauthenticated with an app-level access_token query param.'\nschemes:\n- name: oauth2\n  source: openapi/stocktwits-openapi-original.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.stocktwits.com/api/2/oauth/authorize\n    tokenUrl: https://api.stocktwits.com/api/2/oauth/token\n  description: StockTwits uses OAuth 2.0 for authentication. Some endpoints are available without\n    authentication using just an access_token query parameter.\nscopes:\n- scope: follow_stocks\n  description: Follow and unfollow stocks\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - openapi/stocktwits-openapi-original.json\n- scope: follow_users\n  description: Follow and unfollow users\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/stocktwits-openapi-original.json\n- scope: publish_messages\n  description: Create and interact with messages\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/stocktwits-openapi-original.json\n- scope: publish_watch_lists\n  description: Create and manage watchlists\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/stocktwits-openapi-original.json\n- scope: read\n  description: Read access to public data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/stocktwits-openapi-original.json\n- scope: watchlists\n  sources:\n  - openapi/stocktwits-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stocktwits/refs/heads/main/scopes/stocktwits-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Company
- Fintech
- Social
- Stocks
- Trading
- Investing
- Market Data
- Social Finance
- Watchlists
- Messaging
token_urls:
- https://api.stocktwits.com/api/2/oauth/token
---
