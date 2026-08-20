---
authorization_urls:
- https://developer.bankunited.com/aeh/services/oauth2/authorize
description: ''
docs: https://developer.bankunited.com/s/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Bankunited Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'BankUnited publishes 36 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the BankUnited API on a user''s behalf.


  Tokens are issued from https://developer.bankunited.com/aeh/services/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: BankUnited
provider_slug: bankunited
schemes:
- flows:
  - authorizationUrl: https://developer.bankunited.com/aeh/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://developer.bankunited.com/aeh/services/oauth2/token
  name: OAuth2
  source: well-known/bankunited-openid-configuration.json
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
- lightning
- visualforce
- content
- chatter_api
- wave_api
- eclair_api
- pardot_api
- einstein_gpt_api
- sfap_api
- mcp_api
- interaction_api
- scrt_api
- chatbot_api
- user_registration_api
- pwdless_login_api
- forgot_password
- custom_permissions
- cdp_api
- cdp_query_api
- cdp_ingest_api
- cdp_profile_api
- cdp_segment_api
- cdp_identityresolution_api
- cdp_calculated_insight_api
- data_cloud_user_claims
scopes:
- description: OpenID Connect authentication
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
- description: Salesforce identity URL access
  flows: []
  scope: id
- description: Access the platform REST/SOAP APIs
  flows: []
  scope: api
- description: Web browser access to the connected app
  flows: []
  scope: web
- description: Full access (all other scopes except refresh_token)
  flows: []
  scope: full
- description: Issue a refresh token
  flows: []
  scope: refresh_token
- description: Offline access (refresh token)
  flows: []
  scope: offline_access
- description: Lightning Experience access
  flows: []
  scope: lightning
- description: Visualforce page access
  flows: []
  scope: visualforce
- description: Salesforce CRM content access
  flows: []
  scope: content
- description: Chatter REST API access
  flows: []
  scope: chatter_api
- description: CRM Analytics (Wave) API access
  flows: []
  scope: wave_api
- description: CRM Analytics charting API access
  flows: []
  scope: eclair_api
- description: Pardot / Account Engagement API access
  flows: []
  scope: pardot_api
- description: Einstein GPT / generative AI API access
  flows: []
  scope: einstein_gpt_api
- description: Salesforce AI platform API access
  flows: []
  scope: sfap_api
- description: Model Context Protocol API access (Salesforce platform)
  flows: []
  scope: mcp_api
- description: Interaction Studio API access
  flows: []
  scope: interaction_api
- description: Service cloud real-time API access
  flows: []
  scope: scrt_api
- description: Einstein Bots API access
  flows: []
  scope: chatbot_api
- description: Self-registration API access
  flows: []
  scope: user_registration_api
- description: Passwordless login API access
  flows: []
  scope: pwdless_login_api
- description: Forgot-password flow access
  flows: []
  scope: forgot_password
- description: Include custom permissions in the token
  flows: []
  scope: custom_permissions
- description: Data Cloud (CDP) API access
  flows: []
  scope: cdp_api
- description: Data Cloud query API access
  flows: []
  scope: cdp_query_api
- description: Data Cloud ingestion API access
  flows: []
  scope: cdp_ingest_api
- description: Data Cloud profile API access
  flows: []
  scope: cdp_profile_api
- description: Data Cloud segmentation API access
  flows: []
  scope: cdp_segment_api
- description: Data Cloud identity resolution API access
  flows: []
  scope: cdp_identityresolution_api
- description: Data Cloud calculated insights API access
  flows: []
  scope: cdp_calculated_insight_api
- description: Data Cloud user claims
  flows: []
  scope: data_cloud_user_claims
