---
authorization_urls:
- https://my.canadalife.com/services/oauth2/authorize
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Canada Life Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Canada Life publishes 36 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Canada Life API on a user''s behalf.


  Tokens are issued from https://api.canadalife.com/oauth2/v1/generate.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Canada Life
provider_slug: canada-life
schemes:
- flows:
  - authorizationUrl: null
    flow: clientCredentials
    scope_count: 0
    tokenUrl: https://api.canadalife.com/oauth2/v1/generate
  name: canadalife-gateway-oauth2
  note: scopes_supported published as an empty array; no scopes to harvest.
  scopes_supported: []
  source: well-known/canada-life-openid-configuration.json
  surface: https://api.canadalife.com
- flows:
  - authorizationUrl: https://my.canadalife.com/services/oauth2/authorize
    flow: authorizationCode
    scope_count: 36
    tokenUrl: https://my.canadalife.com/services/oauth2/token
  name: canadalife-customer-portal-oidc
  note: Salesforce Experience Cloud platform scope vocabulary served on a Canada Life host.
  source: well-known/canada-life-my-openid-configuration.json
  surface: https://my.canadalife.com
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
- description: Standard OIDC scope. Requests the address claim.
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
- description: Standard OIDC scope. Requests the email and email_verified claims.
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
- description: Standard OIDC scope. Requests a refresh token so the client can obtain new access tokens without the user present.
  flows: []
  scope: offline_access
- description: Standard OpenID Connect scope. Requests an ID token for the authenticated user.
  flows: []
  scope: openid
- description: ''
  flows: []
  scope: pardot_api
- description: Standard OIDC scope. Requests the phone_number and phone_number_verified claims.
  flows: []
  scope: phone
