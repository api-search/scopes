---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Agrovision Scopes
name_suffix: OAuth Scopes
note: The anonymous UCP MCP endpoint at /api/ucp/mcp requires none of these scopes for catalog, cart or checkout construction; they gate shopper-identity-bound operations only.
overview: 'Agrovision uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Agrovision
provider_slug: agrovision
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: agrovision-scopes
source_filename: agrovision-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: https://shop.fruitist.com/.well-known/openid-configuration\naid: agrovision-ucp-commerce\nprovider_of_record: >-\n  Shopify customer-account authorization server for this store's tenant\n  (issuer https://shopify.com/authentication/64996540577). Agrovision does not define or\n  document scopes of its own; these are read verbatim from scopes_supported in the discovery\n  document served on its storefront host.\nscope_count: 4\nscopes:\n- name: openid\n  description: Standard OpenID Connect scope requesting an ID token for the signed-in shopper.\n- name: email\n  description: Releases the shopper's email address and email_verified claim.\n- name: customer-account-api:full\n  description: >-\n    Full access to the Shopify Customer Account API for the authenticated shopper — orders,\n    addresses, payment methods and profile on this store.\n- name: customer-account-mcp-api:full\n  description: >-\n    Full access to the customer-account\
  \ MCP API for the authenticated shopper, i.e. the\n    authenticated counterpart of the anonymous UCP commerce MCP endpoint.\nclaims_supported:\n- iss\n- sub\n- aud\n- exp\n- iat\n- nonce\n- sid\n- email\n- email_verified\nnote: >-\n  The anonymous UCP MCP endpoint at /api/ucp/mcp requires none of these scopes for catalog,\n  cart or checkout construction; they gate shopper-identity-bound operations only.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agrovision/refs/heads/main/scopes/agrovision-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Agriculture
- Food and Beverage
- Consumer Packaged Goods
- AgTech
- E-Commerce
- Retail
- Supply Chain
- Agentic Commerce
- Universal Commerce Protocol
token_urls: []
---
