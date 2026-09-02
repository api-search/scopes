---
api_specs:
- filename: service-cloud-bot-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud APIs Bot API
  slug: service-cloud-bot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/service-cloud/refs/heads/main/openapi/service-cloud-bot-api-openapi.yml
- filename: service-cloud-health-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud APIs Health API
  slug: service-cloud-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/service-cloud/refs/heads/main/openapi/service-cloud-health-api-openapi.yml
- filename: service-cloud-versions-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud APIs Versions API
  slug: service-cloud-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/service-cloud/refs/heads/main/openapi/service-cloud-versions-api-openapi.yml
authorization_urls:
- https://login.salesforce.com/services/oauth2/authorize
description: ''
docs: https://help.salesforce.com/s/articleView?id=platform.remoteaccess_oauth_tokens_scopes.htm&type=5
flows:
- authorizationCode
- implicit
kind: oauth-scopes
layout: scope
method: searched
name: Service Cloud Scopes
name_suffix: OAuth Scopes
note: 'The scope list is READ FROM THE PROVIDER''S OWN DISCOVERY DOCUMENTS, not from prose. Two documents disagree: login.salesforce.com/.well-known/openid-configuration advertises 37 scopes; the api.salesforce.com authorization-server document advertises only 4. Both are recorded.'
overview: 'Salesforce Service Cloud APIs publishes 36 OAuth 2.0 scopes via the authorizationCode and implicit flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Salesforce Service Cloud APIs API on a user''s behalf.


  Tokens are issued from https://login.salesforce.com/services/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Salesforce Service Cloud APIs
provider_slug: service-cloud
schemes:
- description: chatbotAuth supports authorization code and implicit OAuth flows.
  flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: implicit
  name: chatbotAuth
  source: openapi/service-cloud-einstein-bots-openapi.yml
  type: oauth2
- description: Salesforce OAuth access token obtained using the JWT Bearer flow. Use the chatbot_api scope with this flow to enable access to the Einstein Bots services.
  name: jwtBearer
  scheme: bearer
  source: openapi/service-cloud-einstein-bots-openapi.yml
  type: http
scope_count: 36
scope_names:
- api
- mcp_api
- chatbot_api
- refresh_token
- offline_access
- sfap_api
- einstein_gpt_api
- full
- openid
- id
- profile
- email
- address
- phone
- web
- lightning
- visualforce
- content
- chatter_api
- custom_permissions
- interaction_api
- wave_api
- eclair_api
- pardot_api
- scrt_api
- user_registration_api
- pwdless_login_api
- forgot_password
- cdp_api
- cdp_ingest_api
- cdp_query_api
- cdp_profile_api
- cdp_segment_api
- cdp_identityresolution_api
- cdp_calculated_insight_api
- data_cloud_user_claims
scopes:
- description: Access the Salesforce platform APIs (REST, SOAP, Bulk) as the authenticated user. The scope Service Cloud record work runs on.
  flows: []
  scope: api
- description: Call the Salesforce hosted MCP servers.
  flows: []
  scope: mcp_api
- description: Access bot APIs — the Einstein Bots Runtime API.
  flows: []
  scope: chatbot_api
- description: Issue a refresh token so the client can obtain new access tokens without re-prompting.
  flows: []
  scope: refresh_token
- description: OIDC equivalent of refresh_token.
  flows: []
  scope: offline_access
- description: Salesforce AI Platform API access.
  flows: []
  scope: sfap_api
- description: Einstein GPT / generative AI platform API access.
  flows: []
  scope: einstein_gpt_api
- description: Full access to all data the user can access. Broadest scope; avoid for agent clients.
  flows: []
  scope: full
- description: OIDC — issue an ID token.
  flows: []
  scope: openid
- description: Access the identity URL service.
  flows: []
  scope: id
- description: ''
  flows: []
  scope: profile
- description: ''
  flows: []
  scope: email
- description: ''
  flows: []
  scope: address
- description: ''
  flows: []
  scope: phone
- description: Access to the web UI via the access token.
  flows: []
  scope: web
- description: Access Lightning applications.
  flows: []
  scope: lightning
- description: Access Visualforce pages.
  flows: []
  scope: visualforce
- description: Access Salesforce CRM Content.
  flows: []
  scope: content
