---
authorization_urls:
- https://supportportal.hammerspace.com/services/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
- implicit
kind: oauth-scopes
layout: scope
method: probed
name: Hammerspace Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Hammerspace publishes 36 OAuth 2.0 scopes via the authorizationCode and implicit flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Hammerspace API on a user''s behalf.


  Tokens are issued from https://supportportal.hammerspace.com/services/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hammerspace
provider_slug: hammerspace
schemes:
- flows:
  - authorizationUrl: https://supportportal.hammerspace.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://supportportal.hammerspace.com/services/oauth2/token
  - authorizationUrl: https://supportportal.hammerspace.com/services/oauth2/authorize
    flow: implicit
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://supportportal.hammerspace.com
  name: supportportal-oidc
  platform: Salesforce Experience Cloud
  response_types_supported:
  - code
  - token
  - token id_token
  source: well-known/hammerspace-openid-configuration.json
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
scope_count: 36
scope_names:
- openid
- profile
- email
- address
- phone
- offline_access
- refresh_token
- id
- api
- full
- web
- lightning
- visualforce
- content
- chatter_api
- chatbot_api
- custom_permissions
- forgot_password
- pwdless_login_api
- user_registration_api
- interaction_api
- wave_api
- eclair_api
- einstein_gpt_api
- sfap_api
- mcp_api
- scrt_api
- pardot_api
- cdp_api
- cdp_query_api
- cdp_ingest_api
- cdp_profile_api
- cdp_segment_api
- cdp_identityresolution_api
- cdp_calculated_insight_api
- data_cloud_user_claims
scopes:
- description: OIDC — request an ID token.
  flows: []
  scope: openid
- description: OIDC — basic profile claims.
  flows: []
  scope: profile
- description: OIDC — email and email_verified claims.
  flows: []
  scope: email
- description: OIDC — address claim.
  flows: []
  scope: address
- description: OIDC — phone_number and phone_number_verified claims.
  flows: []
  scope: phone
- description: OIDC — issue a refresh token.
  flows: []
  scope: offline_access
- description: Salesforce alias for offline_access.
  flows: []
  scope: refresh_token
- description: Salesforce — access the identity URL service.
  flows: []
  scope: id
- description: Salesforce — access the platform REST/SOAP APIs on the user's behalf.
  flows: []
  scope: api
- description: Salesforce — full access to all data accessible to the user.
  flows: []
  scope: full
- description: Salesforce — access web pages via a browser session.
  flows: []
  scope: web
- description: Salesforce — access Lightning applications.
  flows: []
  scope: lightning
- description: Salesforce — access Visualforce pages.
  flows: []
  scope: visualforce
- description: Salesforce — access Files/Content resources.
  flows: []
  scope: content
- description: Salesforce — Connect REST (Chatter) API access.
  flows: []
  scope: chatter_api
- description: Salesforce — Einstein Bots API access.
  flows: []
  scope: chatbot_api
- description: Salesforce — return the user's custom permissions.
  flows: []
  scope: custom_permissions
- description: Salesforce — headless password-reset flow.
  flows: []
  scope: forgot_password
- description: Salesforce — headless passwordless login flow.
  flows: []
  scope: pwdless_login_api
- description: Salesforce — headless self-registration flow.
  flows: []
  scope: user_registration_api
- description: Salesforce — Interaction (Flow) API access.
  flows: []
  scope: interaction_api
- description: Salesforce — CRM Analytics (Wave) API access.
  flows: []
  scope: wave_api
- description: Salesforce — Einstein Vision/Language (Eclair) API access.
  flows: []
  scope: eclair_api
- description: Salesforce — Einstein GPT / models API access.
  flows: []
  scope: einstein_gpt_api
- description: Salesforce — Agentforce platform API access.
  flows: []
  scope: sfap_api
- description: Salesforce — Model Context Protocol API access on the Experience Cloud identity provider. This is a Salesforce platform scope, not a scope on Hammerspace's own MCP server.
  flows: []
  scope: mcp_api
- description: Salesforce — Service Cloud Real-Time (Messaging) API access.
  flows: []
  scope: scrt_api
- description: Salesforce — Account Engagement (Pardot) API access.
  flows: []
  scope: pardot_api
- description: Salesforce — Data Cloud API access.
  flows: []
  scope: cdp_api
- description: Salesforce — Data Cloud query API.
  flows: []
  scope: cdp_query_api
- description: Salesforce — Data Cloud ingestion API.
  flows: []
  scope: cdp_ingest_api
- description: Salesforce — Data Cloud profile API.
  flows: []
  scope: cdp_profile_api
- description: Salesforce — Data Cloud segmentation API.
  flows: []
  scope: cdp_segment_api
- description: Salesforce — Data Cloud identity resolution API.
  flows: []
  scope: cdp_identityresolution_api
- description: Salesforce — Data Cloud calculated insights API.
  flows: []
  scope: cdp_calculated_insight_api
- description: Salesforce — Data Cloud user claims.
  flows: []
  scope: data_cloud_user_claims
