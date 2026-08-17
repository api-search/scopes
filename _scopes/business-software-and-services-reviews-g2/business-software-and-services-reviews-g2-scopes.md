---
api_specs:
- filename: business-software-and-services-reviews-g2-v2-openapi.yml
  format: yaml
  label: G2 API V2
  slug: g2-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/business-software-and-services-reviews-g2/refs/heads/main/openapi/business-software-and-services-reviews-g2-v2-openapi.yml
- filename: business-software-and-services-reviews-g2-v2-openapi.yml
  format: yaml
  label: G2 Buyer Intent Data API
  slug: g2-buyer-intent-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/business-software-and-services-reviews-g2/refs/heads/main/openapi/business-software-and-services-reviews-g2-v2-openapi.yml
- filename: business-software-and-services-reviews-g2-data-solutions-openapi.yml
  format: yaml
  label: G2 Data Solutions API
  slug: g2-data-solutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/business-software-and-services-reviews-g2/refs/heads/main/openapi/business-software-and-services-reviews-g2-data-solutions-openapi.yml
authorization_urls:
- https://www.g2.com/oauth/authorize
description: G2's OAuth 2.0 scope surface, reconciled across three sources that do not agree. The OpenAPI securityScheme declares only six scopes in its flows map but requires ten distinct scopes at the operation level; the MCP documentation publishes an eight-row table; the MCP protected-resource metadata advertises ten. The union is sixteen. `origin` on each entry records which sources name it, because a scope declared in only one place is a scope a client may not be able to request.
docs: https://documentation.g2.com/docs/g2-mcp-server
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Business Software And Services Reviews G2 Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Business Software and Services Reviews | G2 publishes 16 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Business Software and Services Reviews | G2 API on a user''s behalf.


  Tokens are issued from https://www.g2.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Business Software and Services Reviews | G2
provider_slug: business-software-and-services-reviews-g2
schemes:
- flows:
  - authorizationUrl: https://www.g2.com/oauth/authorize
    flow: authorizationCode
    pkce: true
    pkce_methods:
    - S256
    - plain
    tokenUrl: https://www.g2.com/oauth/token
  name: G2OAuth
  sources:
  - openapi/business-software-and-services-reviews-g2-v2-openapi.yml
  - openapi/business-software-and-services-reviews-g2-data-solutions-openapi.yml
  type: oauth2
- name: AccountAPIToken
  note: Non-OAuth path. Developer Portal access tokens carry per-endpoint permissions rather than scopes, and expire one year after creation. One operation (getGridReports) declares a scope-shaped requirement "reports.read" against this bearer scheme rather than against G2OAuth.
  scheme: bearer
  type: http
scope_count: 16
scope_names:
- openid
- profile
- products.read
- products.reviews.read
- vendors.read
- buyer_intent.read
- research_boards.read
- research_boards.write
- ds_reviews.read
- g2_activate.read
- performance_analytics.read
- data_subscriptions.read
- data_subscriptions.read_write
- data_subscriptions.write
- partner:partner-id.read
- snippets
scopes:
- description: OpenID Connect default scope. Required for OAuth authentication.
  flows: []
  scope: openid
- description: Profile information on current user. Required for OAuth authentication.
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
- description: Read Data Solutions reviews — the flat, firmographically enriched review projection. Required by getDataSolutionsReviews.
  flows: []
  scope: ds_reviews.read
- description: Read G2 Activate company unlock data. Required by the four G2 Activate operations; a 403 titled "Missing g2_activate.read scope" is declared.
  flows: []
  scope: g2_activate.read
- description: Read Performance Analytics data. Required by the five Performance Analytics operations; a 403 titled "Missing performance_analytics.read scope" is declared.
  flows: []
  scope: performance_analytics.read
- description: Read Data Subscription records.
  flows: []
  scope: data_subscriptions.read
- description: Modify Data Subscription records.
  flows: []
  scope: data_subscriptions.read_write
- description: Write Data Subscription records.
  flows: []
  scope: data_subscriptions.write
- description: Access records created in Partner realm.
  flows: []
  scope: partner:partner-id.read
- description: Access product snippets. Required by getProductSnippets.
  flows: []
  scope: snippets
