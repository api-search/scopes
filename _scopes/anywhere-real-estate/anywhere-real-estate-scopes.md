---
authorization_urls: []
description: ''
docs: https://developers.anywhere.re/docs/realogy-oauth
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Anywhere Real Estate Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Anywhere Real Estate uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Anywhere Real Estate
provider_slug: anywhere-real-estate
schemes:
- authorization_server_non_production: https://realogy.oktapreview.com/oauth2/ausdtpyw647fbrcPi0h7
  authorization_server_production: https://realogy.okta.com/oauth2/aus7i8b1taFyPOEGc1t7
  flow: clientCredentials
  name: AnywhereOAuth2
  source: https://developers.anywhere.re/docs/realogy-oauth
  token_endpoint_non_production: https://realogy.oktapreview.com/oauth2/ausdtpyw647fbrcPi0h7/v1/token
  token_endpoint_production: https://realogy.okta.com/oauth2/aus7i8b1taFyPOEGc1t7/v1/token
scope_count: 0
scope_names: []
scopes: []
slug: anywhere-real-estate-scopes
source_filename: anywhere-real-estate-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: https://developers.anywhere.re/docs/realogy-oauth\ndocs: https://developers.anywhere.re/docs/realogy-oauth\nmodel: App ID URI\ncaution: >-\n  Anywhere OAuth scopes are Azure/Okta-style App ID URIs — opaque identifiers for a REST\n  API, NOT base URLs. The OAuth guide states verbatim \"The App ID URI is a unique\n  identifier for the REST API. It is not where the REST API is hosted.\" Probing\n  https://btt.realogyfg.com/ does not resolve. Never treat a scope value as a host.\nassignment: >-\n  Scopes are granted per approved application (\"Scope: Will be communicated in the final\n  approval\"). A developer cannot self-select scopes; the set is bound to the API products\n  the application was approved for. Scope is passed to the Okta token endpoint as a\n  space-separated list.\nschemes:\n- name: AnywhereOAuth2\n  flow: clientCredentials\n  authorization_server_production: https://realogy.okta.com/oauth2/aus7i8b1taFyPOEGc1t7\n\
  \  authorization_server_non_production: https://realogy.oktapreview.com/oauth2/ausdtpyw647fbrcPi0h7\n  token_endpoint_production: https://realogy.okta.com/oauth2/aus7i8b1taFyPOEGc1t7/v1/token\n  token_endpoint_non_production: https://realogy.oktapreview.com/oauth2/ausdtpyw647fbrcPi0h7/v1/token\n  source: https://developers.anywhere.re/docs/realogy-oauth\nproduct_scopes:\n- scope: https://btt.realogyfg.com/dashapi\n  description: Dash back-office API. Named as the worked example in the OAuth guide.\n  product: Back Office Management (backoffice)\n  source: https://developers.anywhere.re/docs/realogy-oauth\n- scope: https://btt.realogyfg.com/datasyncapi\n  description: Datasync marketing/listing syndication API.\n  product: Listing Syndication (listing-syndication)\n- scope: https://btt.realogyfg.com/corporatestaffapi\n  description: Corporate Staff master data API.\n  product: Marketing - Franchise (broker-agent-tools)\n- scope: https://btt.realogyfg.com/transactionsapi\n  description:\
  \ Brokerage production / transactions API.\n  product: Transactions - Franchise (realogy-broker-production)\n- scope: https://btt.realogyfg.com/dynamicsearchapi\n  description: Real-time dynamic search over listing details.\n  product: Dynamic Search (dynamic-search)\n- scope: https://btt.realogyfg.com/propertypromotionsapi\n  description: Listing promotions, channels and publication lists.\n  product: Listings Promotions (property-promotions)\n- scope: https://btt.realogyfg.com/analyticsapi\n  description: Listing metrics and analytics.\n  product: Listing Metric (realogy-listings-metrics)\n- scope: https://btt.realogyfg.com/securityapi\n  description: User access / security API on the BTT estate.\n  product: User Access Management (realogy-user-access)\n- scope: https://dataservices.eap.com/eaplistingsapi\n  description: >-\n    MLS Data Service listings API. Confirmed verbatim on the MLS Data Service product\n    page Requirements section - \"Okta scope - https://dataservices.eap.com/eaplistingsapi\"\
  .\n  product: MLS Data Service (mls-data-service)\n  source: https://developers.anywhere.re/api-product/mls-data-service/summary\n- scope: https://api.realogy.com/leadrouterapi\n  description: Lead routing API.\n  product: Leads Management / Leads Engine\n- scope: https://api.realogy.com/iprospectapi\n  description: iProspect agent recruiting API.\n  product: Agent Recruiting (iprospect)\n- scope: https://api.realogy.com/c2shinningcapi\n  description: Consumer Journey (AIS Homebase) API.\n  product: Consumer Journey (c2shinningc)\n- scope: https://api.realogy.com/referralleadsapi\n  description: Referral leads API.\n  product: Referral Partner Integration / Referral Leads\n- scope: https://api.realogy.com/reloauthorizationapi\n  description: Cartus relocation authorization API.\n  product: Relocation Authorization (relocationauthorization)\n- scope: https://api.realogy.com/realvitalizevendorsapi\n  description: RealVitalize vendor services API.\n  product: RealVitalize (realvitalize-vendor-services)\n\
  - scope: https://api.realogy.com/settlementcompanycapabilityapi\n  description: Anywhere Integrated Services settlement company API.\n  product: Settlement Company (settlement-company-capability)\n- scope: https://api.anywhere.re/referralpartnerintegration\n  description: Referral Partner Integration API.\n  product: Referral Partner Integration (referral-partner-integration)\n- scope: https://eps.nrtllc.com/securityapi\n  description: User access / security API on the EPS (NRT) estate.\n  product: User Access Management (realogy-user-access)\n- scope: apim-listingextensions\n  description: >-\n    Listing Extensions API. The only documented scope that is a bare identifier rather\n    than an App ID URI.\n  product: Listing Extensions (listingextensions)\nauthorization_server_scopes:\n  note: >-\n    Scopes advertised by the Okta authorization servers themselves (harvested from the\n    RFC 8414 metadata). These are the standard OIDC/Okta scopes, separate from the\n    per-product App\
  \ ID URIs above, and are not the scopes an API product consumer is\n    granted.\n  production:\n  - https://agentx.com/userconfig\n  - interclient_access\n  - memberOf\n  - okta.myAccount.appAuthenticator.maintenance.manage\n  - okta.myAccount.appAuthenticator.maintenance.read\n  - okta.myAccount.appAuthenticator.manage\n  - okta.myAccount.appAuthenticator.read\n  - openid\n  - profile\n  - email\n  - address\n  - phone\n  - offline_access\n  - device_sso\n  non_production:\n  - interclient_access\n  - memberOf\n  - okta.myAccount.appAuthenticator.maintenance.manage\n  - okta.myAccount.appAuthenticator.maintenance.read\n  - okta.myAccount.appAuthenticator.manage\n  - okta.myAccount.appAuthenticator.read\n  - openid\n  - profile\n  - email\n  - address\n  - phone\n  - offline_access\n  - device_sso\n  sources:\n  - authentication/anywhere-real-estate-okta-prod-authorization-server.json\n  - authentication/anywhere-real-estate-okta-nonprod-authorization-server.json\ngaps:\n- 19 product\
  \ scopes are published anonymously but Anywhere lists 23 API products; there\n  is no anonymously published scope for several products (including the Partner-only\n  Leads Engine).\n- No scope-to-operation mapping is public, because every API specification is login-gated.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anywhere-real-estate/refs/heads/main/scopes/anywhere-real-estate-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Real Estate
- United States
- Property Listings
- MLS
- RESO
- Brokerage
- Franchising
- PropTech
- Title
- Escrow
- Relocation
- Leads
- Transactions
token_urls: []
---
