---
api_specs:
- filename: also-storefront-json-openapi.yml
  format: yaml
  label: ALSO Storefront JSON API
  slug: also-storefront-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/also/refs/heads/main/openapi/also-storefront-json-openapi.yml
authorization_urls:
- https://shopify.com/authentication/74758783200/oauth/authorize
- https://idp.ridealso.com/oauth2/authorize
description: ''
docs: https://ridealso.com/.well-known/oauth-authorization-server
flows:
- authorizationCode
- refreshToken
- urn:ietf:params:oauth:grant-type:jwt-bearer
kind: oauth-scopes
layout: scope
method: searched
name: Also Scopes
name_suffix: OAuth Scopes
note: Scopes are published live in ALSO's own OIDC / RFC 8414 discovery documents at ridealso.com. No OpenAPI on this provider declares oauth2 security schemes, so these were harvested from the discovery surface rather than derived from a spec.
overview: 'Also publishes 5 OAuth 2.0 scopes via the authorizationCode, refreshToken, and urn:ietf:params:oauth:grant-type:jwt-bearer flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Also API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/74758783200/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Also
provider_slug: also
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/74758783200/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/74758783200/oauth/token
  - flow: refreshToken
    tokenUrl: https://shopify.com/authentication/74758783200/oauth/token
  - flow: urn:ietf:params:oauth:grant-type:jwt-bearer
    tokenUrl: https://shopify.com/authentication/74758783200/oauth/token
  issuer: https://shopify.com/authentication/74758783200
  name: shopify-customer-accounts
  source: well-known/also-openid-configuration.json
- flows:
  - authorizationUrl: https://idp.ridealso.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://idp.ridealso.com/oauth2/token
  name: also-idp
  source: https://ridealso.com/ (login links)
scope_count: 5
scope_names:
- openid
- email
- profile
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Issue an OpenID Connect ID token for the signed-in customer.
  flows:
  - authorizationCode
  scope: openid
- description: Release the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Release basic profile claims. Requested by the ALSO idp.ridealso.com social sign-in links.
  flows:
  - authorizationCode
  scope: profile
- description: Full access to the Shopify Customer Account API on behalf of the signed-in customer - orders, addresses, profile and subscriptions.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API - the agent-facing projection of the customer account surface. Notable as an explicitly agent-scoped OAuth scope.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: also-scopes
source_filename: also-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://ridealso.com/.well-known/openid-configuration\ndocs: https://ridealso.com/.well-known/oauth-authorization-server\nnote: Scopes are published live in ALSO's own OIDC / RFC 8414 discovery documents at\n  ridealso.com. No OpenAPI on this provider declares oauth2 security schemes, so these\n  were harvested from the discovery surface rather than derived from a spec.\nschemes:\n- name: shopify-customer-accounts\n  source: well-known/also-openid-configuration.json\n  issuer: https://shopify.com/authentication/74758783200\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/74758783200/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/74758783200/oauth/token\n  - flow: refreshToken\n    tokenUrl: https://shopify.com/authentication/74758783200/oauth/token\n  - flow: 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n    tokenUrl: https://shopify.com/authentication/74758783200/oauth/token\n\
  - name: also-idp\n  source: 'https://ridealso.com/ (login links)'\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://idp.ridealso.com/oauth2/authorize\n    tokenUrl: https://idp.ridealso.com/oauth2/token\nscopes:\n- scope: openid\n  description: Issue an OpenID Connect ID token for the signed-in customer.\n  flows: [authorizationCode]\n  sources: [well-known/also-openid-configuration.json, 'https://ridealso.com/']\n- scope: email\n  description: Release the customer's email address and email_verified claim.\n  flows: [authorizationCode]\n  sources: [well-known/also-openid-configuration.json, 'https://ridealso.com/']\n- scope: profile\n  description: Release basic profile claims. Requested by the ALSO idp.ridealso.com\n    social sign-in links.\n  flows: [authorizationCode]\n  sources: ['https://ridealso.com/']\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API on behalf of the signed-in\n    customer - orders, addresses,\
  \ profile and subscriptions.\n  flows: [authorizationCode]\n  sources: [well-known/also-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: Full access to the Customer Account MCP API - the agent-facing projection\n    of the customer account surface. Notable as an explicitly agent-scoped OAuth scope.\n  flows: [authorizationCode]\n  sources: [well-known/also-openid-configuration.json]\nclaims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/also/refs/heads/main/scopes/also-scopes.yml
summary_line: 5 scopes · authorizationCode/refreshToken/urn:ietf:params:oauth:grant-type:jwt-bearer
tags:
- Company
- Micromobility
- Electric Vehicles
- Transportation
- E-Commerce
- Consumer Hardware
- Agentic Commerce
- Logistics
- Delivery
token_urls:
- https://shopify.com/authentication/74758783200/oauth/token
- https://idp.ridealso.com/oauth2/token
---
