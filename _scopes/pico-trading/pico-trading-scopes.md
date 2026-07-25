---
authorization_urls:
- https://portal.pico.net/services/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Pico Trading Scopes
name_suffix: OAuth Scopes
note: Pico publishes no public product-API OAuth documentation. These are the scopes_supported advertised by the authorization server of the login-gated Salesforce Experience Cloud customer portal (portal.pico.net) that gates all product and Corvil API documentation. They are Salesforce platform scopes, not Pico product-API scopes; descriptions are intentionally omitted rather than inferred.
overview: 'Pico publishes 36 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Pico API on a user''s behalf.


  Tokens are issued from https://portal.pico.net/services/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Pico
provider_slug: pico-trading
schemes:
- flows:
  - authorizationUrl: https://portal.pico.net/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://portal.pico.net/services/oauth2/token
  name: portalOAuth2
  source: well-known/pico-trading-openid-configuration.json
scope_count: 36
scope_names:
- address
- api
- cdp_api
- cdp_calculated_insight_api
- cdp_identityresolution_api
- cdp_ingest_api
- cdp_profile_api
- cdp_query_api
- cdp_segment_api
- chatbot_api
- chatter_api
- content
- custom_permissions
- data_cloud_user_claims
- eclair_api
- einstein_gpt_api
- email
- forgot_password
- full
- id
- interaction_api
- lightning
- mcp_api
- offline_access
- openid
- pardot_api
- phone
- profile
- pwdless_login_api
- refresh_token
- scrt_api
- sfap_api
- user_registration_api
- visualforce
- wave_api
- web
scopes:
- description: ''
  flows: []
  scope: address
- description: ''
  flows: []
  scope: api
- description: ''
  flows: []
  scope: cdp_api
- description: ''
  flows: []
  scope: cdp_calculated_insight_api
- description: ''
  flows: []
  scope: cdp_identityresolution_api
- description: ''
  flows: []
  scope: cdp_ingest_api
- description: ''
  flows: []
  scope: cdp_profile_api
- description: ''
  flows: []
  scope: cdp_query_api
- description: ''
  flows: []
  scope: cdp_segment_api
- description: ''
  flows: []
  scope: chatbot_api
- description: ''
  flows: []
  scope: chatter_api
- description: ''
  flows: []
  scope: content
- description: ''
  flows: []
  scope: custom_permissions
- description: ''
  flows: []
  scope: data_cloud_user_claims
- description: ''
  flows: []
  scope: eclair_api
- description: ''
  flows: []
  scope: einstein_gpt_api
- description: ''
  flows: []
  scope: email
- description: ''
  flows: []
  scope: forgot_password
- description: ''
  flows: []
  scope: full
- description: ''
  flows: []
  scope: id
- description: ''
  flows: []
  scope: interaction_api
- description: ''
  flows: []
  scope: lightning
- description: ''
  flows: []
  scope: mcp_api
- description: ''
  flows: []
  scope: offline_access
- description: ''
  flows: []
  scope: openid
- description: ''
  flows: []
  scope: pardot_api
- description: ''
  flows: []
  scope: phone
- description: ''
  flows: []
  scope: profile
- description: ''
  flows: []
  scope: pwdless_login_api
- description: ''
  flows: []
  scope: refresh_token
- description: ''
  flows: []
  scope: scrt_api
- description: ''
  flows: []
  scope: sfap_api
- description: ''
  flows: []
  scope: user_registration_api
- description: ''
  flows: []
  scope: visualforce
- description: ''
  flows: []
  scope: wave_api
- description: ''
  flows: []
  scope: web
