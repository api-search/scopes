---
api_specs:
- filename: criteo-retail-media-api-openapi.yml
  format: yaml
  label: Criteo Retail Media API
  slug: criteo-retail-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-retail-media-api-openapi.yml
- filename: criteo-marketing-solutions-api-openapi.yml
  format: yaml
  label: Criteo Marketing Solutions API
  slug: criteo-marketing-solutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-marketing-solutions-api-openapi.yml
- filename: criteo-commerce-grid-api-openapi.yml
  format: yaml
  label: Criteo Commerce Grid API
  slug: criteo-commerce-grid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-commerce-grid-api-openapi.yml
authorization_urls:
- https://api.criteo.com/oauth2
description: ''
docs: https://developers.criteo.com/criteo-apis/docs/create-your-app
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Criteo Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Criteo publishes 22 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Criteo API on a user''s behalf.


  Tokens are issued from https://api.criteo.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Criteo
provider_slug: criteo
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.criteo.com/oauth2/token
  - authorizationUrl: https://api.criteo.com/oauth2
    flow: authorizationCode
    tokenUrl: https://api.criteo.com/oauth2/token
  name: oauth
  note: The spec's declared flow `scopes` maps are empty ({}) in all three services; the scope strings appear only on per-operation `security` requirements. A generic OAuth client reading only components.securitySchemes will therefore see zero scopes — this is a real spec-quality gap worth reporting to Criteo.
  source: openapi/criteo-retail-media-api-openapi.yml
scope_count: 22
scope_names:
- RetailMedia_Accounts_Read
- RetailMedia_Accounts_Manage
- RetailMedia_Campaign_Read
- RetailMedia_Campaign_Manage
- RetailMedia_Audience_Read
- RetailMedia_Audience_Manage
- RetailMedia_Balance_Read
- RetailMedia_Balance_Manage
- RetailMedia_Analytics_Read
- RetailMedia_Billing_Read
- RetailMedia_Catalog_Manage
- MarketingSolutions_Campaign_Read
- MarketingSolutions_Campaign_Manage
- MarketingSolutions_Audience_Read
- MarketingSolutions_Audience_Manage
- MarketingSolutions_Creative_Read
- MarketingSolutions_Creative_Manage
- MarketingSolutions_Analytics_Read
- MarketingSolutions_Reco_Read
- MarketingSolutions_Reco_Manage
- CommerceGrid_Segment_Read
- CommerceGrid_Segment_Manage
scopes:
- description: Read accounts, their properties and parent/child relationships.
  flows: []
  scope: RetailMedia_Accounts_Read
- description: Create and modify accounts, add/remove brands, create child brand accounts under a Private Market parent.
  flows: []
  scope: RetailMedia_Accounts_Manage
- description: Read campaigns, line items, keywords, promoted products and targeting.
  flows: []
  scope: RetailMedia_Campaign_Read
- description: Create and modify campaigns, auction and preferred line items, keywords, promoted products and targeting.
  flows: []
  scope: RetailMedia_Campaign_Manage
- description: Read audiences and audience segments available to campaigns.
  flows: []
  scope: RetailMedia_Audience_Read
- description: Create and modify audiences, audience segments and contact lists.
  flows: []
  scope: RetailMedia_Audience_Manage
- description: Read balance entities and the spending limits they define.
  flows: []
  scope: RetailMedia_Balance_Read
- description: Create balances, add funds, change balance dates and attach campaigns to a balance.
  flows: []
  scope: RetailMedia_Balance_Manage
- description: Request and retrieve campaign, line-item, revenue, fill-rate, attributed-transaction and real-time performance reports.
  flows: []
  scope: RetailMedia_Analytics_Read
- description: Request and retrieve partner billing reports.
  flows: []
  scope: RetailMedia_Billing_Read
- description: Request a retailer catalog build and retrieve its status and streamed output.
  flows: []
  scope: RetailMedia_Catalog_Manage
- description: Read campaigns, ad sets, budgets and Marketplace Performance Outcomes entities.
  flows: []
  scope: MarketingSolutions_Campaign_Read
- description: Create and modify campaigns, ad sets, budgets, bids and MPO seller activation.
  flows: []
  scope: MarketingSolutions_Campaign_Manage
- description: Read audiences and audience segments and compute or estimate their sizes.
  flows: []
  scope: MarketingSolutions_Audience_Read
- description: Create and modify audiences and segments, and add/remove contact-list members.
  flows: []
  scope: MarketingSolutions_Audience_Manage
- description: Read creatives, ads, assets and coupons.
  flows: []
  scope: MarketingSolutions_Creative_Read
- description: Create and modify creatives, ads, assets and coupons.
  flows: []
  scope: MarketingSolutions_Creative_Manage
- description: Request and retrieve advertiser and campaign performance reports.
  flows: []
  scope: MarketingSolutions_Analytics_Read
- description: Read product recommendation configuration and product sets.
  flows: []
  scope: MarketingSolutions_Reco_Read
