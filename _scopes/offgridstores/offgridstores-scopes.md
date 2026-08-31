---
authorization_urls: []
description: OAuth scopes advertised by the authorization server Off Grid Stores' own host points at. There is no OpenAPI with oauth2 securitySchemes to derive from; these values are read verbatim from the scopes_supported array of the discovery document served at offgridstores.com.
docs: https://shopify.dev/docs/api/customer
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Offgridstores Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Off Grid Stores - All Things Off-Grid Solar uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Off Grid Stores - All Things Off-Grid Solar
provider_slug: offgridstores
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: offgridstores-scopes
source_filename: offgridstores-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://offgridstores.com/.well-known/oauth-authorization-server\ndocs: https://shopify.dev/docs/api/customer\ndescription: >-\n  OAuth scopes advertised by the authorization server Off Grid Stores' own host points at. There is\n  no OpenAPI with oauth2 securitySchemes to derive from; these values are read verbatim from the\n  scopes_supported array of the discovery document served at offgridstores.com.\nauthorization_server: https://shopify.com/authentication/55184621620\nauthorization_endpoint: https://account.offgridstores.com/authentication/oauth/authorize\ntoken_endpoint: https://account.offgridstores.com/authentication/oauth/token\nscope_count: 4\nscopes:\n- name: openid\n  description: Standard OpenID Connect scope; requests an ID token identifying the customer.\n  category: identity\n- name: email\n  description: Releases the customer's email and email_verified claims.\n  category: identity\n- name: customer-account-api:full\n\
  \  description: Full access to the Customer Account API on behalf of the signed-in customer.\n  category: account\n- name: customer-account-mcp-api:full\n  description: >-\n    Full access to the Customer Account MCP API on behalf of the signed-in customer. No anonymous\n    customer-account MCP endpoint was found on offgridstores.com; /customer/api/mcp returned 404.\n  category: agent\nnotes:\n- Scopes are Shopify customer-account scopes bound to this shop, not Off Grid Stores-authored scopes.\n- The Storefront GraphQL API and the /api/mcp storefront MCP server require no scope at all.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/offgridstores/refs/heads/main/scopes/offgridstores-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Commerce
- E-Commerce
- Retail
- off-grid solar
- Renewable Energy
- Backup Power
- solar generators
- LiFePO4 batteries
- Inverters
- homesteading
- Agentic Commerce
- MCP
- GraphQL
- UCP
token_urls: []
---