slug: business-software-and-services-reviews-g2-scopes
source_filename: business-software-and-services-reviews-g2-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: >-\n  openapi/business-software-and-services-reviews-g2-v2-openapi.yml and\n  openapi/business-software-and-services-reviews-g2-data-solutions-openapi.yml\n  (declared flows + operation-level security requirements), enriched from\n  https://documentation.g2.com/docs/g2-mcp-server (published scope table) and\n  https://mcp.g2.com/.well-known/oauth-protected-resource/mcp (RFC 9728\n  scopes_supported).\ndocs: https://documentation.g2.com/docs/g2-mcp-server\ndescription: >-\n  G2's OAuth 2.0 scope surface, reconciled across three sources that do not\n  agree. The OpenAPI securityScheme declares only six scopes in its flows map but\n  requires ten distinct scopes at the operation level; the MCP documentation\n  publishes an eight-row table; the MCP protected-resource metadata advertises\n  ten. The union is sixteen. `origin` on each entry records which sources name\n  it, because a scope declared in only one place is a scope a\
  \ client may not be\n  able to request.\nauthorization_server: https://www.g2.com/\ndiscovery: well-known/business-software-and-services-reviews-g2-openid-configuration.json\nregistration:\n  url: https://my.g2.com/developers\n  dynamic_client_registration: false\n  note: >-\n    OAuth apps must be pre-registered in the G2 Developer Portal. Permissions are\n    selected per endpoint at registration; a scope requested in the flow must have\n    a matching Read permission enabled on the app or the authorization server\n    returns \"requested scope is invalid, unknown, or malformed\".\nschemes:\n  - name: G2OAuth\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://www.g2.com/oauth/authorize\n        tokenUrl: https://www.g2.com/oauth/token\n        pkce: true\n        pkce_methods: [S256, plain]\n    sources:\n      - openapi/business-software-and-services-reviews-g2-v2-openapi.yml\n      - openapi/business-software-and-services-reviews-g2-data-solutions-openapi.yml\n\
  \  - name: AccountAPIToken\n    type: http\n    scheme: bearer\n    note: >-\n      Non-OAuth path. Developer Portal access tokens carry per-endpoint\n      permissions rather than scopes, and expire one year after creation. One\n      operation (getGridReports) declares a scope-shaped requirement\n      \"reports.read\" against this bearer scheme rather than against G2OAuth.\nscope_count: 16\nscopes:\n  - scope: openid\n    description: OpenID Connect default scope. Required for OAuth authentication.\n    origin: [openapi-flows, mcp-docs, protected-resource, oidc-discovery]\n  - scope: profile\n    description: Profile information on current user. Required for OAuth authentication.\n    origin: [openapi-flows, mcp-docs, protected-resource, oidc-discovery]\n  - scope: products.read\n    description: Read product catalog data.\n    origin: [mcp-docs, protected-resource]\n  - scope: products.reviews.read\n    description: Read product reviews.\n    origin: [mcp-docs, protected-resource]\n\
  \  - scope: vendors.read\n    description: Read vendor data.\n    origin: [mcp-docs, protected-resource]\n  - scope: buyer_intent.read\n    description: Read buyer intent signals.\n    origin: [mcp-docs, protected-resource]\n  - scope: research_boards.read\n    description: Read research boards.\n    origin: [mcp-docs, protected-resource]\n  - scope: research_boards.write\n    description: Create, update, and delete research boards.\n    origin: [mcp-docs, protected-resource]\n  - scope: ds_reviews.read\n    description: >-\n      Read Data Solutions reviews — the flat, firmographically enriched review\n      projection. Required by getDataSolutionsReviews.\n    origin: [protected-resource, openapi-operations]\n  - scope: g2_activate.read\n    description: >-\n      Read G2 Activate company unlock data. Required by the four G2 Activate\n      operations; a 403 titled \"Missing g2_activate.read scope\" is declared.\n    origin: [protected-resource, openapi-operations]\n  - scope: performance_analytics.read\n\
  \    description: >-\n      Read Performance Analytics data. Required by the five Performance Analytics\n      operations; a 403 titled \"Missing performance_analytics.read scope\" is declared.\n    origin: [openapi-flows, openapi-operations]\n    note: Declared in the spec's flows map and required by operations, but absent from both MCP sources.\n  - scope: data_subscriptions.read\n    description: Read Data Subscription records.\n    origin: [openapi-flows, openapi-operations]\n  - scope: data_subscriptions.read_write\n    description: Modify Data Subscription records.\n    origin: [openapi-flows, openapi-operations]\n  - scope: data_subscriptions.write\n    description: Write Data Subscription records.\n    origin: [openapi-operations]\n    note: >-\n      Required by createPartnerDataSubscription but NOT declared in the\n      securityScheme flows map — a client reading only the flows map would never\n      know to request it.\n  - scope: 'partner:partner-id.read'\n    description:\
  \ Access records created in Partner realm.\n    origin: [openapi-flows, openapi-operations]\n    note: >-\n      Templated scope — \"partner-id\" is a placeholder for the partner's own\n      identifier, not a literal value.\n  - scope: snippets\n    description: Access product snippets. Required by getProductSnippets.\n    origin: [openapi-operations]\n    note: >-\n      Bare noun with no read/write suffix, unlike every other G2 scope, and\n      declared nowhere but on the operation. Likely legacy.\noidc_scopes_supported:\n  scopes:\n    - openid\n    - openid_admin\n    - profile\n    - profile_admin\n  note: >-\n    The OIDC discovery document at www.g2.com advertises only these four. The\n    API and MCP scopes above are not listed there, so scopes_supported in\n    discovery is not a usable inventory of G2's API authorization surface.\ninconsistencies:\n  - >-\n    The OpenAPI flows map declares 6 scopes; operations require 10; the union\n    across all published sources is 16.\
  \ No single G2 document lists them all.\n  - >-\n    data_subscriptions.write and snippets are required by operations but appear\n    in no flows map and no documentation.\n  - >-\n    performance_analytics.read and the data_subscriptions family appear in the\n    spec but not in the MCP protected-resource metadata, so they are presumably\n    unavailable to MCP clients.\n  - >-\n    getGridReports attaches \"reports.read\" to the AccountAPIToken bearer scheme,\n    which has no scope model at all.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/business-software-and-services-reviews-g2/refs/heads/main/scopes/business-software-and-services-reviews-g2-scopes.yml
summary_line: 16 scopes · authorizationCode
tags:
- B2B
- SaaS
- Software Reviews
- Buyer Intent
- Competitive Intelligence
- Market Intelligence
- Marketplace
- MCP
token_urls:
- https://www.g2.com/oauth/token
---
