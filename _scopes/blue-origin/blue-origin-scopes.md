---
authorization_urls:
- https://shopify.com/authentication/30100881545/oauth/authorize
- https://payloads.blueorigin.com/services/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Blue Origin Scopes
name_suffix: OAuth Scopes
note: Blue Origin declares no API scopes anywhere it publishes — there is no OpenAPI, no developer portal and no scopes/permissions reference page. Every scope below was read from scopes_supported in an OIDC discovery document served anonymously by a vendor platform bound to a blueorigin.com host. The shop scopes are Shopify customer-account scopes; the portal scopes are the stock Salesforce platform scope catalogue, identical on payloads.blueorigin.com and bodp.blueorigin.com because both communities sit on the same Salesforce org. Neither set contains a Blue-Origin-specific resource scope (there is no read:payloads, no launch:manifest). Treat these as platform scopes, not as a product authorization model.
overview: 'Blue Origin publishes 38 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Blue Origin API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/30100881545/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Blue Origin
provider_slug: blue-origin
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/30100881545/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/30100881545/oauth/token
  issuer: https://shopify.com/authentication/30100881545
  name: shopify-customer-account
  source: well-known/blue-origin-shop-openid-configuration.json
- also_served_by: https://bodp.blueorigin.com
  flows:
  - authorizationUrl: https://payloads.blueorigin.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://payloads.blueorigin.com/services/oauth2/token
  issuer: https://payloads.blueorigin.com
  name: salesforce-experience-cloud
  source: well-known/blue-origin-payloads-openid-configuration.json
scope_count: 38
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
- api
- full
- refresh_token
- offline_access
- profile
- address
- phone
- id
- web
- visualforce
- lightning
- content
- chatter_api
- custom_permissions
- wave_api
- eclair_api
- pardot_api
- interaction_api
- chatbot_api
- scrt_api
- sfap_api
- einstein_gpt_api
- mcp_api
- cdp_api
- cdp_ingest_api
- cdp_query_api
- cdp_profile_api
- cdp_segment_api
- cdp_identityresolution_api
- cdp_calculated_insight_api
- data_cloud_user_claims
- user_registration_api
- pwdless_login_api
- forgot_password
scopes:
- description: Issue an OIDC ID token for the authenticated end user.
  flows: []
  scope: openid
- description: Release the end user's email address claim.
  flows: []
  scope: email
- description: Full access to the Shopify Customer Account API for the signed-in shopper (orders, addresses, profile) on the Blue Origin Shop.
  flows: []
  scope: customer-account-api:full
- description: Full access to the customer-scoped MCP surface of the Blue Origin Shop — the authenticated counterpart of the anonymous /api/mcp tools.
  flows: []
  scope: customer-account-mcp-api:full
- description: Salesforce REST/SOAP/Bulk API access on behalf of the portal user.
  flows: []
  scope: api
- description: Full access to all data the portal user has access to.
  flows: []
  scope: full
- description: Issue a refresh token so the client can renew access without re-prompting.
  flows: []
  scope: refresh_token
- description: Offline access — the OIDC alias of refresh_token.
  flows: []
  scope: offline_access
- description: Basic profile claims for the portal user.
  flows: []
  scope: profile
- description: The end user's address claim.
  flows: []
  scope: address
- description: The end user's phone number claim.
  flows: []
  scope: phone
- description: Access the Salesforce identity URL service.
  flows: []
  scope: id
- description: Open a web session using the access token.
  flows: []
  scope: web
- description: Access Visualforce pages in the portal.
  flows: []
  scope: visualforce
- description: Access Lightning applications and components in the portal.
  flows: []
  scope: lightning
- description: Access Salesforce CMS and managed content.
  flows: []
  scope: content
- description: Access the Connect REST (Chatter) API.
  flows: []
  scope: chatter_api
- description: Include the user's custom permissions in the token response.
  flows: []
  scope: custom_permissions
- description: Access CRM Analytics (Wave) APIs.
  flows: []
  scope: wave_api
