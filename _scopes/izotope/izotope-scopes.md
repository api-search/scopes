---
authorization_urls:
- https://account.izotope.com/authentication/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Izotope Scopes
name_suffix: OAuth Scopes
note: Read from the live OIDC/RFC 8414 discovery documents iZotope serves; there is no OpenAPI to derive from and iZotope publishes no human-readable scope reference page of its own. The scope vocabulary is Shopify's customer-accounts vocabulary as exposed by iZotope's tenant.
overview: 'iZotope publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the iZotope API on a user''s behalf.


  Tokens are issued from https://account.izotope.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: iZotope
provider_slug: izotope
schemes:
- flows:
  - authorizationUrl: https://account.izotope.com/authentication/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://account.izotope.com/authentication/oauth/token
  issuer: https://shopify.com/authentication/73782919339
  name: izotope-customer-accounts
  source: well-known/izotope-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect sign-in; issues an ID token for the customer account.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the customer account API for the signed-in iZotope customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the customer-account MCP API — the authenticated companion to the anonymous UCP commerce MCP endpoint at /api/ucp/mcp.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: izotope-scopes
source_filename: izotope-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://www.izotope.com/.well-known/openid-configuration\nnote: >-\n  Read from the live OIDC/RFC 8414 discovery documents iZotope serves; there is\n  no OpenAPI to derive from and iZotope publishes no human-readable scope\n  reference page of its own. The scope vocabulary is Shopify's customer-accounts\n  vocabulary as exposed by iZotope's tenant.\nschemes:\n  - name: izotope-customer-accounts\n    source: well-known/izotope-openid-configuration.json\n    issuer: https://shopify.com/authentication/73782919339\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://account.izotope.com/authentication/oauth/authorize\n        tokenUrl: https://account.izotope.com/authentication/oauth/token\n        pkce: S256\nscope_count: 4\nscopes:\n  - scope: openid\n    description: OpenID Connect sign-in; issues an ID token for the customer account.\n    flows: [authorizationCode]\n    sources: [well-known/izotope-openid-configuration.json]\n\
  \  - scope: email\n    description: Access to the customer's email address and email_verified claim.\n    flows: [authorizationCode]\n    sources: [well-known/izotope-openid-configuration.json]\n  - scope: 'customer-account-api:full'\n    description: Full access to the customer account API for the signed-in iZotope customer.\n    flows: [authorizationCode]\n    sources: [well-known/izotope-openid-configuration.json]\n  - scope: 'customer-account-mcp-api:full'\n    description: >-\n      Full access to the customer-account MCP API — the authenticated companion\n      to the anonymous UCP commerce MCP endpoint at /api/ucp/mcp.\n    flows: [authorizationCode]\n    sources: [well-known/izotope-openid-configuration.json]\nx-evidence:\n  fetched: '2026-08-12'\n  url: https://www.izotope.com/.well-known/openid-configuration\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/izotope/refs/heads/main/scopes/izotope-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Audio
- Audio Software
- Music Production
- Mixing
- Mastering
- Audio Restoration
- Audio Repair
- Post Production
- Plugins
- VST
- AudioUnit
- AAX
- DSP
- AI Audio
- Machine Learning Audio
- Vocal Processing
- Agent Commerce
- Universal Commerce Protocol
- Model Context Protocol
- Ecommerce
- Boris FX
token_urls:
- https://account.izotope.com/authentication/oauth/token
---
