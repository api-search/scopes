---
authorization_urls:
- https://portal.firstsolar.com/developer/services/oauth2/authorize
description: ''
docs: https://portal.firstsolar.com/developer/PortalCustomLogin
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: First Solar Scopes
name_suffix: OAuth Scopes
note: 'Served by the Salesforce Experience Cloud tenant that runs the First Solar Developer Portal (portal.firstsolar.com) — First Solar''s own host and its own OIDC issuer. The endpoints and the scope vocabulary are Salesforce platform-standard, not a First Solar-authored API contract: First Solar publishes no API product of its own. Recorded because it is a real, unauthenticated, machine-readable document the provider serves. The scope names below are Salesforce''s platform scope vocabulary as advertised by this tenant''s discovery document; they are not First Solar product scopes. No scope reference page is published — the Developer Portal is behind a login.'
overview: 'First Solar publishes 36 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the First Solar API on a user''s behalf.


  Tokens are issued from https://portal.firstsolar.com/developer/services/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: First Solar
provider_slug: first-solar
schemes:
- flows:
  - authorizationUrl: https://portal.firstsolar.com/developer/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://portal.firstsolar.com/developer/services/oauth2/token
  name: OAuth2
  source: well-known/first-solar-openid-configuration.json
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
  flows:
  - authorizationCode
  scope: address
- description: ''
  flows:
  - authorizationCode
  scope: api
- description: ''
  flows:
  - authorizationCode
  scope: cdp_api
- description: ''
  flows:
  - authorizationCode
  scope: cdp_calculated_insight_api
- description: ''
  flows:
  - authorizationCode
  scope: cdp_identityresolution_api
- description: ''
  flows:
  - authorizationCode
  scope: cdp_ingest_api
- description: ''
  flows:
  - authorizationCode
  scope: cdp_profile_api
- description: ''
  flows:
  - authorizationCode
  scope: cdp_query_api
- description: ''
  flows:
  - authorizationCode
  scope: cdp_segment_api
- description: ''
  flows:
  - authorizationCode
  scope: chatbot_api
- description: ''
  flows:
  - authorizationCode
  scope: chatter_api
- description: ''
  flows:
  - authorizationCode
  scope: content
- description: ''
  flows:
  - authorizationCode
  scope: custom_permissions
- description: ''
  flows:
  - authorizationCode
  scope: data_cloud_user_claims
- description: ''
  flows:
  - authorizationCode
  scope: eclair_api
- description: ''
  flows:
  - authorizationCode
  scope: einstein_gpt_api
- description: ''
  flows:
  - authorizationCode
  scope: email
- description: ''
  flows:
  - authorizationCode
  scope: forgot_password
- description: ''
  flows:
  - authorizationCode
  scope: full
- description: ''
  flows:
  - authorizationCode
  scope: id
- description: ''
  flows:
  - authorizationCode
  scope: interaction_api
- description: ''
  flows:
  - authorizationCode
  scope: lightning
- description: ''
  flows:
  - authorizationCode
  scope: mcp_api
- description: ''
  flows:
  - authorizationCode
  scope: offline_access
- description: ''
  flows:
  - authorizationCode
  scope: openid
- description: ''
  flows:
  - authorizationCode
  scope: pardot_api
- description: ''
  flows:
  - authorizationCode
  scope: phone
- description: ''
  flows:
  - authorizationCode
  scope: profile
- description: ''
  flows:
  - authorizationCode
  scope: pwdless_login_api
- description: ''
  flows:
  - authorizationCode
  scope: refresh_token
- description: ''
  flows:
  - authorizationCode
  scope: scrt_api
- description: ''
  flows:
  - authorizationCode
  scope: sfap_api
- description: ''
  flows:
  - authorizationCode
  scope: user_registration_api
- description: ''
  flows:
  - authorizationCode
  scope: visualforce
- description: ''
  flows:
  - authorizationCode
  scope: wave_api
- description: ''
  flows:
  - authorizationCode
  scope: web
