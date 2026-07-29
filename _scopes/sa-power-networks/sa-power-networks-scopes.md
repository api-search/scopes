---
authorization_urls:
- https://customer.portal.sapowernetworks.com.au/meterdata/services/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Sa Power Networks Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'SA Power Networks publishes 36 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the SA Power Networks API on a user''s behalf.


  Tokens are issued from https://customer.portal.sapowernetworks.com.au/meterdata/services/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SA Power Networks
provider_slug: sa-power-networks
schemes:
- flows:
  - authorizationUrl: https://customer.portal.sapowernetworks.com.au/meterdata/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://customer.portal.sapowernetworks.com.au/meterdata/services/oauth2/token
  issuer: https://customer.portal.sapowernetworks.com.au/meterdata
  name: meterdata-oidc
  source: well-known/sa-power-networks-meterdata-openid-configuration.json
  type: openIdConnect
scope_count: 36
scope_names:
- openid
- profile
- email
- address
- phone
- id
- api
- web
- full
- refresh_token
- offline_access
- custom_permissions
- lightning
- visualforce
- content
- chatter_api
- chatbot_api
- eclair_api
- wave_api
- interaction_api
- pardot_api
- scrt_api
- sfap_api
- einstein_gpt_api
- mcp_api
- user_registration_api
- pwdless_login_api
- forgot_password
- cdp_api
- cdp_query_api
- cdp_profile_api
- cdp_ingest_api
- cdp_segment_api
- cdp_identityresolution_api
- cdp_calculated_insight_api
- data_cloud_user_claims
scopes:
- description: OpenID Connect authentication; returns an ID token.
  flows: []
  scope: openid
- description: Basic profile claims for the authenticated user.
  flows: []
  scope: profile
- description: Email address claim.
  flows: []
  scope: email
- description: Address claims.
  flows: []
  scope: address
- description: Phone number claims.
  flows: []
  scope: phone
- description: Identity URL access.
  flows: []
  scope: id
- description: Salesforce REST/SOAP API access on behalf of the user.
  flows: []
  scope: api
- description: Web session access to the org.
  flows: []
  scope: web
- description: Full access to all data the user can access.
  flows: []
  scope: full
- description: Issue a refresh token.
  flows: []
  scope: refresh_token
- description: Offline access (refresh token alias).
  flows: []
  scope: offline_access
- description: Returns the custom permissions granted to the user.
  flows: []
  scope: custom_permissions
- description: Lightning Experience access.
  flows: []
  scope: lightning
- description: Visualforce page access.
  flows: []
  scope: visualforce
- description: Salesforce CMS / content access.
  flows: []
  scope: content
- description: Connect (Chatter) REST API access.
  flows: []
  scope: chatter_api
- description: Einstein Bots API access.
  flows: []
  scope: chatbot_api
- description: Einstein analytics (Eclair) API access.
  flows: []
  scope: eclair_api
- description: CRM Analytics (Wave) API access.
  flows: []
  scope: wave_api
- description: Interaction Studio / personalization API access.
  flows: []
  scope: interaction_api
- description: Account Engagement (Pardot) API access.
  flows: []
  scope: pardot_api
- description: Service Cloud real-time (SCRT) messaging API access.
  flows: []
  scope: scrt_api
- description: Salesforce platform agent API access.
  flows: []
  scope: sfap_api
- description: Einstein GPT API access.
  flows: []
  scope: einstein_gpt_api
- description: Salesforce Model Context Protocol API access (platform-provided).
  flows: []
  scope: mcp_api
- description: Self-registration API access.
  flows: []
  scope: user_registration_api
- description: Passwordless login API access.
  flows: []
  scope: pwdless_login_api
- description: Forgot-password flow API access.
  flows: []
  scope: forgot_password
- description: Data Cloud (CDP) API access.
  flows: []
  scope: cdp_api
- description: Data Cloud query API access.
  flows: []
  scope: cdp_query_api
- description: Data Cloud profile API access.
  flows: []
  scope: cdp_profile_api
- description: Data Cloud ingestion API access.
  flows: []
  scope: cdp_ingest_api
- description: Data Cloud segmentation API access.
  flows: []
  scope: cdp_segment_api
- description: Data Cloud identity resolution API access.
  flows: []
  scope: cdp_identityresolution_api
- description: Data Cloud calculated insights API access.
  flows: []
  scope: cdp_calculated_insight_api
- description: Data Cloud user claims.
  flows: []
  scope: data_cloud_user_claims
