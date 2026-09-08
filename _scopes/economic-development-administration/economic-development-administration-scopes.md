---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Economic Development Administration Scopes
name_suffix: OAuth Scopes
note: 'scopes_supported read verbatim from the OpenID Provider metadata served at https://sfgrants.eda.gov/.well-known/openid-configuration (HTTP 200, 2026-09-06). This is the Salesforce Experience Cloud platform scope vocabulary exposed by EDA''s grants-portal tenant under EDA''s own domain — it is NOT an EDA-authored scope taxonomy, and EDA publishes no scopes/permissions reference page. Descriptions below are the platform meanings of each scope, not EDA prose. Which of these scopes EDA actually grants to a portal client cannot be determined anonymously: every data endpoint behind the issuer returned 401.'
overview: 'Economic Development Administration publishes 36 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Economic Development Administration API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Economic Development Administration
provider_slug: economic-development-administration
schemes: []
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
- description: Standard OIDC address claim.
  flows: []
  scope: address
- description: Access the Salesforce REST/SOAP data APIs for the EDA grants org.
  flows: []
  scope: api
- description: Access Data Cloud (CDP) APIs.
  flows: []
  scope: cdp_api
- description: Read Data Cloud calculated insights.
  flows: []
  scope: cdp_calculated_insight_api
- description: Run Data Cloud identity resolution.
  flows: []
  scope: cdp_identityresolution_api
- description: Ingest records into Data Cloud.
  flows: []
  scope: cdp_ingest_api
- description: Read unified Data Cloud profiles.
  flows: []
  scope: cdp_profile_api
- description: Query Data Cloud objects.
  flows: []
  scope: cdp_query_api
- description: Manage Data Cloud segments.
  flows: []
  scope: cdp_segment_api
- description: Access Einstein Bots APIs.
  flows: []
  scope: chatbot_api
- description: Access the Connect (Chatter) REST API.
  flows: []
  scope: chatter_api
- description: Access Salesforce CMS / managed content APIs.
  flows: []
  scope: content
- description: Return the custom permissions granted to the user.
  flows: []
  scope: custom_permissions
- description: Return Data Cloud user claims in the token.
  flows: []
  scope: data_cloud_user_claims
- description: Access CRM Analytics chart/Eclair APIs.
  flows: []
  scope: eclair_api
- description: Access Einstein Generative AI APIs.
  flows: []
  scope: einstein_gpt_api
- description: Standard OIDC email and email_verified claims.
  flows: []
  scope: email
- description: Forgot-password API for Experience Cloud users.
  flows: []
  scope: forgot_password
- description: Full access to all data the authenticated portal user can reach.
  flows: []
  scope: full
- description: Salesforce identity URL access (user id, organization id, urls).
  flows: []
  scope: id
- description: Access the Interaction (Salesforce Interactions) API.
  flows: []
  scope: interaction_api
- description: Access Lightning Experience / Lightning component endpoints.
  flows: []
  scope: lightning
- description: Access the Salesforce platform Model Context Protocol API surface.
  flows: []
  scope: mcp_api
- description: Synonym of refresh_token — offline access to the portal API.
  flows: []
  scope: offline_access
- description: Issue an OpenID Connect ID token for the authenticated portal user.
  flows: []
  scope: openid
- description: Access Account Engagement (Pardot) APIs.
  flows: []
  scope: pardot_api
- description: Standard OIDC phone_number and phone_number_verified claims.
  flows: []
  scope: phone
- description: Standard OIDC profile claims (name, preferred_username, picture, zoneinfo).
  flows: []
  scope: profile
- description: Passwordless login API for Experience Cloud users.
  flows: []
  scope: pwdless_login_api
- description: Issue a refresh token for long-lived access.
  flows: []
  scope: refresh_token
- description: Access Service Cloud Real-Time (Messaging) APIs.
  flows: []
  scope: scrt_api
- description: Access Salesforce Agentforce Platform APIs.
  flows: []
  scope: sfap_api
- description: Self-registration API for Experience Cloud users.
  flows: []
  scope: user_registration_api
- description: Access Visualforce pages in the org.
  flows: []
  scope: visualforce
- description: Access CRM Analytics (Wave) APIs.
  flows: []
  scope: wave_api
- description: Access the portal web session (Experience Cloud).
  flows: []
  scope: web
