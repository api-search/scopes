---
api_specs:
- filename: bureau-of-land-management-gbp-hub-search-openapi.json
  format: json
  label: BLM GBP Hub Search API (OGC API - Records)
  slug: blm-gbp-hub-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bureau-of-land-management/refs/heads/main/openapi/bureau-of-land-management-gbp-hub-search-openapi.json
authorization_urls:
- https://mlrs.blm.gov/services/oauth2/authorize
- https://glorecords.blm.gov/services/oauth2/authorize
- https://blm-egis.maps.arcgis.com/sharing/rest/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Bureau Of Land Management Scopes
name_suffix: OAuth Scopes
note: 'READ THIS BEFORE USING THE SCOPE LIST. BLM authors none of these scopes. MLRS and GLO Records run on Salesforce Experience Cloud, and their discovery documents advertise the stock Salesforce platform scope set — identical strings on both hosts, including scopes for products BLM plainly does not operate through these sites (pardot_api, einstein_gpt_api, cdp_*). They describe what the PLATFORM can issue, not what BLM grants. BLM publishes no scopes/permissions reference page of its own. Both surfaces are, in practice, closed: every non-discovery path on both hosts answered 401 to an anonymous client on 2026-09-05, and there is no self-service developer registration. The public geospatial surface — the GBP Hub Search API, the 13 ArcGIS Server instances and the WMS endpoints — has NO scope model because it has no authentication at all.'
overview: 'Bureau of Land Management publishes 12 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Bureau of Land Management API on a user''s behalf.


  Tokens are issued from https://mlrs.blm.gov/services/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bureau of Land Management
provider_slug: bureau-of-land-management
schemes:
- flows:
  - authorizationUrl: https://mlrs.blm.gov/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://mlrs.blm.gov/services/oauth2/token
  name: mlrs-oidc
  scope_authorship: salesforce-platform-default
  source: well-known/bureau-of-land-management-mlrs-openid-configuration.json
  surface: https://mlrs.blm.gov
- flows:
  - authorizationUrl: https://glorecords.blm.gov/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://glorecords.blm.gov/services/oauth2/token
  name: glorecords-oidc
  scope_authorship: salesforce-platform-default
  source: well-known/bureau-of-land-management-glorecords-openid-configuration.json
  surface: https://glorecords.blm.gov
- flows:
  - authorizationUrl: https://blm-egis.maps.arcgis.com/sharing/rest/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://blm-egis.maps.arcgis.com/sharing/rest/oauth2/token
  name: arcgis-online-oauth2
  note: The RFC 8414 document advertises no scopes_supported array at all.
  scope_authorship: esri-platform-default
  source: well-known/bureau-of-land-management-blm-egis-arcgis-oauth-authorization-server.json
  surface: https://blm-egis.maps.arcgis.com
scope_count: 12
scope_names:
- openid
- profile
- email
- address
- phone
- id
- api
- web
- refresh_token
- offline_access
- content
- full
scopes:
- description: OpenID Connect — issue an ID token.
  flows:
  - authorizationCode
  scope: openid
- description: Basic profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Email claim.
  flows:
  - authorizationCode
  scope: email
- description: Address claim.
  flows:
  - authorizationCode
  scope: address
- description: Phone claim.
  flows:
  - authorizationCode
  scope: phone
- description: Identity URL access.
  flows:
  - authorizationCode
  scope: id
- description: Access the platform data API on behalf of the user.
  flows:
  - authorizationCode
  scope: api
- description: Web session access.
  flows:
  - authorizationCode
  scope: web
- description: Issue a refresh token.
  flows:
  - authorizationCode
  scope: refresh_token
- description: Long-lived access (alias of refresh_token on this platform).
  flows:
  - authorizationCode
  scope: offline_access
- description: Content/document access.
  flows:
  - authorizationCode
  scope: content
- description: Full access to everything the user can reach.
  flows:
  - authorizationCode
  scope: full
