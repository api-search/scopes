---
api_specs:
- filename: salesforce-openapi.yml
  format: yaml
  label: Salesforce REST API
  slug: salesforce-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/openapi/salesforce-openapi.yml
- filename: salesforce-bulk-api-2-openapi.yml
  format: yaml
  label: Salesforce Bulk API 2.0
  slug: salesforce-bulk-api-2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/openapi/salesforce-bulk-api-2-openapi.yml
- filename: salesforce-streaming-asyncapi.yml
  format: yaml
  label: Salesforce Streaming API
  slug: salesforce-streaming-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/asyncapi/salesforce-streaming-asyncapi.yml
- filename: salesforce-platform-events-asyncapi.yml
  format: yaml
  label: Salesforce Platform Events API
  slug: salesforce-platform-events-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/asyncapi/salesforce-platform-events-asyncapi.yml
- filename: salesforce-change-data-capture-asyncapi.yml
  format: yaml
  label: Salesforce Change Data Capture API
  slug: salesforce-change-data-capture-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/asyncapi/salesforce-change-data-capture-asyncapi.yml
- filename: salesforce-ui-api-openapi.yml
  format: yaml
  label: Salesforce UI API
  slug: salesforce-ui-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/openapi/salesforce-ui-api-openapi.yml
- filename: salesforce-marketing-cloud-rest-openapi.yml
  format: yaml
  label: Salesforce Marketing Cloud REST API
  slug: salesforce-marketing-cloud-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/openapi/salesforce-marketing-cloud-rest-openapi.yml
- filename: salesforce-openapi.yml
  format: yaml
  label: Salesforce
  slug: salesforce-salesforce
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/openapi/salesforce-openapi.yml
authorization_urls:
- https://login.salesforce.com/services/oauth2/authorize
description: ''
docs: https://help.salesforce.com/s/articleView?id=sf.remoteaccess_oauth_tokens_scopes.htm
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Salesforce Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Salesforce publishes 36 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Salesforce API on a user''s behalf.


  Tokens are issued from https://login.salesforce.com/services/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Salesforce
provider_slug: salesforce
schemes:
- flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  source: https://login.salesforce.com/.well-known/openid-configuration
  type: oauth2
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
- visualforce
- lightning
- content
- chatter_api
- chatbot_api
- wave_api
- eclair_api
- pardot_api
- interaction_api
- custom_permissions
- user_registration_api
- pwdless_login_api
- forgot_password
- sfap_api
- einstein_gpt_api
- mcp_api
- scrt_api
- cdp_api
- cdp_query_api
- cdp_ingest_api
- cdp_profile_api
- cdp_segment_api
- cdp_calculated_insight_api
- cdp_identityresolution_api
- data_cloud_user_claims
scopes:
- description: OpenID Connect — return an ID token (OIDC).
  flows: []
  scope: openid
