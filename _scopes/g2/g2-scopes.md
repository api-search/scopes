---
api_specs:
- filename: g2-api-v2-openapi.yaml
  format: yaml
  label: G2 API
  slug: g2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/g2/refs/heads/main/openapi/g2-api-v2-openapi.yaml
- filename: g2-data-solutions-openapi.yaml
  format: yaml
  label: G2 Data Solutions API
  slug: g2-data-solutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/g2/refs/heads/main/openapi/g2-data-solutions-openapi.yaml
authorization_urls: []
description: ''
docs: https://documentation.g2.com/docs/g2-mcp-server#connect-directly-to-the-g2-mcp-server
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: G2 Scopes
name_suffix: OAuth Scopes
note: 'G2 publishes NO single consolidated scopes reference. Two partial lists exist and they do not agree: the OpenAPI securityScheme declares six scopes, while the MCP documentation''s scope table names eight, four of which (products.read, products.reviews.read, vendors.read, buyer_intent.read, research_boards.read/write) never appear in the securityScheme. A third set is only discoverable from per-operation 403 error titles in the spec (performance_analytics.read, g2_activate.read, g2_activate.write) and from operation descriptions ("Requires `products.read` scope"). This file is the union, with the source of each scope recorded — that divergence is itself the finding.'
overview: 'G2 publishes 18 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the G2 API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: G2
provider_slug: g2
schemes:
- authorizationUrl: https://www.g2.com/oauth/authorize
  dynamic_client_registration: false
  flow: authorizationCode
  name: G2OAuth
  pkce: S256
  registration: https://my.g2.com/developers
  tokenUrl: https://www.g2.com/oauth/token
  type: oauth2
- name: AccountAPIToken
  note: Account tokens are not scoped by OAuth scope strings. They carry a per-endpoint Access permission grid selected at token creation in the Developer Portal.
  scheme: bearer
  type: http
scope_count: 18
scope_names:
- openid
- profile
- products.read
- products.reviews.read
- vendors.read
- buyer_intent.read
- research_boards.read
- research_boards.write
- data_subscriptions.read
- data_subscriptions.read_write
- data_subscriptions.write
- performance_analytics.read
- partner:partner-id.read
- g2_activate.read
- g2_activate.write
- snippets
- openid_admin
- profile_admin
scopes:
- description: OpenID Connect default scope. Required for OAuth authentication.
  flows: []
  scope: openid
- description: Profile information on the current user. Required for OAuth authentication.
  flows: []
  scope: profile
- description: Read product catalog data.
  flows: []
  scope: products.read
- description: Read product reviews.
  flows: []
  scope: products.reviews.read
- description: Read vendor data.
  flows: []
  scope: vendors.read
- description: Read buyer intent signals.
  flows: []
  scope: buyer_intent.read
- description: Read research boards.
  flows: []
  scope: research_boards.read
- description: Create, update, and delete research boards.
  flows: []
  scope: research_boards.write
- description: Read Data Subscription records.
  flows: []
  scope: data_subscriptions.read
- description: Modify Data Subscription records.
  flows: []
  scope: data_subscriptions.read_write
- description: Write Data Subscription records.
  flows: []
  scope: data_subscriptions.write
- description: Read Performance Analytics data.
  flows: []
  scope: performance_analytics.read
- description: Access records created in the Partner realm.
  flows: []
  scope: partner:partner-id.read
- description: Read G2 Activate locked/unlocked company records.
  flows: []
  scope: g2_activate.read
- description: Spend credits to unlock G2 Activate companies.
  flows: []
  scope: g2_activate.write
- description: Access review snippets.
  flows: []
  scope: snippets
- description: Administrative OpenID scope.
  flows: []
  scope: openid_admin
- description: Administrative profile scope.
  flows: []
  scope: profile_admin
