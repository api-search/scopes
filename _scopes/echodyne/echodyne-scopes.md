---
authorization_urls:
- https://portal.echodyne.com/services/oauth2/authorize
description: ''
docs: https://portal.echodyne.com/s/login/
flows:
- authorizationCode
- implicit
kind: oauth-scopes
layout: scope
method: searched
name: Echodyne Scopes
name_suffix: OAuth Scopes
note: Scopes advertised by the Echodyne Customer Portal OpenID Connect discovery document. The portal runs on Salesforce Experience Cloud, so scopes_supported is the Salesforce platform scope vocabulary advertised by that tenant, not a scope surface Echodyne authored for its radar API. Recorded verbatim as probed; which scopes are actually grantable to a given portal client is not publicly documented. The EchoWare radar management/data API publishes no OAuth scope reference on the open web.
overview: 'Echodyne publishes 36 OAuth 2.0 scopes via the authorizationCode and implicit flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Echodyne API on a user''s behalf.


  Tokens are issued from https://portal.echodyne.com/services/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Echodyne
provider_slug: echodyne
schemes:
- flows:
  - authorizationUrl: https://portal.echodyne.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://portal.echodyne.com/services/oauth2/token
  - authorizationUrl: https://portal.echodyne.com/services/oauth2/authorize
    flow: implicit
  issuer: https://portal.echodyne.com
  name: EchodynePortalOIDC
  source: well-known/echodyne-openid-configuration.json
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
- description: Access the user address claim.
  flows: []
  scope: address
- description: Access the Salesforce platform REST/SOAP APIs on behalf of the portal user.
  flows: []
  scope: api
- description: Access the Data Cloud (CDP) API.
  flows: []
  scope: cdp_api
- description: Access the Data Cloud calculated insights API.
  flows: []
  scope: cdp_calculated_insight_api
- description: Access the Data Cloud identity resolution API.
  flows: []
  scope: cdp_identityresolution_api
- description: Access the Data Cloud ingestion API.
  flows: []
  scope: cdp_ingest_api
- description: Access the Data Cloud profile API.
  flows: []
  scope: cdp_profile_api
- description: Access the Data Cloud query API.
  flows: []
  scope: cdp_query_api
- description: Access the Data Cloud segmentation API.
  flows: []
  scope: cdp_segment_api
- description: Access the bot/chatbot API.
  flows: []
  scope: chatbot_api
- description: Access the Connect (Chatter) REST API.
  flows: []
  scope: chatter_api
- description: Access content/files resources.
  flows: []
  scope: content
- description: Return the custom permissions granted to the portal user.
  flows: []
  scope: custom_permissions
- description: Return Data Cloud user claims.
  flows: []
  scope: data_cloud_user_claims
- description: Access the Eclair analytics chart API.
  flows: []
  scope: eclair_api
- description: Access the Einstein GPT / generative AI API.
  flows: []
  scope: einstein_gpt_api
- description: Access the user email and email_verified claims.
  flows: []
  scope: email
- description: Access the forgot-password flow API.
  flows: []
  scope: forgot_password
- description: Full access to all data the portal user can access (excludes refresh_token).
  flows: []
  scope: full
- description: Access the identity URL service.
  flows: []
  scope: id
- description: Access the interaction/journey API.
  flows: []
  scope: interaction_api
- description: Access Lightning Experience / Experience Cloud resources.
  flows: []
  scope: lightning
- description: Access the platform Model Context Protocol (MCP) API.
  flows: []
  scope: mcp_api
- description: Issue a refresh token (OIDC synonym of refresh_token).
  flows: []
  scope: offline_access
- description: Request an ID token (OpenID Connect).
  flows: []
  scope: openid
- description: Access the Pardot/Account Engagement API.
  flows: []
  scope: pardot_api
- description: Access the user phone_number and phone_number_verified claims.
  flows: []
  scope: phone
