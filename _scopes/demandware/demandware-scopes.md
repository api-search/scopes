---
authorization_urls: []
description: OAuth scope model for Salesforce B2C Commerce (Demandware). SCAPI encodes access as OAuth scopes carried in the JWT access token. Scopes combine a tenant filter and an API family; the exact scope list is tenant- and API-specific and is managed in Account Manager / SLAS rather than published as a fixed enumeration. Documented from the SCAPI authorization guides; no spec-declared scope map is in the repo, so representative scope families are captured rather than a full list.
docs: https://developer.salesforce.com/docs/commerce/commerce-api/guide/authorization.html
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Demandware Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Demandware uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Demandware
provider_slug: demandware
schemes:
- docs: https://developer.salesforce.com/docs/commerce/commerce-api/guide/slas.html
  flows:
  - authorizationCode
  - clientCredentials
  name: SLAS
- docs: https://developer.salesforce.com/docs/commerce/commerce-api/guide/authorization-for-admin-apis.html
  flows:
  - clientCredentials
  name: Account Manager
scope_count: 0
scope_names: []
scopes: []
slug: demandware-scopes
source_filename: demandware-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developer.salesforce.com/docs/commerce/commerce-api/guide/authorization.html\ndocs: https://developer.salesforce.com/docs/commerce/commerce-api/guide/authorization.html\ndescription: >-\n  OAuth scope model for Salesforce B2C Commerce (Demandware). SCAPI encodes access\n  as OAuth scopes carried in the JWT access token. Scopes combine a tenant filter\n  and an API family; the exact scope list is tenant- and API-specific and is\n  managed in Account Manager / SLAS rather than published as a fixed enumeration.\n  Documented from the SCAPI authorization guides; no spec-declared scope map is in\n  the repo, so representative scope families are captured rather than a full list.\nschemes:\n- name: SLAS\n  flows: [authorizationCode, clientCredentials]\n  docs: https://developer.salesforce.com/docs/commerce/commerce-api/guide/slas.html\n- name: Account Manager\n  flows: [clientCredentials]\n  docs: https://developer.salesforce.com/docs/commerce/commerce-api/guide/authorization-for-admin-apis.html\n\
  scope_families:\n- scope: \"sfcc.shopper-*\"\n  description: >-\n    Shopper API scope family (e.g. sfcc.shopper-products, sfcc.shopper-baskets,\n    sfcc.shopper-orders, sfcc.shopper-customers) granted via SLAS tokens.\n  audience: shopper\n- scope: \"sfcc.<resource>.rw / .r\"\n  description: >-\n    Admin API scope family granting read (.r) or read-write (.rw) access to a\n    resource, granted via Account Manager tokens (e.g. sfcc.orders.rw,\n    sfcc.catalogs.rw, sfcc.products.r).\n  audience: admin\nnotes: >-\n  Scope strings are tenant-scoped and configured per API client. See the SCAPI\n  authorization guide and each API reference for the exact scope required by an\n  operation.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/demandware/refs/heads/main/scopes/demandware-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Commerce
- E-commerce
- Retail
- Commerce Cloud
- Storefront
- Shopper
- Catalog
- Orders
- SaaS
- Salesforce
token_urls: []
---