- description: Access the Connect REST API (Chatter/Connect).
  flows: []
  scope: chatter_api
- description: Return the custom permissions in the org associated with the connected app.
  flows: []
  scope: custom_permissions
- description: Interaction Studio / personalization API.
  flows: []
  scope: interaction_api
- description: CRM Analytics (Wave/Tableau CRM) REST API.
  flows: []
  scope: wave_api
- description: CRM Analytics Eclair chart API.
  flows: []
  scope: eclair_api
- description: Account Engagement (Pardot) API.
  flows: []
  scope: pardot_api
- description: Service Cloud Real-Time (SCRT) — the Messaging for In-App and Web transport.
  flows: []
  scope: scrt_api
- description: ''
  flows: []
  scope: user_registration_api
- description: Passwordless login API.
  flows: []
  scope: pwdless_login_api
- description: ''
  flows: []
  scope: forgot_password
- description: Data Cloud / CDP API.
  flows: []
  scope: cdp_api
- description: ''
  flows: []
  scope: cdp_ingest_api
- description: ''
  flows: []
  scope: cdp_query_api
- description: ''
  flows: []
  scope: cdp_profile_api
- description: ''
  flows: []
  scope: cdp_segment_api
- description: ''
  flows: []
  scope: cdp_identityresolution_api
- description: ''
  flows: []
  scope: cdp_calculated_insight_api
- description: ''
  flows: []
  scope: data_cloud_user_claims
