---
authorization_urls:
- https://shopify.com/authentication/85271511350/oauth/authorize
- https://network.flo.com/services/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Flo Ev Scopes
name_suffix: OAuth Scopes
note: FLO defines no OAuth scopes of its own. Every scope below is advertised by a platform FLO hosts under a flo.com name - Shopify Customer Accounts on store.flo.com and Salesforce Experience Cloud on network.flo.com - and is recorded because it is the only real, machine-readable authorization surface in FLO's estate. None of these scopes grants access to charging sessions, station telemetry, roaming (OCPI) or demand response (OpenADR); those remain partner-mediated with no published authorization model.
overview: 'FLO publishes 38 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the FLO API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/85271511350/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: FLO
provider_slug: flo-ev
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/85271511350/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/85271511350/oauth/token
  issuer: https://shopify.com/authentication/85271511350
  name: shopify-customer-accounts
  source: well-known/flo-ev-store-openid-configuration.json
- flows:
  - authorizationUrl: https://network.flo.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://network.flo.com/services/oauth2/token
  issuer: https://network.flo.com
  name: salesforce-experience-cloud
  source: well-known/flo-ev-network-openid-configuration.json
scope_count: 38
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
- profile
- address
- phone
- id
- api
- web
- full
- refresh_token
- offline_access
- content
- custom_permissions
- lightning
- visualforce
- chatter_api
- chatbot_api
- interaction_api
- wave_api
- eclair_api
- pardot_api
- scrt_api
- sfap_api
- mcp_api
- einstein_gpt_api
- cdp_api
- cdp_query_api
- cdp_profile_api
- cdp_ingest_api
- cdp_segment_api
- cdp_identityresolution_api
- cdp_calculated_insight_api
- data_cloud_user_claims
- user_registration_api
- pwdless_login_api
- forgot_password
scopes:
- description: OIDC authentication
  flows:
  - authorizationCode
  scope: openid
- description: Email address claim
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the signed-in FLO store customer
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API - the authenticated half of the MCP server at https://store.flo.com/api/mcp
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
- description: ''
  flows: []
  scope: profile
- description: ''
  flows: []
  scope: address
- description: ''
  flows: []
  scope: phone
- description: ''
  flows: []
  scope: id
- description: Salesforce REST/SOAP platform API access
  flows: []
  scope: api
- description: ''
  flows: []
  scope: web
- description: ''
  flows: []
  scope: full
- description: ''
  flows: []
  scope: refresh_token
- description: ''
  flows: []
  scope: offline_access
- description: ''
  flows: []
  scope: content
- description: ''
  flows: []
  scope: custom_permissions
- description: ''
  flows: []
  scope: lightning
- description: ''
  flows: []
  scope: visualforce
- description: ''
  flows: []
  scope: chatter_api
- description: ''
  flows: []
  scope: chatbot_api
- description: ''
  flows: []
  scope: interaction_api
- description: ''
  flows: []
  scope: wave_api
- description: ''
  flows: []
  scope: eclair_api
- description: ''
  flows: []
  scope: pardot_api
- description: ''
  flows: []
  scope: scrt_api
- description: ''
  flows: []
  scope: sfap_api
- description: Salesforce platform MCP scope advertised by the community org (no MCP endpoint was reachable anonymously)
  flows: []
  scope: mcp_api
- description: ''
  flows: []
  scope: einstein_gpt_api
- description: ''
  flows: []
  scope: cdp_api
- description: ''
  flows: []
  scope: cdp_query_api
- description: ''
  flows: []
  scope: cdp_profile_api
- description: ''
  flows: []
  scope: cdp_ingest_api
- description: ''
  flows: []
  scope: cdp_segment_api
- description: ''
  flows: []
  scope: cdp_identityresolution_api
- description: ''
  flows: []
  scope: cdp_calculated_insight_api
- description: ''
  flows: []
  scope: data_cloud_user_claims
- description: ''
  flows: []
  scope: user_registration_api
- description: ''
  flows: []
  scope: pwdless_login_api
- description: ''
  flows: []
  scope: forgot_password