- description: Access CRM Analytics Eclair chart APIs.
  flows: []
  scope: eclair_api
- description: Access Account Engagement (Pardot) APIs.
  flows: []
  scope: pardot_api
- description: Access Salesforce Interaction (Next Best Action) APIs.
  flows: []
  scope: interaction_api
- description: Access Einstein Bots APIs.
  flows: []
  scope: chatbot_api
- description: Access Service Cloud real-time (Messaging) APIs.
  flows: []
  scope: scrt_api
- description: Access Salesforce platform AI (Models/Agentforce) APIs.
  flows: []
  scope: sfap_api
- description: Access Einstein GPT APIs.
  flows: []
  scope: einstein_gpt_api
- description: Access the Salesforce platform MCP API surface. Advertised by the portal discovery document; no MCP endpoint on either portal host answered anonymously.
  flows: []
  scope: mcp_api
- description: Access Data Cloud (CDP) APIs.
  flows: []
  scope: cdp_api
- description: Ingest records into Data Cloud.
  flows: []
  scope: cdp_ingest_api
- description: Query Data Cloud.
  flows: []
  scope: cdp_query_api
- description: Read Data Cloud unified profiles.
  flows: []
  scope: cdp_profile_api
- description: Manage Data Cloud segments.
  flows: []
  scope: cdp_segment_api
- description: Run Data Cloud identity resolution.
  flows: []
  scope: cdp_identityresolution_api
- description: Read Data Cloud calculated insights.
  flows: []
  scope: cdp_calculated_insight_api
- description: Include Data Cloud user claims in the token.
  flows: []
  scope: data_cloud_user_claims
- description: Self-registration API for portal users.
  flows: []
  scope: user_registration_api
- description: Passwordless login API for portal users.
  flows: []
  scope: pwdless_login_api
- description: Forgot-password API for portal users.
  flows: []
  scope: forgot_password
