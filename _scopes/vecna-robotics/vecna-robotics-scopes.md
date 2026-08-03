---
authorization_urls:
- https://vecnarobotics.my.site.com/services/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
- implicit
kind: oauth-scopes
layout: scope
method: probed
name: Vecna Robotics Scopes
name_suffix: OAuth Scopes
note: Scopes advertised by the scopes_supported array of the live OpenID Connect discovery document on the Vecna Robotics partner portal (Salesforce Experience Cloud). These are the Salesforce platform scope set as exposed on Vecna's org host, not a Vecna-authored scope taxonomy — Vecna Robotics publishes no product API and therefore no product scope reference. Descriptions are the documented meaning of each Salesforce OAuth scope; scope names are recorded verbatim from the discovery document.
overview: 'Vecna Robotics publishes 36 OAuth 2.0 scopes via the authorizationCode and implicit flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Vecna Robotics API on a user''s behalf.


  Tokens are issued from https://vecnarobotics.my.site.com/services/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Vecna Robotics
provider_slug: vecna-robotics
schemes:
- flows:
  - authorizationUrl: https://vecnarobotics.my.site.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://vecnarobotics.my.site.com/services/oauth2/token
  - authorizationUrl: https://vecnarobotics.my.site.com/services/oauth2/authorize
    flow: implicit
  issuer: https://vecnarobotics.my.site.com
  name: PartnerPortalOIDC
  source: well-known/vecna-robotics-openid-configuration.json
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
- description: Access the address claim.
  flows:
  - authorizationCode
  - implicit
  scope: address
- description: Access the Salesforce platform REST/SOAP APIs on behalf of the user.
  flows:
  - authorizationCode
  - implicit
  scope: api
- description: Access the Data Cloud (CDP) API.
  flows:
  - authorizationCode
  - implicit
  scope: cdp_api
- description: Access Data Cloud calculated insights.
  flows:
  - authorizationCode
  - implicit
  scope: cdp_calculated_insight_api
- description: Access Data Cloud identity resolution.
  flows:
  - authorizationCode
  - implicit
  scope: cdp_identityresolution_api
- description: Ingest records into Data Cloud.
  flows:
  - authorizationCode
  - implicit
  scope: cdp_ingest_api
- description: Access Data Cloud unified profiles.
  flows:
  - authorizationCode
  - implicit
  scope: cdp_profile_api
- description: Query Data Cloud data.
  flows:
  - authorizationCode
  - implicit
  scope: cdp_query_api
- description: Access Data Cloud segmentation.
  flows:
  - authorizationCode
  - implicit
  scope: cdp_segment_api
- description: Access the Einstein Bots (chatbot) API.
  flows:
  - authorizationCode
  - implicit
  scope: chatbot_api
- description: Access the Chatter (Connect) REST API.
  flows:
  - authorizationCode
  - implicit
  scope: chatter_api
- description: Access Salesforce content/files (Content and Files APIs).
  flows:
  - authorizationCode
  - implicit
  scope: content
- description: Return the custom permissions in the org associated with the user.
  flows:
  - authorizationCode
  - implicit
  scope: custom_permissions
- description: Return Data Cloud user claims in the token response.
  flows:
  - authorizationCode
  - implicit
  scope: data_cloud_user_claims
- description: Access the CRM Analytics Eclair chart API.
  flows:
  - authorizationCode
  - implicit
  scope: eclair_api
- description: Access the Einstein GPT / generative AI API.
  flows:
  - authorizationCode
  - implicit
  scope: einstein_gpt_api
- description: Access the email and email_verified claims.
  flows:
  - authorizationCode
  - implicit
  scope: email
- description: Access the forgot-password / password-reset API.
  flows:
  - authorizationCode
  - implicit
  scope: forgot_password
- description: Full access to all data accessible to the authenticated user (excludes refresh_token).
  flows:
  - authorizationCode
  - implicit
  scope: full
- description: Access the Salesforce identity URL for the user.
  flows:
  - authorizationCode
  - implicit
  scope: id
- description: Access the Salesforce Interaction (Marketing Cloud Personalization) API.
  flows:
  - authorizationCode
  - implicit
  scope: interaction_api
- description: Access Lightning Experience / Lightning component resources.
  flows:
  - authorizationCode
  - implicit
  scope: lightning
