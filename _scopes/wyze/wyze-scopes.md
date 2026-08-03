---
authorization_urls:
- https://account.wyze.com/authentication/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
- refreshToken
kind: oauth-scopes
layout: scope
method: searched
name: Wyze Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Wyze publishes 4 OAuth 2.0 scopes via the authorizationCode and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Wyze API on a user''s behalf.


  Tokens are issued from https://account.wyze.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Wyze
provider_slug: wyze
schemes:
- flows:
  - authorizationUrl: https://account.wyze.com/authentication/oauth/authorize
    flow: authorizationCode
    pkce:
    - S256
    tokenUrl: https://account.wyze.com/authentication/oauth/token
  - flow: refreshToken
    tokenUrl: https://account.wyze.com/authentication/oauth/token
  issuer: https://shopify.com/authentication/58004504738
  name: WyzeCustomerAccountOIDC
  source: well-known/wyze-openid-configuration.json
  type: openIdConnect
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OpenID Connect scope; requests an ID token asserting the subject of the authenticated Wyze customer account.
  flows:
  - authorizationCode
  scope: openid
- description: Releases the email and email_verified claims for the authenticated customer account.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the signed-in Wyze customer - orders, addresses, payment methods and profile.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the customer-account MCP surface at https://account.wyze.com/customer/api/mcp - order status, store credit balances and return requests on behalf of the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: wyze-scopes
source_filename: wyze-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://www.wyze.com/.well-known/openid-configuration\nfile: well-known/wyze-openid-configuration.json\nnotes: >-\n  Wyze publishes no OpenAPI, so no scopes could be derived from a spec. The scopes below\n  are the complete scopes_supported list published in the OIDC discovery document served\n  from the wyze.com origin for Shopify-backed Wyze customer accounts. The Wyze device\n  /cloud API (api.wyzecam.com) is API-key + bearer-token based and has NO scope surface -\n  it is intentionally absent here rather than represented with invented scopes.\nschemes:\n- name: WyzeCustomerAccountOIDC\n  type: openIdConnect\n  issuer: https://shopify.com/authentication/58004504738\n  source: well-known/wyze-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.wyze.com/authentication/oauth/authorize\n    tokenUrl: https://account.wyze.com/authentication/oauth/token\n    pkce: [S256]\n  -\
  \ flow: refreshToken\n    tokenUrl: https://account.wyze.com/authentication/oauth/token\nscopes:\n- scope: openid\n  description: >-\n    Standard OpenID Connect scope; requests an ID token asserting the subject of the\n    authenticated Wyze customer account.\n  flows: [authorizationCode]\n  sources: [well-known/wyze-openid-configuration.json]\n- scope: email\n  description: >-\n    Releases the email and email_verified claims for the authenticated customer account.\n  flows: [authorizationCode]\n  sources: [well-known/wyze-openid-configuration.json]\n- scope: customer-account-api:full\n  description: >-\n    Full access to the Shopify Customer Account API for the signed-in Wyze customer -\n    orders, addresses, payment methods and profile.\n  flows: [authorizationCode]\n  sources: [well-known/wyze-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: >-\n    Full access to the customer-account MCP surface at\n    https://account.wyze.com/customer/api/mcp\
  \ - order status, store credit balances and\n    return requests on behalf of the signed-in customer.\n  flows: [authorizationCode]\n  sources: [well-known/wyze-openid-configuration.json]\nclaims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wyze/refs/heads/main/scopes/wyze-scopes.yml
summary_line: 4 scopes · authorizationCode/refreshToken
tags:
- Company
- Smart Home
- Internet of Things
- Home Security
- Cameras
- Consumer Electronics
- Home Automation
- Video
- Sensors
- Commerce
token_urls:
- https://account.wyze.com/authentication/oauth/token
---