slug: service-cloud-scopes
source_filename: service-cloud-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: >-\n  https://login.salesforce.com/.well-known/openid-configuration (probed 200, 2026-08-27 — saved to\n  well-known/service-cloud-login-openid-configuration.json),\n  https://api.salesforce.com/.well-known/oauth-authorization-server (probed 200),\n  https://api.salesforce.com/.well-known/oauth-protected-resource/platform/mcp/v1/platform/sobject-all (probed 200),\n  and openapi/service-cloud-einstein-bots-openapi.yml\ndocs: https://help.salesforce.com/s/articleView?id=platform.remoteaccess_oauth_tokens_scopes.htm&type=5\nnote: >-\n  The scope list is READ FROM THE PROVIDER'S OWN DISCOVERY DOCUMENTS, not from prose. Two documents\n  disagree: login.salesforce.com/.well-known/openid-configuration advertises 37 scopes; the\n  api.salesforce.com authorization-server document advertises only 4. Both are recorded.\nschemes:\n  - name: chatbotAuth\n    type: oauth2\n    source: openapi/service-cloud-einstein-bots-openapi.yml\n   \
  \ flows:\n      - flow: authorizationCode\n        authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n        tokenUrl: https://login.salesforce.com/services/oauth2/token\n      - flow: implicit\n        authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    description: chatbotAuth supports authorization code and implicit OAuth flows.\n  - name: jwtBearer\n    type: http\n    scheme: bearer\n    source: openapi/service-cloud-einstein-bots-openapi.yml\n    description: >-\n      Salesforce OAuth access token obtained using the JWT Bearer flow. Use the chatbot_api scope\n      with this flow to enable access to the Einstein Bots services.\nscopes:\n  - scope: api\n    description: Access the Salesforce platform APIs (REST, SOAP, Bulk) as the authenticated user. The scope Service Cloud record work runs on.\n    advertised_by: [login.salesforce.com, api.salesforce.com]\n  - scope: mcp_api\n    description: Call the Salesforce hosted MCP servers.\n\
  \    advertised_by: [login.salesforce.com, 'api.salesforce.com (per-resource metadata for /platform/mcp/v1/platform/sobject-all)']\n  - scope: chatbot_api\n    description: Access bot APIs — the Einstein Bots Runtime API.\n    advertised_by: [login.salesforce.com, 'openapi/service-cloud-einstein-bots-openapi.yml']\n  - scope: refresh_token\n    description: Issue a refresh token so the client can obtain new access tokens without re-prompting.\n    advertised_by: [login.salesforce.com, api.salesforce.com, 'api.salesforce.com per-resource metadata']\n  - scope: offline_access\n    description: OIDC equivalent of refresh_token.\n    advertised_by: [login.salesforce.com]\n  - scope: sfap_api\n    description: Salesforce AI Platform API access.\n    advertised_by: [login.salesforce.com, api.salesforce.com]\n  - scope: einstein_gpt_api\n    description: Einstein GPT / generative AI platform API access.\n    advertised_by: [login.salesforce.com, api.salesforce.com]\n  - scope: full\n    description:\
  \ Full access to all data the user can access. Broadest scope; avoid for agent clients.\n    advertised_by: [login.salesforce.com]\n  - scope: openid\n    description: OIDC — issue an ID token.\n    advertised_by: [login.salesforce.com]\n  - scope: id\n    description: Access the identity URL service.\n    advertised_by: [login.salesforce.com]\n  - scope: profile\n    advertised_by: [login.salesforce.com]\n  - scope: email\n    advertised_by: [login.salesforce.com]\n  - scope: address\n    advertised_by: [login.salesforce.com]\n  - scope: phone\n    advertised_by: [login.salesforce.com]\n  - scope: web\n    description: Access to the web UI via the access token.\n    advertised_by: [login.salesforce.com]\n  - scope: lightning\n    description: Access Lightning applications.\n    advertised_by: [login.salesforce.com]\n  - scope: visualforce\n    description: Access Visualforce pages.\n    advertised_by: [login.salesforce.com]\n  - scope: content\n    description: Access Salesforce CRM Content.\n\
  \    advertised_by: [login.salesforce.com]\n  - scope: chatter_api\n    description: Access the Connect REST API (Chatter/Connect).\n    advertised_by: [login.salesforce.com]\n  - scope: custom_permissions\n    description: Return the custom permissions in the org associated with the connected app.\n    advertised_by: [login.salesforce.com]\n  - scope: interaction_api\n    description: Interaction Studio / personalization API.\n    advertised_by: [login.salesforce.com]\n  - scope: wave_api\n    description: CRM Analytics (Wave/Tableau CRM) REST API.\n    advertised_by: [login.salesforce.com]\n  - scope: eclair_api\n    description: CRM Analytics Eclair chart API.\n    advertised_by: [login.salesforce.com]\n  - scope: pardot_api\n    description: Account Engagement (Pardot) API.\n    advertised_by: [login.salesforce.com]\n  - scope: scrt_api\n    description: Service Cloud Real-Time (SCRT) — the Messaging for In-App and Web transport.\n    advertised_by: [login.salesforce.com]\n    note:\
  \ The most Service-Cloud-specific scope in the list.\n  - scope: user_registration_api\n    advertised_by: [login.salesforce.com]\n  - scope: pwdless_login_api\n    description: Passwordless login API.\n    advertised_by: [login.salesforce.com]\n  - scope: forgot_password\n    advertised_by: [login.salesforce.com]\n  - scope: cdp_api\n    description: Data Cloud / CDP API.\n    advertised_by: [login.salesforce.com]\n  - scope: cdp_ingest_api\n    advertised_by: [login.salesforce.com]\n  - scope: cdp_query_api\n    advertised_by: [login.salesforce.com]\n  - scope: cdp_profile_api\n    advertised_by: [login.salesforce.com]\n  - scope: cdp_segment_api\n    advertised_by: [login.salesforce.com]\n  - scope: cdp_identityresolution_api\n    advertised_by: [login.salesforce.com]\n  - scope: cdp_calculated_insight_api\n    advertised_by: [login.salesforce.com]\n  - scope: data_cloud_user_claims\n    advertised_by: [login.salesforce.com]\nscope_count: 36\nleast_privilege:\n  note: >-\n    Scopes\
  \ are coarse. `api` grants everything the authenticated USER can reach — there is no\n    read-only or Case-only scope. Fine-grained restriction is enforced by the org's profile,\n    permission set and sharing rules on that user, not by the token. For agents, the practical\n    least-privilege lever is choosing the narrow hosted MCP server (sobject-reads or\n    sobject-mutations instead of sobject-all) and a purpose-built integration user.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/service-cloud/refs/heads/main/scopes/service-cloud-scopes.yml
summary_line: 36 scopes · authorizationCode/implicit
tags:
- Cloud
- CRM
- Customer Service
- Enterprise
- Salesforce
- Support
token_urls:
- https://login.salesforce.com/services/oauth2/token
---
