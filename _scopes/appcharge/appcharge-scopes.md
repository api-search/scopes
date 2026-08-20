---
api_specs:
- filename: appcharge-assets-api-openapi.yml
  format: yaml
  label: Appcharge Assets API
  slug: appcharge-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/openapi/appcharge-assets-api-openapi.yml
- filename: appcharge-authentication-api-openapi.yml
  format: yaml
  label: Appcharge Authentication API
  slug: appcharge-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/openapi/appcharge-authentication-api-openapi.yml
- filename: appcharge-badges-api-openapi.yml
  format: yaml
  label: Appcharge Badges API
  slug: appcharge-badges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/openapi/appcharge-badges-api-openapi.yml
- filename: appcharge-coupons-api-openapi.yml
  format: yaml
  label: Appcharge Coupons API
  slug: appcharge-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/openapi/appcharge-coupons-api-openapi.yml
- filename: appcharge-general-api-openapi.yml
  format: yaml
  label: Appcharge General API
  slug: appcharge-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/openapi/appcharge-general-api-openapi.yml
- filename: appcharge-localization-api-openapi.yml
  format: yaml
  label: Appcharge Localization API
  slug: appcharge-localization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/openapi/appcharge-localization-api-openapi.yml
- filename: appcharge-offer-designs-api-openapi.yml
  format: yaml
  label: Appcharge Offer Designs API
  slug: appcharge-offer-designs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/openapi/appcharge-offer-designs-api-openapi.yml
- filename: appcharge-offers-api-openapi.yml
  format: yaml
  label: Appcharge Offers API
  slug: appcharge-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/openapi/appcharge-offers-api-openapi.yml
- filename: appcharge-orders-api-openapi.yml
  format: yaml
  label: Appcharge Orders API
  slug: appcharge-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/openapi/appcharge-orders-api-openapi.yml
- filename: appcharge-personalization-api-openapi.yml
  format: yaml
  label: Appcharge Personalization API
  slug: appcharge-personalization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/openapi/appcharge-personalization-api-openapi.yml
- filename: appcharge-popups-api-openapi.yml
  format: yaml
  label: Appcharge Popups API
  slug: appcharge-popups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/openapi/appcharge-popups-api-openapi.yml
- filename: appcharge-portal-content-api-openapi.yml
  format: yaml
  label: Appcharge Portal Content API
  slug: appcharge-portal-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/openapi/appcharge-portal-content-api-openapi.yml
- filename: appcharge-products-api-openapi.yml
  format: yaml
  label: Appcharge Products API
  slug: appcharge-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/openapi/appcharge-products-api-openapi.yml
- filename: appcharge-promo-codes-api-openapi.yml
  format: yaml
  label: Appcharge Promo Codes API
  slug: appcharge-promo-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/openapi/appcharge-promo-codes-api-openapi.yml
- filename: appcharge-rolling-offers-api-openapi.yml
  format: yaml
  label: Appcharge Rolling Offers API
  slug: appcharge-rolling-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/openapi/appcharge-rolling-offers-api-openapi.yml
- filename: appcharge-store-refresh-popups-api-openapi.yml
  format: yaml
  label: Appcharge Store Refresh Popups API
  slug: appcharge-store-refresh-popups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/openapi/appcharge-store-refresh-popups-api-openapi.yml
- filename: appcharge-triggered-popups-api-openapi.yml
  format: yaml
  label: Appcharge Triggered Popups API
  slug: appcharge-triggered-popups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/openapi/appcharge-triggered-popups-api-openapi.yml
authorization_urls:
- https://api.appcharge.com/oauth/authorize
description: 'OAuth 2.0 scopes published by Appcharge''s authorization server (RFC 8414). These scopes gate the hosted MCP server (mcp.appcharge.com); the publisher REST API itself authenticates with the x-publisher-token API key (see authentication/). Flow: authorization_code with PKCE (S256) and dynamic client registration; token_endpoint_auth_methods_supported = [none] (public clients).'
docs: https://mcp.appcharge.com/.well-known/oauth-protected-resource
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Appcharge Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Appcharge publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Appcharge API on a user''s behalf.


  Tokens are issued from https://api.appcharge.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Appcharge
provider_slug: appcharge
schemes:
- flows:
  - authorizationUrl: https://api.appcharge.com/oauth/authorize
    flow: authorizationCode
    jwksUri: https://api.appcharge.com/.well-known/jwks-oauth.json
    pkce:
    - S256
    registrationUrl: https://api.appcharge.com/oauth/register
    tokenUrl: https://api.appcharge.com/oauth/token
  issuer: https://api.appcharge.com
  name: OAuth2
  source: https://api.appcharge.com/.well-known/oauth-authorization-server
scope_count: 2
scope_names:
- mcp:read
- mcp:write
scopes:
- description: Read access via the Appcharge MCP server.
  flows:
  - authorizationCode
  scope: mcp:read
- description: Write access via the Appcharge MCP server.
  flows:
  - authorizationCode
  scope: mcp:write
slug: appcharge-scopes
source_filename: appcharge-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://api.appcharge.com/.well-known/oauth-authorization-server\ndocs: https://mcp.appcharge.com/.well-known/oauth-protected-resource\ndescription: >-\n  OAuth 2.0 scopes published by Appcharge's authorization server (RFC 8414).\n  These scopes gate the hosted MCP server (mcp.appcharge.com); the publisher\n  REST API itself authenticates with the x-publisher-token API key (see\n  authentication/). Flow: authorization_code with PKCE (S256) and dynamic\n  client registration; token_endpoint_auth_methods_supported = [none] (public\n  clients).\nschemes:\n  - name: OAuth2\n    source: https://api.appcharge.com/.well-known/oauth-authorization-server\n    issuer: https://api.appcharge.com\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://api.appcharge.com/oauth/authorize\n        tokenUrl: https://api.appcharge.com/oauth/token\n        registrationUrl: https://api.appcharge.com/oauth/register\n    \
  \    jwksUri: https://api.appcharge.com/.well-known/jwks-oauth.json\n        pkce: [S256]\nscopes:\n  - scope: mcp:read\n    description: Read access via the Appcharge MCP server.\n    flows: [authorizationCode]\n    sources: [https://api.appcharge.com/.well-known/oauth-authorization-server]\n  - scope: mcp:write\n    description: Write access via the Appcharge MCP server.\n    flows: [authorizationCode]\n    sources: [https://api.appcharge.com/.well-known/oauth-authorization-server]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/scopes/appcharge-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Payments
- Monetization
- Merchant of Record
- Mobile Games
- Gaming
- Checkout
- In-Game Purchases
- Web Store
- E-Commerce
token_urls:
- https://api.appcharge.com/oauth/token
---