- description: Standard OIDC scope. Requests the default profile claims (name, family_name, given_name, nickname, picture, preferred_username, profile, updated_at, zoneinfo, locale).
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
slug: canada-life-scopes
source_filename: canada-life-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://my.canadalife.com/.well-known/openid-configuration (HTTP 200, fetched 2026-07-25)\ndocs: null\ndocs_note: Canada Life publishes no scopes or permissions reference page. The scope vocabulary\n  below is served by the Salesforce Experience Cloud platform that hosts my.canadalife.com,\n  so the authoritative descriptions live in Salesforce's OAuth scope documentation, not in\n  a Canada Life document. Descriptions are filled in only for the RFC-standard OpenID Connect\n  scopes; platform-specific scopes are left null rather than guessed.\ncaveat: These are NOT Canada Life business scopes. No insurance, policy, claims, benefits\n  or group-retirement scope vocabulary is published anywhere. The partner gateway at api.canadalife.com\n  publishes scopes_supported as an empty array.\nschemes:\n- name: canadalife-gateway-oauth2\n  surface: https://api.canadalife.com\n  source: well-known/canada-life-openid-configuration.json\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.canadalife.com/oauth2/v1/generate\n    authorizationUrl: null\n    scope_count: 0\n  scopes_supported: []\n  note: scopes_supported published as an empty array; no scopes to harvest.\n- name: canadalife-customer-portal-oidc\n  surface: https://my.canadalife.com\n  source: well-known/canada-life-my-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://my.canadalife.com/services/oauth2/authorize\n    tokenUrl: https://my.canadalife.com/services/oauth2/token\n    scope_count: 36\n  note: Salesforce Experience Cloud platform scope vocabulary served on a Canada Life host.\nscope_count: 36\nscopes:\n- scope: address\n  description: Standard OIDC scope. Requests the address claim.\n  origin: oidc-core\n  sources:\n  - well-known/canada-life-my-openid-configuration.json\n- scope: api\n  description: null\n  origin: salesforce-experience-cloud\n  sources:\n  - well-known/canada-life-my-openid-configuration.json\n\
  - scope: cdp_api\n  description: null\n  origin: salesforce-experience-cloud\n  sources:\n  - well-known/canada-life-my-openid-configuration.json\n- scope: cdp_calculated_insight_api\n  description: null\n  origin: salesforce-experience-cloud\n  sources:\n  - well-known/canada-life-my-openid-configuration.json\n- scope: cdp_identityresolution_api\n  description: null\n  origin: salesforce-experience-cloud\n  sources:\n  - well-known/canada-life-my-openid-configuration.json\n- scope: cdp_ingest_api\n  description: null\n  origin: salesforce-experience-cloud\n  sources:\n  - well-known/canada-life-my-openid-configuration.json\n- scope: cdp_profile_api\n  description: null\n  origin: salesforce-experience-cloud\n  sources:\n  - well-known/canada-life-my-openid-configuration.json\n- scope: cdp_query_api\n  description: null\n  origin: salesforce-experience-cloud\n  sources:\n  - well-known/canada-life-my-openid-configuration.json\n- scope: cdp_segment_api\n  description: null\n  origin: salesforce-experience-cloud\n\
  \  sources:\n  - well-known/canada-life-my-openid-configuration.json\n- scope: chatbot_api\n  description: null\n  origin: salesforce-experience-cloud\n  sources:\n  - well-known/canada-life-my-openid-configuration.json\n- scope: chatter_api\n  description: null\n  origin: salesforce-experience-cloud\n  sources:\n  - well-known/canada-life-my-openid-configuration.json\n- scope: content\n  description: null\n  origin: salesforce-experience-cloud\n  sources:\n  - well-known/canada-life-my-openid-configuration.json\n- scope: custom_permissions\n  description: null\n  origin: salesforce-experience-cloud\n  sources:\n  - well-known/canada-life-my-openid-configuration.json\n- scope: data_cloud_user_claims\n  description: null\n  origin: salesforce-experience-cloud\n  sources:\n  - well-known/canada-life-my-openid-configuration.json\n- scope: eclair_api\n  description: null\n  origin: salesforce-experience-cloud\n  sources:\n  - well-known/canada-life-my-openid-configuration.json\n- scope: einstein_gpt_api\n\
  \  description: null\n  origin: salesforce-experience-cloud\n  sources:\n  - well-known/canada-life-my-openid-configuration.json\n- scope: email\n  description: Standard OIDC scope. Requests the email and email_verified claims.\n  origin: oidc-core\n  sources:\n  - well-known/canada-life-my-openid-configuration.json\n- scope: forgot_password\n  description: null\n  origin: salesforce-experience-cloud\n  sources:\n  - well-known/canada-life-my-openid-configuration.json\n- scope: full\n  description: null\n  origin: salesforce-experience-cloud\n  sources:\n  - well-known/canada-life-my-openid-configuration.json\n- scope: id\n  description: null\n  origin: salesforce-experience-cloud\n  sources:\n  - well-known/canada-life-my-openid-configuration.json\n- scope: interaction_api\n  description: null\n  origin: salesforce-experience-cloud\n  sources:\n  - well-known/canada-life-my-openid-configuration.json\n- scope: lightning\n  description: null\n  origin: salesforce-experience-cloud\n  sources:\n\
  \  - well-known/canada-life-my-openid-configuration.json\n- scope: mcp_api\n  description: null\n  origin: salesforce-experience-cloud\n  sources:\n  - well-known/canada-life-my-openid-configuration.json\n- scope: offline_access\n  description: Standard OIDC scope. Requests a refresh token so the client can obtain new\n    access tokens without the user present.\n  origin: oidc-core\n  sources:\n  - well-known/canada-life-my-openid-configuration.json\n- scope: openid\n  description: Standard OpenID Connect scope. Requests an ID token for the authenticated user.\n  origin: oidc-core\n  sources:\n  - well-known/canada-life-my-openid-configuration.json\n- scope: pardot_api\n  description: null\n  origin: salesforce-experience-cloud\n  sources:\n  - well-known/canada-life-my-openid-configuration.json\n- scope: phone\n  description: Standard OIDC scope. Requests the phone_number and phone_number_verified claims.\n  origin: oidc-core\n  sources:\n  - well-known/canada-life-my-openid-configuration.json\n\
  - scope: profile\n  description: Standard OIDC scope. Requests the default profile claims (name, family_name,\n    given_name, nickname, picture, preferred_username, profile, updated_at, zoneinfo, locale).\n  origin: oidc-core\n  sources:\n  - well-known/canada-life-my-openid-configuration.json\n- scope: pwdless_login_api\n  description: null\n  origin: salesforce-experience-cloud\n  sources:\n  - well-known/canada-life-my-openid-configuration.json\n- scope: refresh_token\n  description: null\n  origin: salesforce-experience-cloud\n  sources:\n  - well-known/canada-life-my-openid-configuration.json\n- scope: scrt_api\n  description: null\n  origin: salesforce-experience-cloud\n  sources:\n  - well-known/canada-life-my-openid-configuration.json\n- scope: sfap_api\n  description: null\n  origin: salesforce-experience-cloud\n  sources:\n  - well-known/canada-life-my-openid-configuration.json\n- scope: user_registration_api\n  description: null\n  origin: salesforce-experience-cloud\n  sources:\n\
  \  - well-known/canada-life-my-openid-configuration.json\n- scope: visualforce\n  description: null\n  origin: salesforce-experience-cloud\n  sources:\n  - well-known/canada-life-my-openid-configuration.json\n- scope: wave_api\n  description: null\n  origin: salesforce-experience-cloud\n  sources:\n  - well-known/canada-life-my-openid-configuration.json\n- scope: web\n  description: null\n  origin: salesforce-experience-cloud\n  sources:\n  - well-known/canada-life-my-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canada-life/refs/heads/main/scopes/canada-life-scopes.yml
summary_line: 36 scopes · clientCredentials/authorizationCode
tags:
- Insurance
- Canada
- Life Insurance
- Health Insurance
- Employee Benefits
- Group Retirement
- Carrier
- ACORD
- Partner Gated
- No Public API
token_urls:
- https://api.canadalife.com/oauth2/v1/generate
- https://my.canadalife.com/services/oauth2/token
---