- description: Access the Salesforce Model Context Protocol (MCP) API surface.
  flows:
  - authorizationCode
  - implicit
  scope: mcp_api
- description: Equivalent to refresh_token; keep access after the user is offline.
  flows:
  - authorizationCode
  - implicit
  scope: offline_access
- description: Issue an OpenID Connect ID token for the authenticated portal user.
  flows:
  - authorizationCode
  - implicit
  scope: openid
- description: Access the Account Engagement (Pardot) API.
  flows:
  - authorizationCode
  - implicit
  scope: pardot_api
- description: Access the phone_number and phone_number_verified claims.
  flows:
  - authorizationCode
  - implicit
  scope: phone
- description: Access the standard OIDC profile claims for the authenticated user.
  flows:
  - authorizationCode
  - implicit
  scope: profile
- description: Access the passwordless login API.
  flows:
  - authorizationCode
  - implicit
  scope: pwdless_login_api
- description: Issue a refresh token so the client can obtain new access tokens.
  flows:
  - authorizationCode
  - implicit
  scope: refresh_token
- description: Access the Service Cloud Real-Time (SCRT) messaging API.
  flows:
  - authorizationCode
  - implicit
  scope: scrt_api
- description: Access the Salesforce AI platform (Models/Agent) API.
  flows:
  - authorizationCode
  - implicit
  scope: sfap_api
- description: Access the self-registration / user registration API for the portal.
  flows:
  - authorizationCode
  - implicit
  scope: user_registration_api
- description: Access Visualforce pages.
  flows:
  - authorizationCode
  - implicit
  scope: visualforce
- description: Access the CRM Analytics (Wave) REST API.
  flows:
  - authorizationCode
  - implicit
  scope: wave_api
- description: Open the portal web UI in a browser session using the issued access token.
  flows:
  - authorizationCode
  - implicit
  scope: web
