---
authorization_urls: []
description: OAuth 2.0 / OpenID Connect scopes advertised by the store's customer-account authorization server, read from the scopes_supported array of the discovery document served on the company's own domain. Derived from no OpenAPI — this store publishes none — so every value here is verbatim from the provider's discovery document.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Willie S Reserve Scopes
name_suffix: OAuth Scopes
note: These scopes govern the customer-account surface only. The anonymous UCP/MCP endpoint at /api/ucp/mcp requires no scope and no token.
overview: 'Willie''s Reserve publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Willie''s Reserve API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Willie's Reserve
provider_slug: willie-s-reserve
schemes: []
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OpenID Connect scope requesting an ID token for the authenticated customer.
  flows: []
  scope: openid
- description: Releases the customer's email and email_verified claims.
  flows: []
  scope: email
- description: Full access to the customer-account API for the authenticated customer.
  flows: []
  scope: customer-account-api:full
- description: Full access to the customer-account MCP API — the authenticated counterpart to the anonymous UCP/MCP storefront endpoint, covering the signed-in customer's own account context.
  flows: []
  scope: customer-account-mcp-api:full
slug: willie-s-reserve-scopes
source_filename: willie-s-reserve-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: https://williesreserve.com/.well-known/openid-configuration\ndescription: >-\n  OAuth 2.0 / OpenID Connect scopes advertised by the store's customer-account authorization\n  server, read from the scopes_supported array of the discovery document served on the company's\n  own domain. Derived from no OpenAPI — this store publishes none — so every value here is\n  verbatim from the provider's discovery document.\nissuer: https://shopify.com/authentication/59591163950\nscope_count: 4\nscopes:\n- name: openid\n  description: Standard OpenID Connect scope requesting an ID token for the authenticated customer.\n- name: email\n  description: Releases the customer's email and email_verified claims.\n- name: customer-account-api:full\n  description: Full access to the customer-account API for the authenticated customer.\n- name: customer-account-mcp-api:full\n  description: >-\n    Full access to the customer-account MCP API — the authenticated\
  \ counterpart to the anonymous\n    UCP/MCP storefront endpoint, covering the signed-in customer's own account context.\nnote: >-\n  These scopes govern the customer-account surface only. The anonymous UCP/MCP endpoint at\n  /api/ucp/mcp requires no scope and no token.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/willie-s-reserve/refs/heads/main/scopes/willie-s-reserve-scopes.yml
summary_line: 4 scopes
tags:
- Company
- Cannabis
- Consumer Products
- Retail
- E-Commerce
- Agentic Commerce
- MCP
- Universal Commerce Protocol
- Shopify
token_bound: false
token_urls: []
---