- description: Access basic profile information (name
  flows: []
  scope: profile
- description: Access the user's email address.
  flows: []
  scope: email
- description: Access the user's address information.
  flows: []
  scope: address
- description: Access the user's phone number.
  flows: []
  scope: phone
- description: Access the identity URL service.
  flows: []
  scope: id
- description: Access the Salesforce APIs (REST
  flows: []
  scope: api
- description: Access to Salesforce web pages / Visualforce via the access token.
  flows: []
  scope: web
- description: Full access to all data accessible by the user; does not grant refresh_token.
  flows: []
  scope: full
- description: Obtain a refresh token for long-lived access (same as offline_access).
  flows: []
  scope: refresh_token
- description: Obtain a refresh token for offline access.
  flows: []
  scope: offline_access
- description: Access Visualforce pages.
  flows: []
  scope: visualforce
- description: Access Lightning applications and components.
  flows: []
  scope: lightning
- description: Access Salesforce CRM Content and Files (ContentDocument) resources.
  flows: []
  scope: content
- description: Access the Chatter / Connect REST API.
  flows: []
  scope: chatter_api
- description: Access the Einstein Bots / chatbot API.
  flows: []
  scope: chatbot_api
- description: Access the CRM Analytics (Wave/Tableau CRM) REST API.
  flows: []
  scope: wave_api
- description: Access CRM Analytics Eclair chart-rendering API.
  flows: []
  scope: eclair_api
- description: Access the Pardot / Account Engagement API.
  flows: []
  scope: pardot_api
- description: Access the Interaction Studio / messaging interaction API.
  flows: []
  scope: interaction_api
- description: Return the custom permissions in the org associated with the user.
  flows: []
  scope: custom_permissions
- description: Access the self-registration / user registration API.
  flows: []
  scope: user_registration_api
- description: Access the passwordless login API.
  flows: []
  scope: pwdless_login_api
- description: Access the forgot-password / headless password-reset API.
  flows: []
  scope: forgot_password
- description: Access the Salesforce Foundations / Agentforce platform API.
  flows: []
  scope: sfap_api
- description: Access Einstein GPT / generative AI (Models) API.
  flows: []
  scope: einstein_gpt_api
- description: Access the Salesforce Model Context Protocol (MCP) API surface.
  flows: []
  scope: mcp_api
- description: Access the Service Cloud real-time (messaging) API.
  flows: []
  scope: scrt_api
- description: Access the Data Cloud (CDP) API.
  flows: []
  scope: cdp_api
- description: Run queries against Data Cloud.
  flows: []
  scope: cdp_query_api
- description: Ingest data into Data Cloud.
  flows: []
  scope: cdp_ingest_api
- description: Access unified customer profiles in Data Cloud.
  flows: []
  scope: cdp_profile_api
- description: Manage Data Cloud segments.
  flows: []
  scope: cdp_segment_api
- description: Access Data Cloud calculated insights.
  flows: []
  scope: cdp_calculated_insight_api
- description: Access Data Cloud identity resolution.
  flows: []
  scope: cdp_identityresolution_api
- description: Return Data Cloud user claims in the token.
  flows: []
  scope: data_cloud_user_claims
slug: salesforce-scopes
source_filename: salesforce-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: https://login.salesforce.com/.well-known/openid-configuration\ndocs: https://help.salesforce.com/s/articleView?id=sf.remoteaccess_oauth_tokens_scopes.htm\nnotes: >-\n  Authoritative scope list taken verbatim from the Salesforce identity host OIDC discovery\n  document (scopes_supported). Salesforce OAuth scopes are org-wide connected-app permissions,\n  not per-object; fine-grained authorization is enforced by profiles, permission sets, and\n  sharing rules on top of these scopes.\nauthorization_endpoint: https://login.salesforce.com/services/oauth2/authorize\ntoken_endpoint: https://login.salesforce.com/services/oauth2/token\nschemes:\n  - name: oauth2\n    type: oauth2\n    source: https://login.salesforce.com/.well-known/openid-configuration\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n        tokenUrl: https://login.salesforce.com/services/oauth2/token\n\
  scopes:\n  - {scope: openid, description: OpenID Connect — return an ID token (OIDC).}\n  - {scope: profile, description: Access basic profile information (name, photo, etc.) via the userinfo endpoint.}\n  - {scope: email, description: Access the user's email address.}\n  - {scope: address, description: Access the user's address information.}\n  - {scope: phone, description: Access the user's phone number.}\n  - {scope: id, description: Access the identity URL service.}\n  - {scope: api, description: Access the Salesforce APIs (REST, SOAP, Bulk, etc.) on the user's behalf.}\n  - {scope: web, description: Access to Salesforce web pages / Visualforce via the access token.}\n  - {scope: full, description: Full access to all data accessible by the user; does not grant refresh_token.}\n  - {scope: refresh_token, description: Obtain a refresh token for long-lived access (same as offline_access).}\n  - {scope: offline_access, description: Obtain a refresh token for offline access.}\n  - {scope:\
  \ visualforce, description: Access Visualforce pages.}\n  - {scope: lightning, description: Access Lightning applications and components.}\n  - {scope: content, description: Access Salesforce CRM Content and Files (ContentDocument) resources.}\n  - {scope: chatter_api, description: Access the Chatter / Connect REST API.}\n  - {scope: chatbot_api, description: Access the Einstein Bots / chatbot API.}\n  - {scope: wave_api, description: Access the CRM Analytics (Wave/Tableau CRM) REST API.}\n  - {scope: eclair_api, description: Access CRM Analytics Eclair chart-rendering API.}\n  - {scope: pardot_api, description: Access the Pardot / Account Engagement API.}\n  - {scope: interaction_api, description: Access the Interaction Studio / messaging interaction API.}\n  - {scope: custom_permissions, description: Return the custom permissions in the org associated with the user.}\n  - {scope: user_registration_api, description: Access the self-registration / user registration API.}\n  - {scope: pwdless_login_api,\
  \ description: Access the passwordless login API.}\n  - {scope: forgot_password, description: Access the forgot-password / headless password-reset API.}\n  - {scope: sfap_api, description: Access the Salesforce Foundations / Agentforce platform API.}\n  - {scope: einstein_gpt_api, description: Access Einstein GPT / generative AI (Models) API.}\n  - {scope: mcp_api, description: Access the Salesforce Model Context Protocol (MCP) API surface.}\n  - {scope: scrt_api, description: Access the Service Cloud real-time (messaging) API.}\n  # --- Data Cloud (CDP) scopes ---\n  - {scope: cdp_api, description: Access the Data Cloud (CDP) API.}\n  - {scope: cdp_query_api, description: Run queries against Data Cloud.}\n  - {scope: cdp_ingest_api, description: Ingest data into Data Cloud.}\n  - {scope: cdp_profile_api, description: Access unified customer profiles in Data Cloud.}\n  - {scope: cdp_segment_api, description: Manage Data Cloud segments.}\n  - {scope: cdp_calculated_insight_api, description:\
  \ Access Data Cloud calculated insights.}\n  - {scope: cdp_identityresolution_api, description: Access Data Cloud identity resolution.}\n  - {scope: data_cloud_user_claims, description: Return Data Cloud user claims in the token.}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/scopes/salesforce-scopes.yml
summary_line: 36 scopes · authorizationCode
tags:
- Fortune 500
- AI
- Analytics
- Cloud
- Commerce
- CRM
- Customer Service
- Enterprise
- Marketing
- Platform
- Sales
token_urls:
- https://login.salesforce.com/services/oauth2/token
---
