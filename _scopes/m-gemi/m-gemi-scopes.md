---
authorization_urls: []
description: ''
docs: https://mgemi.com/.well-known/oauth-authorization-server
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: M Gemi Scopes
name_suffix: OAuth Scopes
note: Scopes are advertised by the Shopify Customer Account OIDC/RFC 8414 discovery documents served on M.Gemi's own store host for M.Gemi's shop tenant. M.Gemi publishes no scope reference page of its own; these are the values the server itself declares in scopes_supported.
overview: 'M.Gemi publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the M.Gemi API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: M.Gemi
provider_slug: m-gemi
schemes: []
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect sign-in; requests an ID token for the customer.
  flows: []
  scope: openid
- description: Access to the customer's email address and email_verified claim.
  flows: []
  scope: email
- description: Full access to the Shopify Customer Account API for the signed-in customer of the M.Gemi store.
  flows: []
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API for the signed-in customer - the authenticated counterpart to the anonymous UCP commerce MCP endpoint.
  flows: []
  scope: customer-account-mcp-api:full
slug: m-gemi-scopes
source_filename: m-gemi-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: https://mgemi.com/.well-known/openid-configuration\ndocs: https://mgemi.com/.well-known/oauth-authorization-server\nauthorization_server: https://shopify.com/authentication/13666484283\nnote: >-\n  Scopes are advertised by the Shopify Customer Account OIDC/RFC 8414 discovery documents\n  served on M.Gemi's own store host for M.Gemi's shop tenant. M.Gemi publishes no scope\n  reference page of its own; these are the values the server itself declares in\n  scopes_supported.\nscope_count: 4\nscopes:\n- name: openid\n  description: OpenID Connect sign-in; requests an ID token for the customer.\n- name: email\n  description: Access to the customer's email address and email_verified claim.\n- name: customer-account-api:full\n  description: Full access to the Shopify Customer Account API for the signed-in customer\n    of the M.Gemi store.\n- name: customer-account-mcp-api:full\n  description: Full access to the Shopify Customer Account\
  \ MCP API for the signed-in\n    customer - the authenticated counterpart to the anonymous UCP commerce MCP endpoint.\nclaims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/m-gemi/refs/heads/main/scopes/m-gemi-scopes.yml
summary_line: 4 scopes
tags:
- Company
- Retail
- E-Commerce
- Fashion
- Footwear
- Direct to Consumer
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- Shopify
- Catalog
- Checkout
token_bound: false
token_urls: []
---
