---
authorization_urls: []
description: ''
docs: https://developers.cafe24.com/app/front/app/develop/oauth
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Wyatt Scopes
name_suffix: OAuth Scopes
note: 'Read verbatim from scopes_supported in the two discovery documents Wyatt''s domain serves. Two distinct scope vocabularies are published, and they do not overlap: the OIDC/authorization-server document advertises UCP-namespaced shopping scopes, while the RFC 9728 protected-resource document guarding the MCP endpoint advertises Cafe24''s own mall.* scopes. Both are recorded as published; no scope was inferred.'
overview: 'Wyatt uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Wyatt
provider_slug: wyatt
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: wyatt-scopes
source_filename: wyatt-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: https://drforhair.co.kr/.well-known/openid-configuration\ndocs: https://developers.cafe24.com/app/front/app/develop/oauth\nnote: >-\n  Read verbatim from scopes_supported in the two discovery documents Wyatt's domain serves. Two\n  distinct scope vocabularies are published, and they do not overlap: the OIDC/authorization-server\n  document advertises UCP-namespaced shopping scopes, while the RFC 9728 protected-resource\n  document guarding the MCP endpoint advertises Cafe24's own mall.* scopes. Both are recorded as\n  published; no scope was inferred.\noperator: cafe24\nscope_count: 8\nvocabularies:\n- name: ucp-shopping\n  namespace: dev.ucp.shopping\n  standard: Universal Commerce Protocol (UCP)\n  advertised_by: /.well-known/openid-configuration and /.well-known/oauth-authorization-server\n  scopes:\n  - name: openid\n    description: OIDC — request an ID token for the shopper.\n  - name: dev.ucp.shopping.checkout:manage\n\
  \    description: Create and manage a checkout for the shopper.\n    write: true\n  - name: dev.ucp.shopping.cart:manage\n    description: Create and manage the shopper's cart.\n    write: true\n  - name: dev.ucp.shopping.order:read\n    description: Read the shopper's orders.\n    write: false\n  - name: dev.ucp.shopping.catalog.search:read\n    description: Search the storefront catalog.\n    write: false\n  - name: dev.ucp.shopping.catalog.lookup:read\n    description: Look up a specific catalog item.\n    write: false\n- name: cafe24-mall\n  namespace: mall\n  advertised_by: /.well-known/oauth-protected-resource\n  guards: https://drforhair2024.cafe24api.com/api/mcp\n  scopes:\n  - name: openid\n    description: OIDC — request an ID token for the shopper.\n  - name: mall.read_customer_order\n    description: Read the authenticated customer's orders. Backs search-customer-orders and\n      search-customer-order-detail.\n    write: false\n  - name: mall.write_customer_order\n    description:\
  \ Write to the authenticated customer's orders. Backs cancel-unpaid-order.\n    write: true\ndivergence_note: >-\n  The scopes guarding the live MCP resource (mall.*) are NOT the scopes advertised on the\n  authorization-server metadata (dev.ucp.shopping.*). An agent reading only the OIDC document\n  would request scopes the MCP resource does not name. Recorded as observed; not reconciled,\n  because reconciling it would require guessing.\nx-evidence:\n  fetched: '2026-09-04'\n  openid_configuration_status: 200\n  oauth_protected_resource_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wyatt/refs/heads/main/scopes/wyatt-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Beauty
- Personal Care
- Haircare
- Consumer Products
- E-Commerce
- Retail
- Agentic Commerce
- Model Context Protocol
- South Korea
token_urls: []
---