slug: flo-ev-scopes
source_filename: flo-ev-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: >-\n  https://store.flo.com/.well-known/openid-configuration and\n  https://network.flo.com/.well-known/openid-configuration (both HTTP 200,\n  fetched 2026-07-27)\nnote: >-\n  FLO defines no OAuth scopes of its own. Every scope below is advertised by a\n  platform FLO hosts under a flo.com name - Shopify Customer Accounts on\n  store.flo.com and Salesforce Experience Cloud on network.flo.com - and is\n  recorded because it is the only real, machine-readable authorization surface\n  in FLO's estate. None of these scopes grants access to charging sessions,\n  station telemetry, roaming (OCPI) or demand response (OpenADR); those remain\n  partner-mediated with no published authorization model.\nschemes:\n- name: shopify-customer-accounts\n  source: well-known/flo-ev-store-openid-configuration.json\n  issuer: https://shopify.com/authentication/85271511350\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/85271511350/oauth/authorize\n\
  \    tokenUrl: https://shopify.com/authentication/85271511350/oauth/token\n- name: salesforce-experience-cloud\n  source: well-known/flo-ev-network-openid-configuration.json\n  issuer: https://network.flo.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://network.flo.com/services/oauth2/authorize\n    tokenUrl: https://network.flo.com/services/oauth2/token\nscopes:\n- {scope: openid, description: OIDC authentication, flows: [authorizationCode], sources: [store.flo.com, network.flo.com]}\n- {scope: email, description: Email address claim, flows: [authorizationCode], sources: [store.flo.com, network.flo.com]}\n- {scope: 'customer-account-api:full', description: Full access to the Shopify Customer Account API for the signed-in FLO store customer, flows: [authorizationCode], sources: [store.flo.com]}\n- {scope: 'customer-account-mcp-api:full', description: Full access to the Shopify Customer Account MCP API - the authenticated half of the MCP server at https://store.flo.com/api/mcp,\
  \ flows: [authorizationCode], sources: [store.flo.com]}\n- {scope: profile, sources: [network.flo.com]}\n- {scope: address, sources: [network.flo.com]}\n- {scope: phone, sources: [network.flo.com]}\n- {scope: id, sources: [network.flo.com]}\n- {scope: api, description: Salesforce REST/SOAP platform API access, sources: [network.flo.com]}\n- {scope: web, sources: [network.flo.com]}\n- {scope: full, sources: [network.flo.com]}\n- {scope: refresh_token, sources: [network.flo.com]}\n- {scope: offline_access, sources: [network.flo.com]}\n- {scope: content, sources: [network.flo.com]}\n- {scope: custom_permissions, sources: [network.flo.com]}\n- {scope: lightning, sources: [network.flo.com]}\n- {scope: visualforce, sources: [network.flo.com]}\n- {scope: chatter_api, sources: [network.flo.com]}\n- {scope: chatbot_api, sources: [network.flo.com]}\n- {scope: interaction_api, sources: [network.flo.com]}\n- {scope: wave_api, sources: [network.flo.com]}\n- {scope: eclair_api, sources: [network.flo.com]}\n\
  - {scope: pardot_api, sources: [network.flo.com]}\n- {scope: scrt_api, sources: [network.flo.com]}\n- {scope: sfap_api, sources: [network.flo.com]}\n- {scope: mcp_api, description: Salesforce platform MCP scope advertised by the community org (no MCP endpoint was reachable anonymously), sources: [network.flo.com]}\n- {scope: einstein_gpt_api, sources: [network.flo.com]}\n- {scope: cdp_api, sources: [network.flo.com]}\n- {scope: cdp_query_api, sources: [network.flo.com]}\n- {scope: cdp_profile_api, sources: [network.flo.com]}\n- {scope: cdp_ingest_api, sources: [network.flo.com]}\n- {scope: cdp_segment_api, sources: [network.flo.com]}\n- {scope: cdp_identityresolution_api, sources: [network.flo.com]}\n- {scope: cdp_calculated_insight_api, sources: [network.flo.com]}\n- {scope: data_cloud_user_claims, sources: [network.flo.com]}\n- {scope: user_registration_api, sources: [network.flo.com]}\n- {scope: pwdless_login_api, sources: [network.flo.com]}\n- {scope: forgot_password, sources: [network.flo.com]}\n\
  counts:\n  total_unique: 38\n  flo_defined: 0\n  shopify_platform: 4\n  salesforce_platform: 36\n  shared_by_both: 2\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flo-ev/refs/heads/main/scopes/flo-ev-scopes.yml
summary_line: 38 scopes · authorizationCode
tags:
- Energy
- Canada
- EV Charging
- Electricity
- Grid
- Demand Response
- Interoperability
- OCPP
- OCPI
- OpenADR
- Charge Point Operator
- Quebec
token_urls:
- https://shopify.com/authentication/85271511350/oauth/token
- https://network.flo.com/services/oauth2/token
---