slug: pico-trading-scopes
source_filename: pico-trading-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: https://portal.pico.net/.well-known/openid-configuration\nnote: Pico publishes no public product-API OAuth documentation. These are the\n  scopes_supported advertised by the authorization server of the login-gated\n  Salesforce Experience Cloud customer portal (portal.pico.net) that gates all\n  product and Corvil API documentation. They are Salesforce platform scopes,\n  not Pico product-API scopes; descriptions are intentionally omitted rather\n  than inferred.\nschemes:\n- name: portalOAuth2\n  source: well-known/pico-trading-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://portal.pico.net/services/oauth2/authorize\n    tokenUrl: https://portal.pico.net/services/oauth2/token\nscopes:\n- scope: address\n  sources:\n  - well-known/pico-trading-openid-configuration.json\n- scope: api\n  sources:\n  - well-known/pico-trading-openid-configuration.json\n- scope: cdp_api\n  sources:\n\
  \  - well-known/pico-trading-openid-configuration.json\n- scope: cdp_calculated_insight_api\n  sources:\n  - well-known/pico-trading-openid-configuration.json\n- scope: cdp_identityresolution_api\n  sources:\n  - well-known/pico-trading-openid-configuration.json\n- scope: cdp_ingest_api\n  sources:\n  - well-known/pico-trading-openid-configuration.json\n- scope: cdp_profile_api\n  sources:\n  - well-known/pico-trading-openid-configuration.json\n- scope: cdp_query_api\n  sources:\n  - well-known/pico-trading-openid-configuration.json\n- scope: cdp_segment_api\n  sources:\n  - well-known/pico-trading-openid-configuration.json\n- scope: chatbot_api\n  sources:\n  - well-known/pico-trading-openid-configuration.json\n- scope: chatter_api\n  sources:\n  - well-known/pico-trading-openid-configuration.json\n- scope: content\n  sources:\n  - well-known/pico-trading-openid-configuration.json\n- scope: custom_permissions\n  sources:\n  - well-known/pico-trading-openid-configuration.json\n- scope:\
  \ data_cloud_user_claims\n  sources:\n  - well-known/pico-trading-openid-configuration.json\n- scope: eclair_api\n  sources:\n  - well-known/pico-trading-openid-configuration.json\n- scope: einstein_gpt_api\n  sources:\n  - well-known/pico-trading-openid-configuration.json\n- scope: email\n  sources:\n  - well-known/pico-trading-openid-configuration.json\n- scope: forgot_password\n  sources:\n  - well-known/pico-trading-openid-configuration.json\n- scope: full\n  sources:\n  - well-known/pico-trading-openid-configuration.json\n- scope: id\n  sources:\n  - well-known/pico-trading-openid-configuration.json\n- scope: interaction_api\n  sources:\n  - well-known/pico-trading-openid-configuration.json\n- scope: lightning\n  sources:\n  - well-known/pico-trading-openid-configuration.json\n- scope: mcp_api\n  sources:\n  - well-known/pico-trading-openid-configuration.json\n- scope: offline_access\n  sources:\n  - well-known/pico-trading-openid-configuration.json\n- scope: openid\n  sources:\n\
  \  - well-known/pico-trading-openid-configuration.json\n- scope: pardot_api\n  sources:\n  - well-known/pico-trading-openid-configuration.json\n- scope: phone\n  sources:\n  - well-known/pico-trading-openid-configuration.json\n- scope: profile\n  sources:\n  - well-known/pico-trading-openid-configuration.json\n- scope: pwdless_login_api\n  sources:\n  - well-known/pico-trading-openid-configuration.json\n- scope: refresh_token\n  sources:\n  - well-known/pico-trading-openid-configuration.json\n- scope: scrt_api\n  sources:\n  - well-known/pico-trading-openid-configuration.json\n- scope: sfap_api\n  sources:\n  - well-known/pico-trading-openid-configuration.json\n- scope: user_registration_api\n  sources:\n  - well-known/pico-trading-openid-configuration.json\n- scope: visualforce\n  sources:\n  - well-known/pico-trading-openid-configuration.json\n- scope: wave_api\n  sources:\n  - well-known/pico-trading-openid-configuration.json\n- scope: web\n  sources:\n  - well-known/pico-trading-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pico-trading/refs/heads/main/scopes/pico-trading-scopes.yml
summary_line: 36 scopes · authorizationCode
tags:
- Financial
- Market Data
- Trading
- Real-Time
- Low Latency
- Feed Handlers
- Order Execution
- Network Analytics
- Exchange Connectivity
token_urls:
- https://portal.pico.net/services/oauth2/token
---