- description: Access the standard OIDC profile claims for the portal user.
  flows: []
  scope: profile
- description: Access the passwordless login API.
  flows: []
  scope: pwdless_login_api
- description: Issue a refresh token for long-lived access.
  flows: []
  scope: refresh_token
- description: Access the Service Cloud real-time (messaging) API.
  flows: []
  scope: scrt_api
- description: Access the platform agent/AI (Agentforce) API.
  flows: []
  scope: sfap_api
- description: Access the self-registration API.
  flows: []
  scope: user_registration_api
- description: Access Visualforce pages.
  flows: []
  scope: visualforce
- description: Access the analytics (Wave/CRM Analytics) API.
  flows: []
  scope: wave_api
- description: Access the portal web UI with the issued token.
  flows: []
  scope: web
slug: echodyne-scopes
source_filename: echodyne-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: https://portal.echodyne.com/.well-known/openid-configuration\ndocs: https://portal.echodyne.com/s/login/\nnote: Scopes advertised by the Echodyne Customer Portal OpenID Connect discovery document. The portal\n  runs on Salesforce Experience Cloud, so scopes_supported is the Salesforce platform scope vocabulary\n  advertised by that tenant, not a scope surface Echodyne authored for its radar API. Recorded verbatim\n  as probed; which scopes are actually grantable to a given portal client is not publicly documented.\n  The EchoWare radar management/data API publishes no OAuth scope reference on the open web.\nschemes:\n- name: EchodynePortalOIDC\n  issuer: https://portal.echodyne.com\n  source: well-known/echodyne-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://portal.echodyne.com/services/oauth2/authorize\n    tokenUrl: https://portal.echodyne.com/services/oauth2/token\n  - flow:\
  \ implicit\n    authorizationUrl: https://portal.echodyne.com/services/oauth2/authorize\nscopes:\n- scope: address\n  description: Access the user address claim.\n  sources:\n  - well-known/echodyne-openid-configuration.json\n- scope: api\n  description: Access the Salesforce platform REST/SOAP APIs on behalf of the portal user.\n  sources:\n  - well-known/echodyne-openid-configuration.json\n- scope: cdp_api\n  description: Access the Data Cloud (CDP) API.\n  sources:\n  - well-known/echodyne-openid-configuration.json\n- scope: cdp_calculated_insight_api\n  description: Access the Data Cloud calculated insights API.\n  sources:\n  - well-known/echodyne-openid-configuration.json\n- scope: cdp_identityresolution_api\n  description: Access the Data Cloud identity resolution API.\n  sources:\n  - well-known/echodyne-openid-configuration.json\n- scope: cdp_ingest_api\n  description: Access the Data Cloud ingestion API.\n  sources:\n  - well-known/echodyne-openid-configuration.json\n- scope:\
  \ cdp_profile_api\n  description: Access the Data Cloud profile API.\n  sources:\n  - well-known/echodyne-openid-configuration.json\n- scope: cdp_query_api\n  description: Access the Data Cloud query API.\n  sources:\n  - well-known/echodyne-openid-configuration.json\n- scope: cdp_segment_api\n  description: Access the Data Cloud segmentation API.\n  sources:\n  - well-known/echodyne-openid-configuration.json\n- scope: chatbot_api\n  description: Access the bot/chatbot API.\n  sources:\n  - well-known/echodyne-openid-configuration.json\n- scope: chatter_api\n  description: Access the Connect (Chatter) REST API.\n  sources:\n  - well-known/echodyne-openid-configuration.json\n- scope: content\n  description: Access content/files resources.\n  sources:\n  - well-known/echodyne-openid-configuration.json\n- scope: custom_permissions\n  description: Return the custom permissions granted to the portal user.\n  sources:\n  - well-known/echodyne-openid-configuration.json\n- scope: data_cloud_user_claims\n\
  \  description: Return Data Cloud user claims.\n  sources:\n  - well-known/echodyne-openid-configuration.json\n- scope: eclair_api\n  description: Access the Eclair analytics chart API.\n  sources:\n  - well-known/echodyne-openid-configuration.json\n- scope: einstein_gpt_api\n  description: Access the Einstein GPT / generative AI API.\n  sources:\n  - well-known/echodyne-openid-configuration.json\n- scope: email\n  description: Access the user email and email_verified claims.\n  sources:\n  - well-known/echodyne-openid-configuration.json\n- scope: forgot_password\n  description: Access the forgot-password flow API.\n  sources:\n  - well-known/echodyne-openid-configuration.json\n- scope: full\n  description: Full access to all data the portal user can access (excludes refresh_token).\n  sources:\n  - well-known/echodyne-openid-configuration.json\n- scope: id\n  description: Access the identity URL service.\n  sources:\n  - well-known/echodyne-openid-configuration.json\n- scope: interaction_api\n\
  \  description: Access the interaction/journey API.\n  sources:\n  - well-known/echodyne-openid-configuration.json\n- scope: lightning\n  description: Access Lightning Experience / Experience Cloud resources.\n  sources:\n  - well-known/echodyne-openid-configuration.json\n- scope: mcp_api\n  description: Access the platform Model Context Protocol (MCP) API.\n  sources:\n  - well-known/echodyne-openid-configuration.json\n- scope: offline_access\n  description: Issue a refresh token (OIDC synonym of refresh_token).\n  sources:\n  - well-known/echodyne-openid-configuration.json\n- scope: openid\n  description: Request an ID token (OpenID Connect).\n  sources:\n  - well-known/echodyne-openid-configuration.json\n- scope: pardot_api\n  description: Access the Pardot/Account Engagement API.\n  sources:\n  - well-known/echodyne-openid-configuration.json\n- scope: phone\n  description: Access the user phone_number and phone_number_verified claims.\n  sources:\n  - well-known/echodyne-openid-configuration.json\n\
  - scope: profile\n  description: Access the standard OIDC profile claims for the portal user.\n  sources:\n  - well-known/echodyne-openid-configuration.json\n- scope: pwdless_login_api\n  description: Access the passwordless login API.\n  sources:\n  - well-known/echodyne-openid-configuration.json\n- scope: refresh_token\n  description: Issue a refresh token for long-lived access.\n  sources:\n  - well-known/echodyne-openid-configuration.json\n- scope: scrt_api\n  description: Access the Service Cloud real-time (messaging) API.\n  sources:\n  - well-known/echodyne-openid-configuration.json\n- scope: sfap_api\n  description: Access the platform agent/AI (Agentforce) API.\n  sources:\n  - well-known/echodyne-openid-configuration.json\n- scope: user_registration_api\n  description: Access the self-registration API.\n  sources:\n  - well-known/echodyne-openid-configuration.json\n- scope: visualforce\n  description: Access Visualforce pages.\n  sources:\n  - well-known/echodyne-openid-configuration.json\n\
  - scope: wave_api\n  description: Access the analytics (Wave/CRM Analytics) API.\n  sources:\n  - well-known/echodyne-openid-configuration.json\n- scope: web\n  description: Access the portal web UI with the issued token.\n  sources:\n  - well-known/echodyne-openid-configuration.json\nx-evidence:\n  fetched: '2026-08-01'\n  url: https://portal.echodyne.com/.well-known/openid-configuration\n  http_status: 200\n  scope_count: 36\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/echodyne/refs/heads/main/scopes/echodyne-scopes.yml
summary_line: 36 scopes · authorizationCode/implicit
tags:
- Company
- Radar
- Defense
- Government
- Critical Infrastructure
- Counter-UAS
- Drone Detection
- Sensors
- Situational Awareness
- Aerospace
- Hardware
- Public Safety
token_urls:
- https://portal.echodyne.com/services/oauth2/token
---