slug: vecna-robotics-scopes
source_filename: vecna-robotics-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: https://vecnarobotics.my.site.com/.well-known/openid-configuration\nnote: Scopes advertised by the scopes_supported array of the live OpenID Connect discovery document on\n  the Vecna Robotics partner portal (Salesforce Experience Cloud). These are the Salesforce platform scope\n  set as exposed on Vecna's org host, not a Vecna-authored scope taxonomy — Vecna Robotics publishes no\n  product API and therefore no product scope reference. Descriptions are the documented meaning of each\n  Salesforce OAuth scope; scope names are recorded verbatim from the discovery document.\nschemes:\n- name: PartnerPortalOIDC\n  source: well-known/vecna-robotics-openid-configuration.json\n  issuer: https://vecnarobotics.my.site.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://vecnarobotics.my.site.com/services/oauth2/authorize\n    tokenUrl: https://vecnarobotics.my.site.com/services/oauth2/token\n  - flow: implicit\n\
  \    authorizationUrl: https://vecnarobotics.my.site.com/services/oauth2/authorize\nscope_count: 36\nscopes:\n- scope: address\n  description: Access the address claim.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/vecna-robotics-openid-configuration.json\n- scope: api\n  description: Access the Salesforce platform REST/SOAP APIs on behalf of the user.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/vecna-robotics-openid-configuration.json\n- scope: cdp_api\n  description: Access the Data Cloud (CDP) API.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/vecna-robotics-openid-configuration.json\n- scope: cdp_calculated_insight_api\n  description: Access Data Cloud calculated insights.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/vecna-robotics-openid-configuration.json\n- scope: cdp_identityresolution_api\n  description: Access Data Cloud identity resolution.\n  flows:\n  - authorizationCode\n\
  \  - implicit\n  sources:\n  - well-known/vecna-robotics-openid-configuration.json\n- scope: cdp_ingest_api\n  description: Ingest records into Data Cloud.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/vecna-robotics-openid-configuration.json\n- scope: cdp_profile_api\n  description: Access Data Cloud unified profiles.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/vecna-robotics-openid-configuration.json\n- scope: cdp_query_api\n  description: Query Data Cloud data.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/vecna-robotics-openid-configuration.json\n- scope: cdp_segment_api\n  description: Access Data Cloud segmentation.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/vecna-robotics-openid-configuration.json\n- scope: chatbot_api\n  description: Access the Einstein Bots (chatbot) API.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/vecna-robotics-openid-configuration.json\n\
  - scope: chatter_api\n  description: Access the Chatter (Connect) REST API.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/vecna-robotics-openid-configuration.json\n- scope: content\n  description: Access Salesforce content/files (Content and Files APIs).\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/vecna-robotics-openid-configuration.json\n- scope: custom_permissions\n  description: Return the custom permissions in the org associated with the user.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/vecna-robotics-openid-configuration.json\n- scope: data_cloud_user_claims\n  description: Return Data Cloud user claims in the token response.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/vecna-robotics-openid-configuration.json\n- scope: eclair_api\n  description: Access the CRM Analytics Eclair chart API.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/vecna-robotics-openid-configuration.json\n\
  - scope: einstein_gpt_api\n  description: Access the Einstein GPT / generative AI API.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/vecna-robotics-openid-configuration.json\n- scope: email\n  description: Access the email and email_verified claims.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/vecna-robotics-openid-configuration.json\n- scope: forgot_password\n  description: Access the forgot-password / password-reset API.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/vecna-robotics-openid-configuration.json\n- scope: full\n  description: Full access to all data accessible to the authenticated user (excludes refresh_token).\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/vecna-robotics-openid-configuration.json\n- scope: id\n  description: Access the Salesforce identity URL for the user.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/vecna-robotics-openid-configuration.json\n\
  - scope: interaction_api\n  description: Access the Salesforce Interaction (Marketing Cloud Personalization) API.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/vecna-robotics-openid-configuration.json\n- scope: lightning\n  description: Access Lightning Experience / Lightning component resources.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/vecna-robotics-openid-configuration.json\n- scope: mcp_api\n  description: Access the Salesforce Model Context Protocol (MCP) API surface.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/vecna-robotics-openid-configuration.json\n- scope: offline_access\n  description: Equivalent to refresh_token; keep access after the user is offline.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/vecna-robotics-openid-configuration.json\n- scope: openid\n  description: Issue an OpenID Connect ID token for the authenticated portal user.\n  flows:\n  - authorizationCode\n\
  \  - implicit\n  sources:\n  - well-known/vecna-robotics-openid-configuration.json\n- scope: pardot_api\n  description: Access the Account Engagement (Pardot) API.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/vecna-robotics-openid-configuration.json\n- scope: phone\n  description: Access the phone_number and phone_number_verified claims.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/vecna-robotics-openid-configuration.json\n- scope: profile\n  description: Access the standard OIDC profile claims for the authenticated user.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/vecna-robotics-openid-configuration.json\n- scope: pwdless_login_api\n  description: Access the passwordless login API.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/vecna-robotics-openid-configuration.json\n- scope: refresh_token\n  description: Issue a refresh token so the client can obtain new access tokens.\n\
  \  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/vecna-robotics-openid-configuration.json\n- scope: scrt_api\n  description: Access the Service Cloud Real-Time (SCRT) messaging API.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/vecna-robotics-openid-configuration.json\n- scope: sfap_api\n  description: Access the Salesforce AI platform (Models/Agent) API.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/vecna-robotics-openid-configuration.json\n- scope: user_registration_api\n  description: Access the self-registration / user registration API for the portal.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/vecna-robotics-openid-configuration.json\n- scope: visualforce\n  description: Access Visualforce pages.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/vecna-robotics-openid-configuration.json\n- scope: wave_api\n  description: Access the CRM Analytics\
  \ (Wave) REST API.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/vecna-robotics-openid-configuration.json\n- scope: web\n  description: Open the portal web UI in a browser session using the issued access token.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/vecna-robotics-openid-configuration.json\nx-evidence:\n  fetched: '2026-08-02'\n  url: https://vecnarobotics.my.site.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json;charset=UTF-8\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vecna-robotics/refs/heads/main/scopes/vecna-robotics-scopes.yml
summary_line: 36 scopes · authorizationCode/implicit
tags:
- Company
- Robotics
- Warehouse Automation
- Autonomous Mobile Robots
- Material Handling
- Logistics
- Supply Chain
- Manufacturing
- Industrial Automation
- Robotics as a Service
token_urls:
- https://vecnarobotics.my.site.com/services/oauth2/token
---
