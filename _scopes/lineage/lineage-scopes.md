---
authorization_urls:
- https://lineage-ciam.us.auth0.com/authorize
- https://lineagelinkhelp.onelineage.com/support/services/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
- deviceCode
kind: oauth-scopes
layout: scope
method: searched
name: Lineage Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Lineage publishes 21 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Lineage API on a user''s behalf.


  Tokens are issued from https://lineage-ciam.us.auth0.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Lineage
provider_slug: lineage
schemes:
- flows:
  - authorizationUrl: https://lineage-ciam.us.auth0.com/authorize
    flow: authorizationCode
    tokenUrl: https://lineage-ciam.us.auth0.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://lineage-ciam.us.auth0.com/oauth/token
  - deviceAuthorizationUrl: https://lineage-ciam.us.auth0.com/oauth/device/code
    flow: deviceCode
    tokenUrl: https://lineage-ciam.us.auth0.com/oauth/token
  issuer: https://lineage-ciam.us.auth0.com/
  name: LineageLinkCIAM
  provider: Auth0
  source: well-known/lineage-ciam-openid-configuration.json
- flows:
  - authorizationUrl: https://lineagelinkhelp.onelineage.com/support/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://lineagelinkhelp.onelineage.com/support/services/oauth2/token
  issuer: https://lineagelinkhelp.onelineage.com/support
  name: LineageLinkHelpCommunity
  provider: Salesforce Experience Cloud
  source: well-known/lineage-linkhelp-openid-configuration.json
scope_count: 21
scope_names:
- openid
- profile
- email
- phone
- address
- offline_access
- name
- given_name
- family_name
- nickname
- email_verified
- picture
- created_at
- identities
- api
- full
- id
- refresh_token
- web
- chatter_api
- custom_permissions
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
- description: Phone number claim.
  flows: []
  scope: phone
- description: Address claim.
  flows: []
  scope: address
- description: Issue a refresh token for long-lived access.
  flows: []
  scope: offline_access
- description: Full name claim (Auth0 tenant).
  flows: []
  scope: name
- description: Given name claim (Auth0 tenant).
  flows: []
  scope: given_name
- description: Family name claim (Auth0 tenant).
  flows: []
  scope: family_name
- description: Nickname claim (Auth0 tenant).
  flows: []
  scope: nickname
- description: Email verification status claim (Auth0 tenant).
  flows: []
  scope: email_verified
- description: Profile picture claim (Auth0 tenant).
  flows: []
  scope: picture
- description: Account creation timestamp claim (Auth0 tenant).
  flows: []
  scope: created_at
- description: Linked identity providers claim (Auth0 tenant).
  flows: []
  scope: identities
- description: Salesforce platform API access (Experience Cloud default).
  flows: []
  scope: api
- description: Full Salesforce platform access (Experience Cloud default).
  flows: []
  scope: full
- description: Salesforce identity URL access.
  flows: []
  scope: id
- description: Salesforce refresh token issuance.
  flows: []
  scope: refresh_token
- description: Salesforce web session access.
  flows: []
  scope: web
- description: Salesforce Chatter/Connect REST API access.
  flows: []
  scope: chatter_api
- description: Custom permission claims in the token.
  flows: []
  scope: custom_permissions
