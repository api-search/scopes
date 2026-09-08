---
authorization_urls:
- https://account.3neyecare.com/authentication/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: 3Ntech Scopes
name_suffix: OAuth Scopes
note: Read from scopes_supported in the OpenID Connect discovery document the storefront serves. There is no OpenAPI in this repo to derive from, and 3N TECH publishes no scope reference page of its own — these are the Shopify Customer Account scopes advertised under 3N's host.
overview: '3N TECH publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the 3N TECH API on a user''s behalf.


  Tokens are issued from https://account.3neyecare.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: 3N TECH
provider_slug: 3ntech
schemes:
- flows:
  - authorizationUrl: https://account.3neyecare.com/authentication/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://account.3neyecare.com/authentication/oauth/token
  name: shopify-customer-account-oidc
  source: well-known/3ntech-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OpenID Connect scope; requests an ID token for the customer.
  flows:
  - authorizationCode
  scope: openid
- description: Releases the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the authenticated customer's account API surface (orders, addresses, profile).
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the customer-account MCP surface — an authenticated, per-customer MCP API distinct from the anonymous storefront UCP endpoint.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: 3ntech-scopes
source_filename: 3ntech-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: https://www.3neyecare.com/.well-known/openid-configuration\ndocs: null\nnote: >-\n  Read from scopes_supported in the OpenID Connect discovery document the storefront\n  serves. There is no OpenAPI in this repo to derive from, and 3N TECH publishes no\n  scope reference page of its own — these are the Shopify Customer Account scopes\n  advertised under 3N's host.\nschemes:\n- name: shopify-customer-account-oidc\n  source: well-known/3ntech-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.3neyecare.com/authentication/oauth/authorize\n    tokenUrl: https://account.3neyecare.com/authentication/oauth/token\n    pkce: S256\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope; requests an ID token for the customer.\n  flows: [authorizationCode]\n  sources: [well-known/3ntech-openid-configuration.json]\n- scope: email\n  description: Releases the customer's email\
  \ address and email_verified claim.\n  flows: [authorizationCode]\n  sources: [well-known/3ntech-openid-configuration.json]\n- scope: customer-account-api:full\n  description: Full access to the authenticated customer's account API surface (orders, addresses, profile).\n  flows: [authorizationCode]\n  sources: [well-known/3ntech-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: >-\n    Full access to the customer-account MCP surface — an authenticated, per-customer MCP\n    API distinct from the anonymous storefront UCP endpoint.\n  flows: [authorizationCode]\n  sources: [well-known/3ntech-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/3ntech/refs/heads/main/scopes/3ntech-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Eye Care
- Medical Devices
- Consumer Health
- Contact Lenses
- Ecommerce
- Agentic Commerce
- Universal Commerce Protocol
- Model Context Protocol
- Manufacturing
token_urls:
- https://account.3neyecare.com/authentication/oauth/token
---
