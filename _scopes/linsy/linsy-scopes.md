---
authorization_urls: []
description: Scopes advertised by the Shopify customer-account OpenID Connect issuers behind Linsy's two storefronts. Both stores advertise the same set. Beyond the standard OIDC scopes, the issuer grants full access to the customer account API and to its MCP-flavored counterpart, which is what lets an agent act on an authenticated buyer's account.
docs: https://www.linsyhome.com/.well-known/openid-configuration
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Linsy Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Linsy uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Linsy
provider_slug: linsy
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: linsy-scopes
source_filename: linsy-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.linsyhome.com/.well-known/openid-configuration (scopes_supported)\nname: Linsy OAuth scopes\ndescription: Scopes advertised by the Shopify customer-account OpenID Connect issuers behind Linsy's two\n  storefronts. Both stores advertise the same set. Beyond the standard OIDC scopes, the issuer grants\n  full access to the customer account API and to its MCP-flavored counterpart, which is what lets an\n  agent act on an authenticated buyer's account.\ndocs: https://www.linsyhome.com/.well-known/openid-configuration\nissuers:\n- https://shopify.com/authentication/55555752076\n- https://shopify.com/authentication/73791996150\nscopes:\n- name: openid\n  description: Standard OpenID Connect scope; requests an ID token identifying the customer.\n- name: email\n  description: Releases the customer's email address and email_verified claim.\n- name: 'customer-account-api:full'\n  description: Full access to the Shopify Customer\
  \ Account API on behalf of the signed-in buyer —\n    orders, addresses, and profile.\n- name: 'customer-account-mcp-api:full'\n  description: Full access to the MCP-exposed Customer Account API, the authenticated counterpart of the\n    anonymous UCP commerce endpoint.\ncount: 4\nnotes:\n- Scopes are issued by Shopify for the shop, not defined by Linsy; Linsy publishes no scope reference\n  page of its own.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linsy/refs/heads/main/scopes/linsy-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Consumer
- Retail
- E-Commerce
- Furniture
- Home Goods
- Direct To Consumer
- Agentic Commerce
- Shopify
- MCP
token_urls: []
---