slug: blue-origin-scopes
source_filename: blue-origin-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: https://shop.blueorigin.com/.well-known/openid-configuration and\n  https://payloads.blueorigin.com/.well-known/openid-configuration\ndocs: null\nnote: >-\n  Blue Origin declares no API scopes anywhere it publishes — there is no OpenAPI, no\n  developer portal and no scopes/permissions reference page. Every scope below was read\n  from scopes_supported in an OIDC discovery document served anonymously by a vendor\n  platform bound to a blueorigin.com host. The shop scopes are Shopify customer-account\n  scopes; the portal scopes are the stock Salesforce platform scope catalogue, identical\n  on payloads.blueorigin.com and bodp.blueorigin.com because both communities sit on the\n  same Salesforce org. Neither set contains a Blue-Origin-specific resource scope (there\n  is no read:payloads, no launch:manifest). Treat these as platform scopes, not as a\n  product authorization model.\nschemes:\n- name: shopify-customer-account\n\
  \  source: well-known/blue-origin-shop-openid-configuration.json\n  issuer: https://shopify.com/authentication/30100881545\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/30100881545/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/30100881545/oauth/token\n- name: salesforce-experience-cloud\n  source: well-known/blue-origin-payloads-openid-configuration.json\n  issuer: https://payloads.blueorigin.com\n  also_served_by: https://bodp.blueorigin.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://payloads.blueorigin.com/services/oauth2/authorize\n    tokenUrl: https://payloads.blueorigin.com/services/oauth2/token\nscopes:\n- scope: openid\n  description: Issue an OIDC ID token for the authenticated end user.\n  schemes: [shopify-customer-account, salesforce-experience-cloud]\n  sources: [well-known/blue-origin-shop-openid-configuration.json, well-known/blue-origin-payloads-openid-configuration.json]\n\
  - scope: email\n  description: Release the end user's email address claim.\n  schemes: [shopify-customer-account, salesforce-experience-cloud]\n  sources: [well-known/blue-origin-shop-openid-configuration.json, well-known/blue-origin-payloads-openid-configuration.json]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API for the signed-in shopper\n    (orders, addresses, profile) on the Blue Origin Shop.\n  schemes: [shopify-customer-account]\n  sources: [well-known/blue-origin-shop-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: Full access to the customer-scoped MCP surface of the Blue Origin Shop —\n    the authenticated counterpart of the anonymous /api/mcp tools.\n  schemes: [shopify-customer-account]\n  sources: [well-known/blue-origin-shop-openid-configuration.json]\n- scope: api\n  description: Salesforce REST/SOAP/Bulk API access on behalf of the portal user.\n  schemes: [salesforce-experience-cloud]\n\
  \  sources: [well-known/blue-origin-payloads-openid-configuration.json]\n- scope: full\n  description: Full access to all data the portal user has access to.\n  schemes: [salesforce-experience-cloud]\n  sources: [well-known/blue-origin-payloads-openid-configuration.json]\n- scope: refresh_token\n  description: Issue a refresh token so the client can renew access without re-prompting.\n  schemes: [salesforce-experience-cloud]\n  sources: [well-known/blue-origin-payloads-openid-configuration.json]\n- scope: offline_access\n  description: Offline access — the OIDC alias of refresh_token.\n  schemes: [salesforce-experience-cloud]\n  sources: [well-known/blue-origin-payloads-openid-configuration.json]\n- scope: profile\n  description: Basic profile claims for the portal user.\n  schemes: [salesforce-experience-cloud]\n  sources: [well-known/blue-origin-payloads-openid-configuration.json]\n- scope: address\n  description: The end user's address claim.\n  schemes: [salesforce-experience-cloud]\n\
  \  sources: [well-known/blue-origin-payloads-openid-configuration.json]\n- scope: phone\n  description: The end user's phone number claim.\n  schemes: [salesforce-experience-cloud]\n  sources: [well-known/blue-origin-payloads-openid-configuration.json]\n- scope: id\n  description: Access the Salesforce identity URL service.\n  schemes: [salesforce-experience-cloud]\n  sources: [well-known/blue-origin-payloads-openid-configuration.json]\n- scope: web\n  description: Open a web session using the access token.\n  schemes: [salesforce-experience-cloud]\n  sources: [well-known/blue-origin-payloads-openid-configuration.json]\n- scope: visualforce\n  description: Access Visualforce pages in the portal.\n  schemes: [salesforce-experience-cloud]\n  sources: [well-known/blue-origin-payloads-openid-configuration.json]\n- scope: lightning\n  description: Access Lightning applications and components in the portal.\n  schemes: [salesforce-experience-cloud]\n  sources: [well-known/blue-origin-payloads-openid-configuration.json]\n\
  - scope: content\n  description: Access Salesforce CMS and managed content.\n  schemes: [salesforce-experience-cloud]\n  sources: [well-known/blue-origin-payloads-openid-configuration.json]\n- scope: chatter_api\n  description: Access the Connect REST (Chatter) API.\n  schemes: [salesforce-experience-cloud]\n  sources: [well-known/blue-origin-payloads-openid-configuration.json]\n- scope: custom_permissions\n  description: Include the user's custom permissions in the token response.\n  schemes: [salesforce-experience-cloud]\n  sources: [well-known/blue-origin-payloads-openid-configuration.json]\n- scope: wave_api\n  description: Access CRM Analytics (Wave) APIs.\n  schemes: [salesforce-experience-cloud]\n  sources: [well-known/blue-origin-payloads-openid-configuration.json]\n- scope: eclair_api\n  description: Access CRM Analytics Eclair chart APIs.\n  schemes: [salesforce-experience-cloud]\n  sources: [well-known/blue-origin-payloads-openid-configuration.json]\n- scope: pardot_api\n  description:\
  \ Access Account Engagement (Pardot) APIs.\n  schemes: [salesforce-experience-cloud]\n  sources: [well-known/blue-origin-payloads-openid-configuration.json]\n- scope: interaction_api\n  description: Access Salesforce Interaction (Next Best Action) APIs.\n  schemes: [salesforce-experience-cloud]\n  sources: [well-known/blue-origin-payloads-openid-configuration.json]\n- scope: chatbot_api\n  description: Access Einstein Bots APIs.\n  schemes: [salesforce-experience-cloud]\n  sources: [well-known/blue-origin-payloads-openid-configuration.json]\n- scope: scrt_api\n  description: Access Service Cloud real-time (Messaging) APIs.\n  schemes: [salesforce-experience-cloud]\n  sources: [well-known/blue-origin-payloads-openid-configuration.json]\n- scope: sfap_api\n  description: Access Salesforce platform AI (Models/Agentforce) APIs.\n  schemes: [salesforce-experience-cloud]\n  sources: [well-known/blue-origin-payloads-openid-configuration.json]\n- scope: einstein_gpt_api\n  description: Access\
  \ Einstein GPT APIs.\n  schemes: [salesforce-experience-cloud]\n  sources: [well-known/blue-origin-payloads-openid-configuration.json]\n- scope: mcp_api\n  description: Access the Salesforce platform MCP API surface. Advertised by the portal\n    discovery document; no MCP endpoint on either portal host answered anonymously.\n  schemes: [salesforce-experience-cloud]\n  sources: [well-known/blue-origin-payloads-openid-configuration.json]\n- scope: cdp_api\n  description: Access Data Cloud (CDP) APIs.\n  schemes: [salesforce-experience-cloud]\n  sources: [well-known/blue-origin-payloads-openid-configuration.json]\n- scope: cdp_ingest_api\n  description: Ingest records into Data Cloud.\n  schemes: [salesforce-experience-cloud]\n  sources: [well-known/blue-origin-payloads-openid-configuration.json]\n- scope: cdp_query_api\n  description: Query Data Cloud.\n  schemes: [salesforce-experience-cloud]\n  sources: [well-known/blue-origin-payloads-openid-configuration.json]\n- scope: cdp_profile_api\n\
  \  description: Read Data Cloud unified profiles.\n  schemes: [salesforce-experience-cloud]\n  sources: [well-known/blue-origin-payloads-openid-configuration.json]\n- scope: cdp_segment_api\n  description: Manage Data Cloud segments.\n  schemes: [salesforce-experience-cloud]\n  sources: [well-known/blue-origin-payloads-openid-configuration.json]\n- scope: cdp_identityresolution_api\n  description: Run Data Cloud identity resolution.\n  schemes: [salesforce-experience-cloud]\n  sources: [well-known/blue-origin-payloads-openid-configuration.json]\n- scope: cdp_calculated_insight_api\n  description: Read Data Cloud calculated insights.\n  schemes: [salesforce-experience-cloud]\n  sources: [well-known/blue-origin-payloads-openid-configuration.json]\n- scope: data_cloud_user_claims\n  description: Include Data Cloud user claims in the token.\n  schemes: [salesforce-experience-cloud]\n  sources: [well-known/blue-origin-payloads-openid-configuration.json]\n- scope: user_registration_api\n  description:\
  \ Self-registration API for portal users.\n  schemes: [salesforce-experience-cloud]\n  sources: [well-known/blue-origin-payloads-openid-configuration.json]\n- scope: pwdless_login_api\n  description: Passwordless login API for portal users.\n  schemes: [salesforce-experience-cloud]\n  sources: [well-known/blue-origin-payloads-openid-configuration.json]\n- scope: forgot_password\n  description: Forgot-password API for portal users.\n  schemes: [salesforce-experience-cloud]\n  sources: [well-known/blue-origin-payloads-openid-configuration.json]\nx-evidence:\n  fetched: '2026-08-02'\n  http_status: 200\n  shop_scopes: 4\n  salesforce_scopes: 35\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blue-origin/refs/heads/main/scopes/blue-origin-scopes.yml
summary_line: 38 scopes · authorizationCode
tags:
- Company
- Aerospace
- Space
- Spaceflight
- Launch Services
- Satellites
- Rocket Engines
- Defense
- Manufacturing
- E-commerce
- MCP
token_urls:
- https://shopify.com/authentication/30100881545/oauth/token
- https://payloads.blueorigin.com/services/oauth2/token
---