slug: lineage-scopes
source_filename: lineage-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: >-\n  scopes_supported advertised by the OIDC discovery documents at\n  https://lineage-ciam.us.auth0.com/.well-known/openid-configuration and\n  https://lineagelinkhelp.onelineage.com/.well-known/openid-configuration\n  (fetched 2026-07-19)\ncaveat: >-\n  Lineage publishes no scopes/permissions reference page and no public API. Every\n  scope below is the PLATFORM DEFAULT advertised by the underlying identity vendor\n  (Auth0 for the Lineage Link CIAM tenant, Salesforce Experience Cloud for the\n  Lineage Link Help community) — none is a Lineage-authored, product-specific\n  scope. Recorded as observed discovery data, not as a documented Lineage\n  authorization model.\ndocs: null\nschemes:\n- name: LineageLinkCIAM\n  provider: Auth0\n  issuer: https://lineage-ciam.us.auth0.com/\n  source: well-known/lineage-ciam-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://lineage-ciam.us.auth0.com/authorize\n\
  \    tokenUrl: https://lineage-ciam.us.auth0.com/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://lineage-ciam.us.auth0.com/oauth/token\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://lineage-ciam.us.auth0.com/oauth/device/code\n    tokenUrl: https://lineage-ciam.us.auth0.com/oauth/token\n- name: LineageLinkHelpCommunity\n  provider: Salesforce Experience Cloud\n  issuer: https://lineagelinkhelp.onelineage.com/support\n  source: well-known/lineage-linkhelp-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://lineagelinkhelp.onelineage.com/support/services/oauth2/authorize\n    tokenUrl: https://lineagelinkhelp.onelineage.com/support/services/oauth2/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; returns an ID token.\n  standard: true\n  schemes: [LineageLinkCIAM, LineageLinkHelpCommunity]\n- scope: profile\n  description: Basic profile claims for the authenticated user.\n  standard: true\n\
  \  schemes: [LineageLinkCIAM, LineageLinkHelpCommunity]\n- scope: email\n  description: Email address claim.\n  standard: true\n  schemes: [LineageLinkCIAM, LineageLinkHelpCommunity]\n- scope: phone\n  description: Phone number claim.\n  standard: true\n  schemes: [LineageLinkCIAM, LineageLinkHelpCommunity]\n- scope: address\n  description: Address claim.\n  standard: true\n  schemes: [LineageLinkCIAM, LineageLinkHelpCommunity]\n- scope: offline_access\n  description: Issue a refresh token for long-lived access.\n  standard: true\n  schemes: [LineageLinkCIAM, LineageLinkHelpCommunity]\n- scope: name\n  description: Full name claim (Auth0 tenant).\n  schemes: [LineageLinkCIAM]\n- scope: given_name\n  description: Given name claim (Auth0 tenant).\n  schemes: [LineageLinkCIAM]\n- scope: family_name\n  description: Family name claim (Auth0 tenant).\n  schemes: [LineageLinkCIAM]\n- scope: nickname\n  description: Nickname claim (Auth0 tenant).\n  schemes: [LineageLinkCIAM]\n- scope: email_verified\n\
  \  description: Email verification status claim (Auth0 tenant).\n  schemes: [LineageLinkCIAM]\n- scope: picture\n  description: Profile picture claim (Auth0 tenant).\n  schemes: [LineageLinkCIAM]\n- scope: created_at\n  description: Account creation timestamp claim (Auth0 tenant).\n  schemes: [LineageLinkCIAM]\n- scope: identities\n  description: Linked identity providers claim (Auth0 tenant).\n  schemes: [LineageLinkCIAM]\n- scope: api\n  description: Salesforce platform API access (Experience Cloud default).\n  vendor_default: true\n  schemes: [LineageLinkHelpCommunity]\n- scope: full\n  description: Full Salesforce platform access (Experience Cloud default).\n  vendor_default: true\n  schemes: [LineageLinkHelpCommunity]\n- scope: id\n  description: Salesforce identity URL access.\n  vendor_default: true\n  schemes: [LineageLinkHelpCommunity]\n- scope: refresh_token\n  description: Salesforce refresh token issuance.\n  vendor_default: true\n  schemes: [LineageLinkHelpCommunity]\n- scope:\
  \ web\n  description: Salesforce web session access.\n  vendor_default: true\n  schemes: [LineageLinkHelpCommunity]\n- scope: chatter_api\n  description: Salesforce Chatter/Connect REST API access.\n  vendor_default: true\n  schemes: [LineageLinkHelpCommunity]\n- scope: custom_permissions\n  description: Custom permission claims in the token.\n  vendor_default: true\n  schemes: [LineageLinkHelpCommunity]\nvendor_default_scopes_not_enumerated:\n  note: >-\n    The Salesforce Experience Cloud discovery document additionally advertises the\n    stock Salesforce platform scope set (cdp_* Data Cloud scopes, einstein_gpt_api,\n    sfap_api, mcp_api, wave_api, eclair_api, pardot_api, lightning, visualforce,\n    content, interaction_api, chatbot_api, scrt_api, data_cloud_user_claims,\n    user_registration_api, pwdless_login_api, forgot_password). These are Salesforce\n    platform defaults present on every Experience Cloud site and carry no\n    Lineage-specific meaning; they are recorded here\
  \ rather than listed as Lineage\n    scopes.\n  source: well-known/lineage-linkhelp-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lineage/refs/heads/main/scopes/lineage-scopes.yml
summary_line: 21 scopes · authorizationCode/clientCredentials/deviceCode
tags:
- Company
- Logistics
- Cold Chain
- Warehousing
- Supply Chain
- Temperature Controlled
- Freight
- Transportation
- Food and Beverage
- REIT
token_urls:
- https://lineage-ciam.us.auth0.com/oauth/token
- https://lineagelinkhelp.onelineage.com/support/services/oauth2/token
---
