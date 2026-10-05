---
authorization_urls:
- https://shopify.com/authentication/95682920744/oauth/authorize
description: OAuth 2.0 / OpenID Connect scopes advertised by the authorization server discovered from the Leaft Foods storefront host. The authorization server is Shopify's hosted customer-account issuer for shop 95682920744; the scope list below is taken verbatim from scopes_supported in the discovery document.
docs: https://www.leaftfoods.com/.well-known/oauth-authorization-server
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Leaftfoods Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Leaft Foods publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Leaft Foods API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/95682920744/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Leaft Foods
provider_slug: leaftfoods
schemes: []
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OpenID Connect scope; requests an ID token identifying the signed-in customer.
  flows: []
  scope: openid
- description: Standard OpenID Connect scope; releases the email and email_verified claims.
  flows: []
  scope: email
- description: Full access to the Customer Account API for the authenticated customer — orders, addresses, profile and subscription data belonging to that customer.
  flows: []
  scope: customer-account-api:full
- description: Full access to the customer-account MCP surface, allowing an agent acting for a signed-in customer to operate on that customer's account over MCP.
  flows: []
  scope: customer-account-mcp-api:full
slug: leaftfoods-scopes
source_filename: leaftfoods-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.leaftfoods.com/.well-known/openid-configuration\ndocs: https://www.leaftfoods.com/.well-known/oauth-authorization-server\nname: Leaft Foods OAuth Scopes\ndescription: OAuth 2.0 / OpenID Connect scopes advertised by the authorization server discovered from the\n  Leaft Foods storefront host. The authorization server is Shopify's hosted customer-account issuer for\n  shop 95682920744; the scope list below is taken verbatim from scopes_supported in the discovery document.\nissuer: https://shopify.com/authentication/95682920744\nauthorization_endpoint: https://shopify.com/authentication/95682920744/oauth/authorize\ntoken_endpoint: https://shopify.com/authentication/95682920744/oauth/token\ncount: 4\nscopes:\n- name: openid\n  description: Standard OpenID Connect scope; requests an ID token identifying the signed-in customer.\n  standard: true\n- name: email\n  description: Standard OpenID Connect scope; releases the\
  \ email and email_verified claims.\n  standard: true\n- name: customer-account-api:full\n  description: Full access to the Customer Account API for the authenticated customer — orders, addresses,\n    profile and subscription data belonging to that customer.\n  standard: false\n- name: customer-account-mcp-api:full\n  description: Full access to the customer-account MCP surface, allowing an agent acting for a signed-in\n    customer to operate on that customer's account over MCP.\n  standard: false\nnotes:\n- The UCP storefront MCP endpoint at /api/ucp/mcp is a separate surface and is not gated by these scopes;\n  it gates on agent-profile discovery plus buyer approval at payment.\n- No Leaft Foods-specific (non-Shopify) scopes are published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leaftfoods/refs/heads/main/scopes/leaftfoods-scopes.yml
summary_line: 4 scopes
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
token_bound: false
token_urls:
- https://shopify.com/authentication/95682920744/oauth/token
---