slug: g2-scopes
source_filename: g2-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: >-\n  openapi/g2-api-v2-openapi.yaml (components.securitySchemes.G2OAuth.flows.authorizationCode.scopes\n  and per-operation security requirements), enriched from\n  https://documentation.g2.com/docs/g2-mcp-server and\n  https://documentation.g2.com/docs/developer-portal\ndocs: https://documentation.g2.com/docs/g2-mcp-server#connect-directly-to-the-g2-mcp-server\nprovider: G2\nproviderId: g2\nnote: >-\n  G2 publishes NO single consolidated scopes reference. Two partial lists exist and they do\n  not agree: the OpenAPI securityScheme declares six scopes, while the MCP documentation's\n  scope table names eight, four of which (products.read, products.reviews.read, vendors.read,\n  buyer_intent.read, research_boards.read/write) never appear in the securityScheme. A third\n  set is only discoverable from per-operation 403 error titles in the spec\n  (performance_analytics.read, g2_activate.read, g2_activate.write) and from operation\n\
  \  descriptions (\"Requires `products.read` scope\"). This file is the union, with the source of\n  each scope recorded — that divergence is itself the finding.\nschemes:\n  - name: G2OAuth\n    type: oauth2\n    flow: authorizationCode\n    pkce: S256\n    authorizationUrl: https://www.g2.com/oauth/authorize\n    tokenUrl: https://www.g2.com/oauth/token\n    dynamic_client_registration: false\n    registration: https://my.g2.com/developers\n  - name: AccountAPIToken\n    type: http\n    scheme: bearer\n    note: >-\n      Account tokens are not scoped by OAuth scope strings. They carry a per-endpoint\n      Access permission grid selected at token creation in the Developer Portal.\nscopes:\n  - scope: openid\n    description: OpenID Connect default scope. Required for OAuth authentication.\n    required: true\n    sources: [openapi, mcp-docs, openid-configuration]\n  - scope: profile\n    description: Profile information on the current user. Required for OAuth authentication.\n    required:\
  \ true\n    sources: [openapi, mcp-docs, openid-configuration]\n  - scope: products.read\n    description: Read product catalog data.\n    sources: [mcp-docs, openapi-operation-descriptions]\n    note: Named in operation descriptions (\"Requires `products.read` scope\") but absent from the securityScheme scope map.\n  - scope: products.reviews.read\n    description: Read product reviews.\n    sources: [mcp-docs]\n  - scope: vendors.read\n    description: Read vendor data.\n    sources: [mcp-docs]\n  - scope: buyer_intent.read\n    description: Read buyer intent signals.\n    sources: [mcp-docs]\n  - scope: research_boards.read\n    description: Read research boards.\n    sources: [mcp-docs]\n  - scope: research_boards.write\n    description: Create, update, and delete research boards.\n    sources: [mcp-docs]\n    write: true\n  - scope: data_subscriptions.read\n    description: Read Data Subscription records.\n    sources: [openapi]\n  - scope: data_subscriptions.read_write\n    description:\
  \ Modify Data Subscription records.\n    sources: [openapi]\n    write: true\n  - scope: data_subscriptions.write\n    description: Write Data Subscription records.\n    sources: [openapi]\n    write: true\n    note: Appears in per-operation security requirements but not in the securityScheme scope map.\n  - scope: performance_analytics.read\n    description: Read Performance Analytics data.\n    sources: [openapi]\n    note: Enforced with the 403 title \"Missing performance_analytics.read scope\" on 5 operations.\n  - scope: 'partner:partner-id.read'\n    description: Access records created in the Partner realm.\n    sources: [openapi]\n    note: Templated — substitute the caller's partner id.\n  - scope: g2_activate.read\n    description: Read G2 Activate locked/unlocked company records.\n    sources: [openapi-operation-security, openapi-error-titles]\n    note: Enforced with the 403 title \"Missing g2_activate.read scope\".\n  - scope: g2_activate.write\n    description: Spend credits\
  \ to unlock G2 Activate companies.\n    sources: [openapi-operation-security, openapi-error-titles]\n    write: true\n    billable: true\n    note: >-\n      The only scope in the contract that authorizes spending money. Enforced with the 403\n      title \"Missing g2_activate.write scope\".\n  - scope: snippets\n    description: Access review snippets.\n    sources: [openapi]\n  - scope: openid_admin\n    description: Administrative OpenID scope.\n    sources: [openid-configuration]\n  - scope: profile_admin\n    description: Administrative profile scope.\n    sources: [openid-configuration]\nscope_count: 18\noperational_notes:\n  - >-\n    Requested scopes must match the Read/Write Permissions enabled on the OAuth app in the\n    Developer Portal, or the token request fails with \"requested scope is invalid, unknown, or\n    malformed\". G2's documented remedy is to add scopes back one at a time.\n  - Request only the scopes an application requires; permissions are selected per endpoint\
  \ at app registration.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/g2/refs/heads/main/scopes/g2-scopes.yml
summary_line: 18 scopes
tags:
- B2B
- Software Discovery
- Software Reviews
- Buyer Intent
- Market Intelligence
- Product Catalog
- Competitive Intelligence
- Reviews
- Data Solutions
- MCP
token_urls: []
---