slug: first-solar-scopes
source_filename: first-solar-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: probed\nsource: https://portal.firstsolar.com/.well-known/openid-configuration\ndocs: https://portal.firstsolar.com/developer/PortalCustomLogin\nnote: 'Served by the Salesforce Experience Cloud tenant that runs the First Solar Developer Portal (portal.firstsolar.com)\n  — First Solar''s own host and its own OIDC issuer. The endpoints and the scope vocabulary are Salesforce\n  platform-standard, not a First Solar-authored API contract: First Solar publishes no API product of\n  its own. Recorded because it is a real, unauthenticated, machine-readable document the provider serves.\n  The scope names below are Salesforce''s platform scope vocabulary as advertised by this tenant''s discovery\n  document; they are not First Solar product scopes. No scope reference page is published — the Developer\n  Portal is behind a login.'\nschemes:\n- name: OAuth2\n  source: well-known/first-solar-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n\
  \    authorizationUrl: https://portal.firstsolar.com/developer/services/oauth2/authorize\n    tokenUrl: https://portal.firstsolar.com/developer/services/oauth2/token\nscope_count: 36\nscopes:\n- scope: address\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/first-solar-openid-configuration.json\n- scope: api\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/first-solar-openid-configuration.json\n- scope: cdp_api\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/first-solar-openid-configuration.json\n- scope: cdp_calculated_insight_api\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/first-solar-openid-configuration.json\n- scope: cdp_identityresolution_api\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/first-solar-openid-configuration.json\n- scope: cdp_ingest_api\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/first-solar-openid-configuration.json\n- scope: cdp_profile_api\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - well-known/first-solar-openid-configuration.json\n- scope: cdp_query_api\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/first-solar-openid-configuration.json\n- scope: cdp_segment_api\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/first-solar-openid-configuration.json\n- scope: chatbot_api\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/first-solar-openid-configuration.json\n- scope: chatter_api\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/first-solar-openid-configuration.json\n- scope: content\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/first-solar-openid-configuration.json\n- scope: custom_permissions\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/first-solar-openid-configuration.json\n- scope: data_cloud_user_claims\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/first-solar-openid-configuration.json\n- scope: eclair_api\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/first-solar-openid-configuration.json\n\
  - scope: einstein_gpt_api\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/first-solar-openid-configuration.json\n- scope: email\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/first-solar-openid-configuration.json\n- scope: forgot_password\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/first-solar-openid-configuration.json\n- scope: full\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/first-solar-openid-configuration.json\n- scope: id\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/first-solar-openid-configuration.json\n- scope: interaction_api\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/first-solar-openid-configuration.json\n- scope: lightning\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/first-solar-openid-configuration.json\n- scope: mcp_api\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/first-solar-openid-configuration.json\n- scope: offline_access\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - well-known/first-solar-openid-configuration.json\n- scope: openid\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/first-solar-openid-configuration.json\n- scope: pardot_api\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/first-solar-openid-configuration.json\n- scope: phone\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/first-solar-openid-configuration.json\n- scope: profile\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/first-solar-openid-configuration.json\n- scope: pwdless_login_api\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/first-solar-openid-configuration.json\n- scope: refresh_token\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/first-solar-openid-configuration.json\n- scope: scrt_api\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/first-solar-openid-configuration.json\n- scope: sfap_api\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/first-solar-openid-configuration.json\n\
  - scope: user_registration_api\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/first-solar-openid-configuration.json\n- scope: visualforce\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/first-solar-openid-configuration.json\n- scope: wave_api\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/first-solar-openid-configuration.json\n- scope: web\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/first-solar-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/first-solar/refs/heads/main/scopes/first-solar-scopes.yml
summary_line: 36 scopes · authorizationCode
tags:
- Solar
- Energy
- Renewable Energy
- Manufacturing
- Fortune 1000
- Photovoltaic
- Thin Film
- Utility-Scale Solar
- Clean Energy
token_urls:
- https://portal.firstsolar.com/developer/services/oauth2/token
---
