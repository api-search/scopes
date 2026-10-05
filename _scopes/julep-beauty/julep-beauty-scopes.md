---
api_specs:
- filename: julep-beauty-cart-api-openapi.yml
  format: yaml
  label: Julep Beauty Cart API
  slug: julep-beauty-cart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/julep-beauty/refs/heads/main/openapi/julep-beauty-cart-api-openapi.yml
- filename: julep-beauty-discovery-api-openapi.yml
  format: yaml
  label: Julep Beauty Discovery API
  slug: julep-beauty-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/julep-beauty/refs/heads/main/openapi/julep-beauty-discovery-api-openapi.yml
- filename: julep-beauty-search-api-openapi.yml
  format: yaml
  label: Julep Beauty Search API
  slug: julep-beauty-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/julep-beauty/refs/heads/main/openapi/julep-beauty-search-api-openapi.yml
authorization_urls:
- https://account.julep.com/authentication/oauth/authorize
description: Scopes advertised by the OpenID Connect / OAuth authorization-server metadata served on Julep's own domain for its Shopify Customer Accounts deployment. Captured verbatim from scopes_supported; Julep publishes no separate scope reference page, so no descriptions beyond the standard OIDC meanings and the Shopify Customer Account API naming are asserted here.
docs: ''
flows:
- authorization_code
- refresh_token
- urn:ietf:params:oauth:grant-type:jwt-bearer
kind: oauth-scopes
layout: scope
method: searched
name: Julep Beauty Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Julep Beauty publishes 4 OAuth 2.0 scopes via the authorization_code, refresh_token, and urn:ietf:params:oauth:grant-type:jwt-bearer flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Julep Beauty API on a user''s behalf.


  Tokens are issued from https://account.julep.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Julep Beauty
provider_slug: julep-beauty
schemes: []
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OpenID Connect scope requesting an ID token for the signed-in customer.
  flows: []
  scope: openid
- description: Standard OpenID Connect scope releasing the email and email_verified claims.
  flows: []
  scope: email
- description: Full access to the customer-account surface on behalf of the signed-in customer. Named by the discovery document; Julep publishes no finer-grained breakdown.
  flows: []
  scope: customer-account-api:full
- description: Full access to the customer-account surface over the MCP transport, for agents acting on behalf of the signed-in customer.
  flows: []
  scope: customer-account-mcp-api:full
slug: julep-beauty-scopes
source_filename: julep-beauty-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.julep.com/.well-known/openid-configuration\nname: Julep customer-account OAuth scopes\ndescription: >-\n  Scopes advertised by the OpenID Connect / OAuth authorization-server metadata served on\n  Julep's own domain for its Shopify Customer Accounts deployment. Captured verbatim from\n  scopes_supported; Julep publishes no separate scope reference page, so no descriptions\n  beyond the standard OIDC meanings and the Shopify Customer Account API naming are\n  asserted here.\nissuer: https://shopify.com/authentication/2228781091\nauthorization_endpoint: https://account.julep.com/authentication/oauth/authorize\ntoken_endpoint: https://account.julep.com/authentication/oauth/token\nflows:\n- authorization_code\n- refresh_token\n- 'urn:ietf:params:oauth:grant-type:jwt-bearer'\npkce: S256\ndocs: null\ndocs_note: >-\n  No provider-published scope/permission reference page was found on www.julep.com; the\n  authoritative\
  \ list below is the discovery document itself.\nscopes:\n- name: openid\n  description: Standard OpenID Connect scope requesting an ID token for the signed-in customer.\n  standard: true\n- name: email\n  description: Standard OpenID Connect scope releasing the email and email_verified claims.\n  standard: true\n- name: 'customer-account-api:full'\n  description: >-\n    Full access to the customer-account surface on behalf of the signed-in customer.\n    Named by the discovery document; Julep publishes no finer-grained breakdown.\n  standard: false\n- name: 'customer-account-mcp-api:full'\n  description: >-\n    Full access to the customer-account surface over the MCP transport, for agents acting\n    on behalf of the signed-in customer.\n  standard: false\nclaims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/julep-beauty/refs/heads/main/scopes/julep-beauty-scopes.yml
summary_line: 4 scopes · authorization_code/refresh_token/urn:ietf:params:oauth:grant-type:jwt-bearer
tags:
- Company
- Beauty
- Cosmetics
- Skincare
- Retail
- E-Commerce
- Direct to Consumer
- Shopify
- Agentic Commerce
- Universal Commerce Protocol
token_bound: false
token_urls:
- https://account.julep.com/authentication/oauth/token
---
