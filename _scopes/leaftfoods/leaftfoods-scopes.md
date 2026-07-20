---
authorization_urls: []
description: OAuth 2.0 / OpenID Connect scopes advertised by the authorization server discovered from the Leaft Foods storefront host. The authorization server is Shopify's hosted customer-account issuer for shop 95682920744; the scope list below is taken verbatim from scopes_supported in the discovery document.
docs: https://www.leaftfoods.com/.well-known/oauth-authorization-server
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Leaftfoods Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Leaft Foods uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Leaft Foods
provider_slug: leaftfoods
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: leaftfoods-scopes
source_filename: leaftfoods-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.leaftfoods.com/.well-known/openid-configuration\ndocs: https://www.leaftfoods.com/.well-known/oauth-authorization-server\nname: Leaft Foods OAuth Scopes\ndescription: OAuth 2.0 / OpenID Connect scopes advertised by the authorization server discovered from the\n  Leaft Foods storefront host. The authorization server is Shopify's hosted customer-account issuer for\n  shop 95682920744; the scope list below is taken verbatim from scopes_supported in the discovery document.\nissuer: https://shopify.com/authentication/95682920744\nauthorization_endpoint: https://shopify.com/authentication/95682920744/oauth/authorize\ntoken_endpoint: https://shopify.com/authentication/95682920744/oauth/token\ncount: 4\nscopes:\n- name: openid\n  description: Standard OpenID Connect scope; requests an ID token identifying the signed-in customer.\n  standard: true\n- name: email\n  description: Standard OpenID Connect scope; releases the\
  \ email and email_verified claims.\n  standard: true\n- name: customer-account-api:full\n  description: Full access to the Customer Account API for the authenticated customer — orders, addresses,\n    profile and subscription data belonging to that customer.\n  standard: false\n- name: customer-account-mcp-api:full\n  description: Full access to the customer-account MCP surface, allowing an agent acting for a signed-in\n    customer to operate on that customer's account over MCP.\n  standard: false\nnotes:\n- The UCP storefront MCP endpoint at /api/ucp/mcp is a separate surface and is not gated by these scopes;\n  it gates on agent-profile discovery plus buyer approval at payment.\n- No Leaft Foods-specific (non-Shopify) scopes are published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leaftfoods/refs/heads/main/scopes/leaftfoods-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Food
- AgTech
- Alternative Protein
- Ingredients
- Pet Nutrition
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- Shopify
- New Zealand
token_urls: []
---
