---
api_specs:
- filename: julep-beauty-storefront-openapi.yml
  format: yaml
  label: Julep Storefront Read-Only JSON API
  slug: storefront
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/julep-beauty/refs/heads/main/openapi/julep-beauty-storefront-openapi.yml
authorization_urls: []
description: Scopes advertised by the OpenID Connect / OAuth authorization-server metadata served on Julep's own domain for its Shopify Customer Accounts deployment. Captured verbatim from scopes_supported; Julep publishes no separate scope reference page, so no descriptions beyond the standard OIDC meanings and the Shopify Customer Account API naming are asserted here.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Julep Beauty Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Julep Beauty uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Julep Beauty
provider_slug: julep-beauty
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: julep-beauty-scopes
source_filename: julep-beauty-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.julep.com/.well-known/openid-configuration\nname: Julep customer-account OAuth scopes\ndescription: >-\n  Scopes advertised by the OpenID Connect / OAuth authorization-server metadata served on\n  Julep's own domain for its Shopify Customer Accounts deployment. Captured verbatim from\n  scopes_supported; Julep publishes no separate scope reference page, so no descriptions\n  beyond the standard OIDC meanings and the Shopify Customer Account API naming are\n  asserted here.\nissuer: https://shopify.com/authentication/2228781091\nauthorization_endpoint: https://account.julep.com/authentication/oauth/authorize\ntoken_endpoint: https://account.julep.com/authentication/oauth/token\nflows:\n- authorization_code\n- refresh_token\n- 'urn:ietf:params:oauth:grant-type:jwt-bearer'\npkce: S256\ndocs: null\ndocs_note: >-\n  No provider-published scope/permission reference page was found on www.julep.com; the\n  authoritative\
  \ list below is the discovery document itself.\nscopes:\n- name: openid\n  description: Standard OpenID Connect scope requesting an ID token for the signed-in customer.\n  standard: true\n- name: email\n  description: Standard OpenID Connect scope releasing the email and email_verified claims.\n  standard: true\n- name: 'customer-account-api:full'\n  description: >-\n    Full access to the customer-account surface on behalf of the signed-in customer.\n    Named by the discovery document; Julep publishes no finer-grained breakdown.\n  standard: false\n- name: 'customer-account-mcp-api:full'\n  description: >-\n    Full access to the customer-account surface over the MCP transport, for agents acting\n    on behalf of the signed-in customer.\n  standard: false\nclaims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/julep-beauty/refs/heads/main/scopes/julep-beauty-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
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
token_urls: []
---