slug: sa-power-networks-scopes
source_filename: sa-power-networks-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: https://customer.portal.sapowernetworks.com.au/meterdata/.well-known/openid-configuration\nfile: well-known/sa-power-networks-meterdata-openid-configuration.json\ndocs: null\ncaveat: >-\n  These are the scopes advertised by the Salesforce Experience Cloud identity\n  provider that fronts the \"Your Meter Data\" portal — the stock Salesforce platform\n  scope set, published by the vendor platform rather than designed by SA Power\n  Networks. SA Power Networks documents no scope model of its own, publishes no\n  scope reference page, and exposes no API for these scopes to authorize. They are\n  recorded because they are genuinely published and anonymously retrievable, not\n  because they represent an SA Power Networks authorization contract.\nschemes:\n- name: meterdata-oidc\n  type: openIdConnect\n  issuer: https://customer.portal.sapowernetworks.com.au/meterdata\n  source: well-known/sa-power-networks-meterdata-openid-configuration.json\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://customer.portal.sapowernetworks.com.au/meterdata/services/oauth2/authorize\n    tokenUrl: https://customer.portal.sapowernetworks.com.au/meterdata/services/oauth2/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; returns an ID token.\n  origin: salesforce-platform\n- scope: profile\n  description: Basic profile claims for the authenticated user.\n  origin: salesforce-platform\n- scope: email\n  description: Email address claim.\n  origin: salesforce-platform\n- scope: address\n  description: Address claims.\n  origin: salesforce-platform\n- scope: phone\n  description: Phone number claims.\n  origin: salesforce-platform\n- scope: id\n  description: Identity URL access.\n  origin: salesforce-platform\n- scope: api\n  description: Salesforce REST/SOAP API access on behalf of the user.\n  origin: salesforce-platform\n- scope: web\n  description: Web session access to the org.\n  origin: salesforce-platform\n\
  - scope: full\n  description: Full access to all data the user can access.\n  origin: salesforce-platform\n- scope: refresh_token\n  description: Issue a refresh token.\n  origin: salesforce-platform\n- scope: offline_access\n  description: Offline access (refresh token alias).\n  origin: salesforce-platform\n- scope: custom_permissions\n  description: Returns the custom permissions granted to the user.\n  origin: salesforce-platform\n- scope: lightning\n  description: Lightning Experience access.\n  origin: salesforce-platform\n- scope: visualforce\n  description: Visualforce page access.\n  origin: salesforce-platform\n- scope: content\n  description: Salesforce CMS / content access.\n  origin: salesforce-platform\n- scope: chatter_api\n  description: Connect (Chatter) REST API access.\n  origin: salesforce-platform\n- scope: chatbot_api\n  description: Einstein Bots API access.\n  origin: salesforce-platform\n- scope: eclair_api\n  description: Einstein analytics (Eclair) API access.\n\
  \  origin: salesforce-platform\n- scope: wave_api\n  description: CRM Analytics (Wave) API access.\n  origin: salesforce-platform\n- scope: interaction_api\n  description: Interaction Studio / personalization API access.\n  origin: salesforce-platform\n- scope: pardot_api\n  description: Account Engagement (Pardot) API access.\n  origin: salesforce-platform\n- scope: scrt_api\n  description: Service Cloud real-time (SCRT) messaging API access.\n  origin: salesforce-platform\n- scope: sfap_api\n  description: Salesforce platform agent API access.\n  origin: salesforce-platform\n- scope: einstein_gpt_api\n  description: Einstein GPT API access.\n  origin: salesforce-platform\n- scope: mcp_api\n  description: Salesforce Model Context Protocol API access (platform-provided).\n  origin: salesforce-platform\n- scope: user_registration_api\n  description: Self-registration API access.\n  origin: salesforce-platform\n- scope: pwdless_login_api\n  description: Passwordless login API access.\n \
  \ origin: salesforce-platform\n- scope: forgot_password\n  description: Forgot-password flow API access.\n  origin: salesforce-platform\n- scope: cdp_api\n  description: Data Cloud (CDP) API access.\n  origin: salesforce-platform\n- scope: cdp_query_api\n  description: Data Cloud query API access.\n  origin: salesforce-platform\n- scope: cdp_profile_api\n  description: Data Cloud profile API access.\n  origin: salesforce-platform\n- scope: cdp_ingest_api\n  description: Data Cloud ingestion API access.\n  origin: salesforce-platform\n- scope: cdp_segment_api\n  description: Data Cloud segmentation API access.\n  origin: salesforce-platform\n- scope: cdp_identityresolution_api\n  description: Data Cloud identity resolution API access.\n  origin: salesforce-platform\n- scope: cdp_calculated_insight_api\n  description: Data Cloud calculated insights API access.\n  origin: salesforce-platform\n- scope: data_cloud_user_claims\n  description: Data Cloud user claims.\n  origin: salesforce-platform\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sa-power-networks/refs/heads/main/scopes/sa-power-networks-scopes.yml
summary_line: 36 scopes · authorizationCode
tags:
- Energy
- Australia
- Utilities
- Electricity
- Grid
- Distribution Network
- Smart Metering
- Solar
- DER
- Open Data
token_urls:
- https://customer.portal.sapowernetworks.com.au/meterdata/services/oauth2/token
---