slug: hammerspace-scopes
source_filename: hammerspace-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: https://supportportal.hammerspace.com/.well-known/openid-configuration\napplies_to: >-\n  The Hammerspace customer support portal only. These are the Salesforce\n  Experience Cloud platform scopes advertised by the identity provider that\n  fronts supportportal.hammerspace.com. They are NOT scopes for the Hammerspace\n  Anvil management REST API, which authenticates with a form login and a session\n  cookie and exposes no OAuth scope surface at all. Recorded here because the\n  document is genuinely served from a Hammerspace host and describes a real\n  authorization surface — deliberately NOT wired as an OAuthScopes pointer in\n  apis.yml, because doing so would credit Hammerspace with a scoped OAuth model\n  for its data platform API that it does not publish.\nschemes:\n- name: supportportal-oidc\n  issuer: https://supportportal.hammerspace.com\n  platform: Salesforce Experience Cloud\n  source: well-known/hammerspace-openid-configuration.json\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://supportportal.hammerspace.com/services/oauth2/authorize\n    tokenUrl: https://supportportal.hammerspace.com/services/oauth2/token\n  - flow: implicit\n    authorizationUrl: https://supportportal.hammerspace.com/services/oauth2/authorize\n  response_types_supported: [code, token, token id_token]\n  token_endpoint_auth_methods_supported: [client_secret_post, client_secret_basic,\n    private_key_jwt]\n  id_token_signing_alg_values_supported: [RS256]\nscopes:\n- scope: openid\n  description: OIDC — request an ID token.\n- scope: profile\n  description: OIDC — basic profile claims.\n- scope: email\n  description: OIDC — email and email_verified claims.\n- scope: address\n  description: OIDC — address claim.\n- scope: phone\n  description: OIDC — phone_number and phone_number_verified claims.\n- scope: offline_access\n  description: OIDC — issue a refresh token.\n- scope: refresh_token\n  description: Salesforce alias for\
  \ offline_access.\n- scope: id\n  description: Salesforce — access the identity URL service.\n- scope: api\n  description: Salesforce — access the platform REST/SOAP APIs on the user's behalf.\n- scope: full\n  description: Salesforce — full access to all data accessible to the user.\n- scope: web\n  description: Salesforce — access web pages via a browser session.\n- scope: lightning\n  description: Salesforce — access Lightning applications.\n- scope: visualforce\n  description: Salesforce — access Visualforce pages.\n- scope: content\n  description: Salesforce — access Files/Content resources.\n- scope: chatter_api\n  description: Salesforce — Connect REST (Chatter) API access.\n- scope: chatbot_api\n  description: Salesforce — Einstein Bots API access.\n- scope: custom_permissions\n  description: Salesforce — return the user's custom permissions.\n- scope: forgot_password\n  description: Salesforce — headless password-reset flow.\n- scope: pwdless_login_api\n  description: Salesforce\
  \ — headless passwordless login flow.\n- scope: user_registration_api\n  description: Salesforce — headless self-registration flow.\n- scope: interaction_api\n  description: Salesforce — Interaction (Flow) API access.\n- scope: wave_api\n  description: Salesforce — CRM Analytics (Wave) API access.\n- scope: eclair_api\n  description: Salesforce — Einstein Vision/Language (Eclair) API access.\n- scope: einstein_gpt_api\n  description: Salesforce — Einstein GPT / models API access.\n- scope: sfap_api\n  description: Salesforce — Agentforce platform API access.\n- scope: mcp_api\n  description: >-\n    Salesforce — Model Context Protocol API access on the Experience Cloud\n    identity provider. This is a Salesforce platform scope, not a scope on\n    Hammerspace's own MCP server.\n- scope: scrt_api\n  description: Salesforce — Service Cloud Real-Time (Messaging) API access.\n- scope: pardot_api\n  description: Salesforce — Account Engagement (Pardot) API access.\n- scope: cdp_api\n  description:\
  \ Salesforce — Data Cloud API access.\n- scope: cdp_query_api\n  description: Salesforce — Data Cloud query API.\n- scope: cdp_ingest_api\n  description: Salesforce — Data Cloud ingestion API.\n- scope: cdp_profile_api\n  description: Salesforce — Data Cloud profile API.\n- scope: cdp_segment_api\n  description: Salesforce — Data Cloud segmentation API.\n- scope: cdp_identityresolution_api\n  description: Salesforce — Data Cloud identity resolution API.\n- scope: cdp_calculated_insight_api\n  description: Salesforce — Data Cloud calculated insights API.\n- scope: data_cloud_user_claims\n  description: Salesforce — Data Cloud user claims.\nx-evidence:\n  fetched: '2026-08-04'\n  url: https://supportportal.hammerspace.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json;charset=UTF-8\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hammerspace/refs/heads/main/scopes/hammerspace-scopes.yml
summary_line: 36 scopes · authorizationCode/implicit
tags:
- Company
- Storage
- Data Management
- Filesystem
- Data Orchestration
- Hybrid Cloud
- Kubernetes
- Artificial Intelligence
- Unstructured Data
- Infrastructure
token_urls:
- https://supportportal.hammerspace.com/services/oauth2/token
---
