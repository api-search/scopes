---
authorization_urls:
- https://community.envisagenow.com/cares/services/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Envisagenow Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Envisagenow publishes 36 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Envisagenow API on a user''s behalf.


  Tokens are issued from https://community.envisagenow.com/cares/services/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Envisagenow
provider_slug: envisagenow
schemes:
- flows:
  - authorizationUrl: https://community.envisagenow.com/cares/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://community.envisagenow.com/cares/services/oauth2/token
  name: oauth2
  source: well-known/envisagenow-openid-configuration.json
scope_count: 36
scope_names:
- openid
- profile
- email
- address
- phone
- api
- web
- full
- id
- refresh_token
- offline_access
- lightning
- visualforce
- content
- chatter_api
- custom_permissions
- wave_api
- eclair_api
- pardot_api
- interaction_api
- chatbot_api
- einstein_gpt_api
- sfap_api
- mcp_api
- cdp_api
- cdp_query_api
- cdp_ingest_api
- cdp_profile_api
- cdp_segment_api
- cdp_identityresolution_api
- cdp_calculated_insight_api
- data_cloud_user_claims
- scrt_api
- user_registration_api
- pwdless_login_api
- forgot_password
scopes:
- description: OpenID Connect authentication (issue an ID token)
  flows: []
  scope: openid
- description: Basic profile claims
  flows: []
  scope: profile
- description: Email address claim
  flows: []
  scope: email
- description: Address claim
  flows: []
  scope: address
- description: Phone number claim
  flows: []
  scope: phone
- description: Access the Salesforce REST/SOAP APIs on behalf of the user
  flows: []
  scope: api
- description: Web access
  flows: []
  scope: web
- description: Full access to all data accessible to the user
  flows: []
  scope: full
- description: Access the identity URL service
  flows: []
  scope: id
- description: Obtain a refresh token
  flows: []
  scope: refresh_token
- description: Long-lived offline access
  flows: []
  scope: offline_access
- description: Access Lightning Experience
  flows: []
  scope: lightning
- description: Access Visualforce pages
  flows: []
  scope: visualforce
- description: Access Salesforce CRM Content
  flows: []
  scope: content
- description: Access Chatter REST API
  flows: []
  scope: chatter_api
- description: See the user's custom permissions
  flows: []
  scope: custom_permissions
- description: Access CRM Analytics (Wave) REST API
  flows: []
  scope: wave_api
- description: Access CRM Analytics charting (Eclair) API
  flows: []
  scope: eclair_api
- description: Access Account Engagement (Pardot) API
  flows: []
  scope: pardot_api
- description: Access Interaction / Marketing Cloud API
  flows: []
  scope: interaction_api
- description: Access Einstein Bots (chatbot) API
  flows: []
  scope: chatbot_api
- description: Access Einstein GPT API
  flows: []
  scope: einstein_gpt_api
- description: Access Salesforce AI Platform API
  flows: []
  scope: sfap_api
- description: Access the Salesforce MCP (Model Context Protocol) API
  flows: []
  scope: mcp_api
- description: Access Data Cloud (CDP) API
  flows: []
  scope: cdp_api
- description: Query Data Cloud (CDP)
  flows: []
  scope: cdp_query_api
- description: Ingest data into Data Cloud (CDP)
  flows: []
  scope: cdp_ingest_api
- description: Access Data Cloud unified profiles
  flows: []
  scope: cdp_profile_api
- description: Manage Data Cloud segments
  flows: []
  scope: cdp_segment_api
- description: Data Cloud identity resolution
  flows: []
  scope: cdp_identityresolution_api
- description: Data Cloud calculated insights
  flows: []
  scope: cdp_calculated_insight_api
- description: Data Cloud user claims
  flows: []
  scope: data_cloud_user_claims
- description: Access Salesforce real-time (SCRT) API
  flows: []
  scope: scrt_api
- description: Self-registration API
  flows: []
  scope: user_registration_api
- description: Passwordless login API
  flows: []
  scope: pwdless_login_api
- description: Forgot-password flow
  flows: []
  scope: forgot_password
slug: envisagenow-scopes
source_filename: envisagenow-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://community.envisagenow.com/.well-known/openid-configuration\nnotes: >-\n  Scopes read verbatim from the Acadis Readiness Community OIDC discovery\n  document (Salesforce Experience Cloud identity provider). These are the\n  scopes_supported the community IdP advertises; they are the standard\n  Salesforce platform OAuth scope set exposed for this Experience Cloud site,\n  not a bespoke Envisage/Acadis API scope catalog (Envisage publishes no public\n  developer API).\nschemes:\n- name: oauth2\n  source: well-known/envisagenow-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://community.envisagenow.com/cares/services/oauth2/authorize\n    tokenUrl: https://community.envisagenow.com/cares/services/oauth2/token\nscopes:\n- {scope: openid, description: OpenID Connect authentication (issue an ID token)}\n- {scope: profile, description: Basic profile claims}\n- {scope: email, description:\
  \ Email address claim}\n- {scope: address, description: Address claim}\n- {scope: phone, description: Phone number claim}\n- {scope: api, description: Access the Salesforce REST/SOAP APIs on behalf of the user}\n- {scope: web, description: Web access}\n- {scope: full, description: Full access to all data accessible to the user}\n- {scope: id, description: Access the identity URL service}\n- {scope: refresh_token, description: Obtain a refresh token}\n- {scope: offline_access, description: Long-lived offline access}\n- {scope: lightning, description: Access Lightning Experience}\n- {scope: visualforce, description: Access Visualforce pages}\n- {scope: content, description: Access Salesforce CRM Content}\n- {scope: chatter_api, description: Access Chatter REST API}\n- {scope: custom_permissions, description: See the user's custom permissions}\n- {scope: wave_api, description: Access CRM Analytics (Wave) REST API}\n- {scope: eclair_api, description: Access CRM Analytics charting (Eclair)\
  \ API}\n- {scope: pardot_api, description: Access Account Engagement (Pardot) API}\n- {scope: interaction_api, description: Access Interaction / Marketing Cloud API}\n- {scope: chatbot_api, description: Access Einstein Bots (chatbot) API}\n- {scope: einstein_gpt_api, description: Access Einstein GPT API}\n- {scope: sfap_api, description: Access Salesforce AI Platform API}\n- {scope: mcp_api, description: Access the Salesforce MCP (Model Context Protocol) API}\n- {scope: cdp_api, description: Access Data Cloud (CDP) API}\n- {scope: cdp_query_api, description: Query Data Cloud (CDP)}\n- {scope: cdp_ingest_api, description: Ingest data into Data Cloud (CDP)}\n- {scope: cdp_profile_api, description: Access Data Cloud unified profiles}\n- {scope: cdp_segment_api, description: Manage Data Cloud segments}\n- {scope: cdp_identityresolution_api, description: Data Cloud identity resolution}\n- {scope: cdp_calculated_insight_api, description: Data Cloud calculated insights}\n- {scope: data_cloud_user_claims,\
  \ description: Data Cloud user claims}\n- {scope: scrt_api, description: Access Salesforce real-time (SCRT) API}\n- {scope: user_registration_api, description: Self-registration API}\n- {scope: pwdless_login_api, description: Passwordless login API}\n- {scope: forgot_password, description: Forgot-password flow}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/envisagenow/refs/heads/main/scopes/envisagenow-scopes.yml
summary_line: 36 scopes · authorizationCode
tags:
- Company
- Public Safety
- Training
- Compliance
- Performance Management
- Law Enforcement
- First Responders
- Government
- SaaS
token_urls:
- https://community.envisagenow.com/cares/services/oauth2/token
---