slug: bankunited-scopes
source_filename: bankunited-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://developer.bankunited.com/aeh/.well-known/openid-configuration\ndocs: https://developer.bankunited.com/s/\nnotes: >-\n  These scopes are the scopes_supported list advertised by the BankUnited API\n  Experience Hub OIDC discovery document. Because the portal runs on Salesforce\n  Experience Cloud, this list is the standard Salesforce OAuth 2.0 connected-app\n  scope catalog (openid/profile/email/api/refresh_token plus Salesforce platform\n  scopes such as cdp_*, wave_api, pardot_api, einstein_gpt_api, mcp_api) rather\n  than BankUnited-specific banking-product scopes. The product-level API\n  authorization scopes for BankUnited's own API contracts are defined per API and\n  sit behind portal registration/login. Captured verbatim, honestly flagged as\n  platform scopes.\nschemes:\n- name: OAuth2\n  source: well-known/bankunited-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://developer.bankunited.com/aeh/services/oauth2/authorize\n\
  \    tokenUrl: https://developer.bankunited.com/aeh/services/oauth2/token\nscopes:\n- {scope: openid, description: OpenID Connect authentication, category: identity}\n- {scope: profile, description: Basic profile claims, category: identity}\n- {scope: email, description: Email address claim, category: identity}\n- {scope: address, description: Address claim, category: identity}\n- {scope: phone, description: Phone number claim, category: identity}\n- {scope: id, description: Salesforce identity URL access, category: identity}\n- {scope: api, description: Access the platform REST/SOAP APIs, category: platform}\n- {scope: web, description: Web browser access to the connected app, category: platform}\n- {scope: full, description: Full access (all other scopes except refresh_token), category: platform}\n- {scope: refresh_token, description: Issue a refresh token, category: token}\n- {scope: offline_access, description: Offline access (refresh token), category: token}\n- {scope: lightning,\
  \ description: Lightning Experience access, category: platform}\n- {scope: visualforce, description: Visualforce page access, category: platform}\n- {scope: content, description: Salesforce CRM content access, category: platform}\n- {scope: chatter_api, description: Chatter REST API access, category: platform}\n- {scope: wave_api, description: CRM Analytics (Wave) API access, category: platform}\n- {scope: eclair_api, description: CRM Analytics charting API access, category: platform}\n- {scope: pardot_api, description: Pardot / Account Engagement API access, category: platform}\n- {scope: einstein_gpt_api, description: Einstein GPT / generative AI API access, category: ai}\n- {scope: sfap_api, description: Salesforce AI platform API access, category: ai}\n- {scope: mcp_api, description: Model Context Protocol API access (Salesforce platform), category: ai}\n- {scope: interaction_api, description: Interaction Studio API access, category: platform}\n- {scope: scrt_api, description: Service\
  \ cloud real-time API access, category: platform}\n- {scope: chatbot_api, description: Einstein Bots API access, category: platform}\n- {scope: user_registration_api, description: Self-registration API access, category: platform}\n- {scope: pwdless_login_api, description: Passwordless login API access, category: platform}\n- {scope: forgot_password, description: Forgot-password flow access, category: platform}\n- {scope: custom_permissions, description: Include custom permissions in the token, category: platform}\n- {scope: cdp_api, description: Data Cloud (CDP) API access, category: data-cloud}\n- {scope: cdp_query_api, description: Data Cloud query API access, category: data-cloud}\n- {scope: cdp_ingest_api, description: Data Cloud ingestion API access, category: data-cloud}\n- {scope: cdp_profile_api, description: Data Cloud profile API access, category: data-cloud}\n- {scope: cdp_segment_api, description: Data Cloud segmentation API access, category: data-cloud}\n- {scope: cdp_identityresolution_api,\
  \ description: Data Cloud identity resolution API access, category: data-cloud}\n- {scope: cdp_calculated_insight_api, description: Data Cloud calculated insights API access, category: data-cloud}\n- {scope: data_cloud_user_claims, description: Data Cloud user claims, category: data-cloud}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bankunited/refs/heads/main/scopes/bankunited-scopes.yml
summary_line: 36 scopes · authorizationCode
tags:
- Financial-Services
- Banking
- United States
- Regional Bank
- Commercial Banking
- Open Finance
- Developer Portal
token_urls:
- https://developer.bankunited.com/aeh/services/oauth2/token
---