- description: Create and modify product recommendation configuration and product sets.
  flows: []
  scope: MarketingSolutions_Reco_Manage
- description: Read Commerce Grid audience segments.
  flows: []
  scope: CommerceGrid_Segment_Read
- description: Create and modify Commerce Grid audience segments.
  flows: []
  scope: CommerceGrid_Segment_Manage
slug: criteo-scopes
source_filename: criteo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/criteo-retail-media-api-openapi.yml, openapi/criteo-marketing-solutions-api-openapi.yml, openapi/criteo-commerce-grid-api-openapi.yml\ndocs: https://developers.criteo.com/criteo-apis/docs/create-your-app\nsupersedes: >-\n  The previous version of this file listed Criteo's developer-portal \"domains\" (Accounts,\n  Analytics, Audiences, ...) because the only spec in the repo was a hand-authored scaffold\n  whose oauth2 flows declared an empty scopes map. Criteo's REAL published OpenAPI, harvested\n  2026-08-13 from https://api.criteo.com/2026-07/{service}/open-api-specifications.json,\n  carries the actual scope STRINGS on every operation's security requirement. Those 22\n  strings are recorded below. The portal domains are retained as `authorization_model`\n  because that is genuinely how a developer grants them — the domain is what you toggle in\n  the app UI, the scope string is what arrives in the token.\n\nauthorization_model:\n\
  \  docs: https://developers.criteo.com/criteo-apis/docs/create-your-app\n  description: >-\n    Criteo does not accept a `scope` parameter in the token request. Permissions are bound to\n    the API application: when you create an app in the developer portal you pick a service\n    (Retail Media / Marketing Solutions / Commerce Grid) and set each functional DOMAIN to an\n    authorization level of No access, Read, or Manage. The resulting token silently carries\n    the corresponding `<Service>_<Domain>_<Level>` scopes. An agent cannot widen its own\n    grant at runtime; widening requires an app change and, for Authorization Code apps, a\n    fresh consent from the account owner at https://consent.criteo.com/request.\n  levels: [No access, Read, Manage]\n  level_note: >-\n    Manage implies Read. On the Retail Media Accounts domain, Manage additionally requires\n    prior activation by a Criteo contact.\n\nschemes:\n- name: oauth\n  source: openapi/criteo-retail-media-api-openapi.yml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.criteo.com/oauth2/token\n  - flow: authorizationCode\n    authorizationUrl: https://api.criteo.com/oauth2\n    tokenUrl: https://api.criteo.com/oauth2/token\n  note: >-\n    The spec's declared flow `scopes` maps are empty ({}) in all three services; the scope\n    strings appear only on per-operation `security` requirements. A generic OAuth client\n    reading only components.securitySchemes will therefore see zero scopes — this is a real\n    spec-quality gap worth reporting to Criteo.\n\nscopes:\n# ---- Retail Media (12) ----\n- scope: RetailMedia_Accounts_Read\n  domain: Accounts\n  service: Retail Media\n  level: Read\n  description: Read accounts, their properties and parent/child relationships.\n  sources: [openapi/criteo-retail-media-api-openapi.yml]\n- scope: RetailMedia_Accounts_Manage\n  domain: Accounts\n  service: Retail Media\n  level: Manage\n  description: Create and modify accounts, add/remove brands, create\
  \ child brand accounts under a Private Market parent.\n  note: Manage on this domain requires prior activation by a Criteo contact.\n  sources: [openapi/criteo-retail-media-api-openapi.yml]\n- scope: RetailMedia_Campaign_Read\n  domain: Campaign\n  service: Retail Media\n  level: Read\n  description: Read campaigns, line items, keywords, promoted products and targeting.\n  sources: [openapi/criteo-retail-media-api-openapi.yml]\n- scope: RetailMedia_Campaign_Manage\n  domain: Campaign\n  service: Retail Media\n  level: Manage\n  description: Create and modify campaigns, auction and preferred line items, keywords, promoted products and targeting.\n  sources: [openapi/criteo-retail-media-api-openapi.yml]\n- scope: RetailMedia_Audience_Read\n  domain: Audiences\n  service: Retail Media\n  level: Read\n  description: Read audiences and audience segments available to campaigns.\n  sources: [openapi/criteo-retail-media-api-openapi.yml]\n- scope: RetailMedia_Audience_Manage\n  domain: Audiences\n\
  \  service: Retail Media\n  level: Manage\n  description: Create and modify audiences, audience segments and contact lists.\n  sources: [openapi/criteo-retail-media-api-openapi.yml]\n- scope: RetailMedia_Balance_Read\n  domain: Balances\n  service: Retail Media\n  level: Read\n  description: Read balance entities and the spending limits they define.\n  sources: [openapi/criteo-retail-media-api-openapi.yml]\n- scope: RetailMedia_Balance_Manage\n  domain: Balances\n  service: Retail Media\n  level: Manage\n  description: Create balances, add funds, change balance dates and attach campaigns to a balance.\n  sources: [openapi/criteo-retail-media-api-openapi.yml]\n- scope: RetailMedia_Analytics_Read\n  domain: Analytics\n  service: Retail Media\n  level: Read\n  description: Request and retrieve campaign, line-item, revenue, fill-rate, attributed-transaction and real-time performance reports.\n  sources: [openapi/criteo-retail-media-api-openapi.yml]\n- scope: RetailMedia_Billing_Read\n  domain:\
  \ Billing\n  service: Retail Media\n  level: Read\n  description: Request and retrieve partner billing reports.\n  sources: [openapi/criteo-retail-media-api-openapi.yml]\n- scope: RetailMedia_Catalog_Manage\n  domain: Catalog\n  service: Retail Media\n  level: Manage\n  description: Request a retailer catalog build and retrieve its status and streamed output.\n  note: >-\n    Catalog exposes only a Manage scope in the spec — there is no RetailMedia_Catalog_Read.\n    Reading a catalog requires the same grant as requesting one, because retrieval is the\n    second half of an asynchronous request the caller initiated.\n  sources: [openapi/criteo-retail-media-api-openapi.yml]\n\n# ---- Marketing Solutions (9) ----\n- scope: MarketingSolutions_Campaign_Read\n  domain: Campaign\n  service: Marketing Solutions\n  level: Read\n  description: Read campaigns, ad sets, budgets and Marketplace Performance Outcomes entities.\n  sources: [openapi/criteo-marketing-solutions-api-openapi.yml]\n- scope:\
  \ MarketingSolutions_Campaign_Manage\n  domain: Campaign\n  service: Marketing Solutions\n  level: Manage\n  description: Create and modify campaigns, ad sets, budgets, bids and MPO seller activation.\n  sources: [openapi/criteo-marketing-solutions-api-openapi.yml]\n- scope: MarketingSolutions_Audience_Read\n  domain: Audiences\n  service: Marketing Solutions\n  level: Read\n  description: Read audiences and audience segments and compute or estimate their sizes.\n  sources: [openapi/criteo-marketing-solutions-api-openapi.yml]\n- scope: MarketingSolutions_Audience_Manage\n  domain: Audiences\n  service: Marketing Solutions\n  level: Manage\n  description: Create and modify audiences and segments, and add/remove contact-list members.\n  sources: [openapi/criteo-marketing-solutions-api-openapi.yml]\n- scope: MarketingSolutions_Creative_Read\n  domain: Creative\n  service: Marketing Solutions\n  level: Read\n  description: Read creatives, ads, assets and coupons.\n  sources: [openapi/criteo-marketing-solutions-api-openapi.yml]\n\
  - scope: MarketingSolutions_Creative_Manage\n  domain: Creative\n  service: Marketing Solutions\n  level: Manage\n  description: Create and modify creatives, ads, assets and coupons.\n  sources: [openapi/criteo-marketing-solutions-api-openapi.yml]\n- scope: MarketingSolutions_Analytics_Read\n  domain: Analytics\n  service: Marketing Solutions\n  level: Read\n  description: Request and retrieve advertiser and campaign performance reports.\n  sources: [openapi/criteo-marketing-solutions-api-openapi.yml]\n- scope: MarketingSolutions_Reco_Read\n  domain: Reco\n  service: Marketing Solutions\n  level: Read\n  description: Read product recommendation configuration and product sets.\n  sources: [openapi/criteo-marketing-solutions-api-openapi.yml]\n- scope: MarketingSolutions_Reco_Manage\n  domain: Reco\n  service: Marketing Solutions\n  level: Manage\n  description: Create and modify product recommendation configuration and product sets.\n  sources: [openapi/criteo-marketing-solutions-api-openapi.yml]\n\
  \n# ---- Commerce Grid (2) ----\n- scope: CommerceGrid_Segment_Read\n  domain: Segment\n  service: Commerce Grid\n  level: Read\n  description: Read Commerce Grid audience segments.\n  sources: [openapi/criteo-commerce-grid-api-openapi.yml]\n- scope: CommerceGrid_Segment_Manage\n  domain: Segment\n  service: Commerce Grid\n  level: Manage\n  description: Create and modify Commerce Grid audience segments.\n  sources: [openapi/criteo-commerce-grid-api-openapi.yml]\n\nsummary:\n  scope_count: 22\n  naming_convention: <Service>_<Domain>_<Level>\n  services: [RetailMedia, MarketingSolutions, CommerceGrid]\n  levels: [Read, Manage]\n  read_scopes: 11\n  manage_scopes: 11\n  requested_at_token_time: false\n  bound_to_application: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/scopes/criteo-scopes.yml
summary_line: 22 scopes · clientCredentials/authorizationCode
tags:
- Advertising
- Agent Skills
- Analytics
- Audiences
- Campaigns
- Catalog
- Commerce
- Commerce Media
- Display Advertising
- Marketing
- MCP
- Media
- OAuth 2.0
- OpenAPI
- Reporting
- Retail
- Retail Media
- Sponsored Products
token_urls:
- https://api.criteo.com/oauth2/token
---