slug: bureau-of-land-management-scopes
source_filename: bureau-of-land-management-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: >-\n  well-known/bureau-of-land-management-mlrs-openid-configuration.json,\n  well-known/bureau-of-land-management-glorecords-openid-configuration.json,\n  well-known/bureau-of-land-management-blm-egis-arcgis-oauth-authorization-server.json\nnote: |\n  READ THIS BEFORE USING THE SCOPE LIST. BLM authors none of these scopes. MLRS and GLO Records\n  run on Salesforce Experience Cloud, and their discovery documents advertise the stock\n  Salesforce platform scope set — identical strings on both hosts, including scopes for\n  products BLM plainly does not operate through these sites (pardot_api, einstein_gpt_api,\n  cdp_*). They describe what the PLATFORM can issue, not what BLM grants.\n\n  BLM publishes no scopes/permissions reference page of its own. Both surfaces are, in\n  practice, closed: every non-discovery path on both hosts answered 401 to an anonymous\n  client on 2026-09-05, and there is no self-service developer registration.\n\
  \n  The public geospatial surface — the GBP Hub Search API, the 13 ArcGIS Server instances and\n  the WMS endpoints — has NO scope model because it has no authentication at all.\nschemes:\n  - name: mlrs-oidc\n    surface: https://mlrs.blm.gov\n    source: well-known/bureau-of-land-management-mlrs-openid-configuration.json\n    scope_authorship: salesforce-platform-default\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://mlrs.blm.gov/services/oauth2/authorize\n        tokenUrl: https://mlrs.blm.gov/services/oauth2/token\n  - name: glorecords-oidc\n    surface: https://glorecords.blm.gov\n    source: well-known/bureau-of-land-management-glorecords-openid-configuration.json\n    scope_authorship: salesforce-platform-default\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://glorecords.blm.gov/services/oauth2/authorize\n        tokenUrl: https://glorecords.blm.gov/services/oauth2/token\n  - name: arcgis-online-oauth2\n    surface:\
  \ https://blm-egis.maps.arcgis.com\n    source: well-known/bureau-of-land-management-blm-egis-arcgis-oauth-authorization-server.json\n    scope_authorship: esri-platform-default\n    note: The RFC 8414 document advertises no scopes_supported array at all.\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://blm-egis.maps.arcgis.com/sharing/rest/oauth2/authorize\n        tokenUrl: https://blm-egis.maps.arcgis.com/sharing/rest/oauth2/token\nscopes:\n  - scope: openid\n    description: OpenID Connect — issue an ID token.\n    flows: [authorizationCode]\n    sources: [mlrs-oidc, glorecords-oidc]\n  - scope: profile\n    description: Basic profile claims.\n    flows: [authorizationCode]\n    sources: [mlrs-oidc, glorecords-oidc]\n  - scope: email\n    description: Email claim.\n    flows: [authorizationCode]\n    sources: [mlrs-oidc, glorecords-oidc]\n  - scope: address\n    description: Address claim.\n    flows: [authorizationCode]\n    sources: [mlrs-oidc, glorecords-oidc]\n\
  \  - scope: phone\n    description: Phone claim.\n    flows: [authorizationCode]\n    sources: [mlrs-oidc, glorecords-oidc]\n  - scope: id\n    description: Identity URL access.\n    flows: [authorizationCode]\n    sources: [mlrs-oidc, glorecords-oidc]\n  - scope: api\n    description: Access the platform data API on behalf of the user.\n    flows: [authorizationCode]\n    sources: [mlrs-oidc, glorecords-oidc]\n  - scope: web\n    description: Web session access.\n    flows: [authorizationCode]\n    sources: [mlrs-oidc, glorecords-oidc]\n  - scope: refresh_token\n    description: Issue a refresh token.\n    flows: [authorizationCode]\n    sources: [mlrs-oidc, glorecords-oidc]\n  - scope: offline_access\n    description: Long-lived access (alias of refresh_token on this platform).\n    flows: [authorizationCode]\n    sources: [mlrs-oidc, glorecords-oidc]\n  - scope: content\n    description: Content/document access.\n    flows: [authorizationCode]\n    sources: [mlrs-oidc, glorecords-oidc]\n\
  \  - scope: full\n    description: Full access to everything the user can reach.\n    flows: [authorizationCode]\n    sources: [mlrs-oidc, glorecords-oidc]\nplatform_default_scopes_not_wired_by_blm:\n  - custom_permissions\n  - visualforce\n  - lightning\n  - chatter_api\n  - wave_api\n  - eclair_api\n  - interaction_api\n  - chatbot_api\n  - einstein_gpt_api\n  - sfap_api\n  - scrt_api\n  - pardot_api\n  - user_registration_api\n  - pwdless_login_api\n  - forgot_password\n  - data_cloud_user_claims\n  - mcp_api\n  - cdp_api\n  - cdp_ingest_api\n  - cdp_query_api\n  - cdp_segment_api\n  - cdp_profile_api\n  - cdp_identityresolution_api\n  - cdp_calculated_insight_api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bureau-of-land-management/refs/heads/main/scopes/bureau-of-land-management-scopes.yml
summary_line: 12 scopes · authorizationCode
tags:
- Environment
- Federal-Government
- Land
- Resources
- GIS
- Geospatial
- Mining
- Public-Lands
- Open-Data
- OGC
- Cadastral
- Recreation
- Grazing
- ArcGIS
- DCAT
- Conservation
- Mapping
token_urls:
- https://mlrs.blm.gov/services/oauth2/token
- https://glorecords.blm.gov/services/oauth2/token
- https://blm-egis.maps.arcgis.com/sharing/rest/oauth2/token
---