slug: economic-development-administration-scopes
source_filename: economic-development-administration-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: https://sfgrants.eda.gov/.well-known/openid-configuration\nnote: 'scopes_supported read verbatim from the OpenID Provider metadata served at https://sfgrants.eda.gov/.well-known/openid-configuration\n  (HTTP 200, 2026-09-06). This is the Salesforce Experience Cloud platform scope vocabulary exposed by\n  EDA''s grants-portal tenant under EDA''s own domain — it is NOT an EDA-authored scope taxonomy, and\n  EDA publishes no scopes/permissions reference page. Descriptions below are the platform meanings of\n  each scope, not EDA prose. Which of these scopes EDA actually grants to a portal client cannot be determined\n  anonymously: every data endpoint behind the issuer returned 401.'\nissuer: https://sfgrants.eda.gov\nflows:\n  authorization_code: https://sfgrants.eda.gov/services/oauth2/authorize\ndocs: null\nscope_count: 36\nscopes:\n- scope: address\n  description: Standard OIDC address claim.\n- scope: api\n  description: Access\
  \ the Salesforce REST/SOAP data APIs for the EDA grants org.\n- scope: cdp_api\n  description: Access Data Cloud (CDP) APIs.\n- scope: cdp_calculated_insight_api\n  description: Read Data Cloud calculated insights.\n- scope: cdp_identityresolution_api\n  description: Run Data Cloud identity resolution.\n- scope: cdp_ingest_api\n  description: Ingest records into Data Cloud.\n- scope: cdp_profile_api\n  description: Read unified Data Cloud profiles.\n- scope: cdp_query_api\n  description: Query Data Cloud objects.\n- scope: cdp_segment_api\n  description: Manage Data Cloud segments.\n- scope: chatbot_api\n  description: Access Einstein Bots APIs.\n- scope: chatter_api\n  description: Access the Connect (Chatter) REST API.\n- scope: content\n  description: Access Salesforce CMS / managed content APIs.\n- scope: custom_permissions\n  description: Return the custom permissions granted to the user.\n- scope: data_cloud_user_claims\n  description: Return Data Cloud user claims in the token.\n\
  - scope: eclair_api\n  description: Access CRM Analytics chart/Eclair APIs.\n- scope: einstein_gpt_api\n  description: Access Einstein Generative AI APIs.\n- scope: email\n  description: Standard OIDC email and email_verified claims.\n- scope: forgot_password\n  description: Forgot-password API for Experience Cloud users.\n- scope: full\n  description: Full access to all data the authenticated portal user can reach.\n- scope: id\n  description: Salesforce identity URL access (user id, organization id, urls).\n- scope: interaction_api\n  description: Access the Interaction (Salesforce Interactions) API.\n- scope: lightning\n  description: Access Lightning Experience / Lightning component endpoints.\n- scope: mcp_api\n  description: Access the Salesforce platform Model Context Protocol API surface.\n- scope: offline_access\n  description: Synonym of refresh_token — offline access to the portal API.\n- scope: openid\n  description: Issue an OpenID Connect ID token for the authenticated portal\
  \ user.\n- scope: pardot_api\n  description: Access Account Engagement (Pardot) APIs.\n- scope: phone\n  description: Standard OIDC phone_number and phone_number_verified claims.\n- scope: profile\n  description: Standard OIDC profile claims (name, preferred_username, picture, zoneinfo).\n- scope: pwdless_login_api\n  description: Passwordless login API for Experience Cloud users.\n- scope: refresh_token\n  description: Issue a refresh token for long-lived access.\n- scope: scrt_api\n  description: Access Service Cloud Real-Time (Messaging) APIs.\n- scope: sfap_api\n  description: Access Salesforce Agentforce Platform APIs.\n- scope: user_registration_api\n  description: Self-registration API for Experience Cloud users.\n- scope: visualforce\n  description: Access Visualforce pages in the org.\n- scope: wave_api\n  description: Access CRM Analytics (Wave) APIs.\n- scope: web\n  description: Access the portal web session (Experience Cloud).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/economic-development-administration/refs/heads/main/scopes/economic-development-administration-scopes.yml
summary_line: 36 scopes
tags:
- Economic Development
- Federal-Government
- Grants
- Public Sector
- Regional Development
- Economic Data
token_urls: []
---
