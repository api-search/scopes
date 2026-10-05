---
api_specs:
- filename: makeup-land-brands-api-openapi.yml
  format: yaml
  label: makeup.land Brands API
  slug: makeup-land-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/makeup-land/refs/heads/main/openapi/makeup-land-brands-api-openapi.yml
- filename: makeup-land-cart-api-openapi.yml
  format: yaml
  label: makeup.land Cart API
  slug: makeup-land-cart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/makeup-land/refs/heads/main/openapi/makeup-land-cart-api-openapi.yml
- filename: makeup-land-customers-api-openapi.yml
  format: yaml
  label: makeup.land Customers API
  slug: makeup-land-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/makeup-land/refs/heads/main/openapi/makeup-land-customers-api-openapi.yml
- filename: makeup-land-gift-cards-api-openapi.yml
  format: yaml
  label: makeup.land Gift Cards API
  slug: makeup-land-gift-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/makeup-land/refs/heads/main/openapi/makeup-land-gift-cards-api-openapi.yml
- filename: makeup-land-orders-api-openapi.yml
  format: yaml
  label: makeup.land Orders API
  slug: makeup-land-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/makeup-land/refs/heads/main/openapi/makeup-land-orders-api-openapi.yml
- filename: makeup-land-payment-links-api-openapi.yml
  format: yaml
  label: makeup.land Payment Links API
  slug: makeup-land-payment-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/makeup-land/refs/heads/main/openapi/makeup-land-payment-links-api-openapi.yml
- filename: makeup-land-products-api-openapi.yml
  format: yaml
  label: makeup.land Products API
  slug: makeup-land-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/makeup-land/refs/heads/main/openapi/makeup-land-products-api-openapi.yml
- filename: makeup-land-proposals-api-openapi.yml
  format: yaml
  label: makeup.land Proposals API
  slug: makeup-land-proposals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/makeup-land/refs/heads/main/openapi/makeup-land-proposals-api-openapi.yml
- filename: makeup-land-register-api-openapi.yml
  format: yaml
  label: makeup.land Register API
  slug: makeup-land-register-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/makeup-land/refs/heads/main/openapi/makeup-land-register-api-openapi.yml
authorization_urls: []
description: ''
docs: https://makeup.land/auth.md
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Makeup Land Scopes
name_suffix: OAuth Scopes
note: These are NOT OAuth 2.0 scopes negotiated at request time. derive-oauth-scopes.py found no oauth2 scheme (correctly). The provider publishes the same five scope names in three places — the OpenAPI root x-scopes map and per-operation security[] requirements on the bearerAuth scheme, the RFC 8414 authorization-server metadata scopes_supported, and the RFC 9728 protected-resource metadata scopes_supported — and auth.md explains they are fixed on a bearer token when a human issues it. read_only is a flag, not a scope, but the provider lists it under scopes_supported.
overview: 'makeup.land publishes 5 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the makeup.land API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: makeup.land
provider_slug: makeup-land
schemes:
- bearerFormat: ml_<hex24>
  discovery:
  - https://makeup.land/.well-known/oauth-authorization-server
  - https://makeup.land/.well-known/oauth-protected-resource
  issuance: Manual, by email (info@makeup.land / shop@makeup.land) — auth.md "identity_assertion + email"
  name: bearerAuth
  scheme: bearer
  source: openapi/makeup-land-openapi.yml
  type: http
scope_count: 5
scope_names:
- full
- register
- giftcards
- proposals
- read_only
scopes:
- description: Full read + write access. Default scope for first-party tokens.
  flows: []
  scope: full
- description: Issue new customer registrations and read registrations belonging to the token's registration_source. Restricted to the /register and /registrations endpoints (plus customer opportunities).
  flows: []
  scope: register
- description: Redeem gift cards. Required only by POST /gift-cards/redeem. The public /gift-cards/validate endpoint requires no token.
  flows: []
  scope: giftcards
- description: Submit catalog enrichment proposals to /proposals. Read-only against the rest of the catalog.
  flows: []
  scope: proposals
- description: Marker for tokens whose read_only=true flag rejects every write with 403 read_only_token. Not negotiated at request time — set at token issuance.
  flows: []
  scope: read_only
slug: makeup-land-scopes
source_filename: makeup-land-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/makeup-land-openapi.yml\ndocs: https://makeup.land/auth.md\nnote: >-\n  These are NOT OAuth 2.0 scopes negotiated at request time. derive-oauth-scopes.py found no oauth2 scheme\n  (correctly). The provider publishes the same five scope names in three places — the OpenAPI root x-scopes\n  map and per-operation security[] requirements on the bearerAuth scheme, the RFC 8414 authorization-server\n  metadata scopes_supported, and the RFC 9728 protected-resource metadata scopes_supported — and auth.md\n  explains they are fixed on a bearer token when a human issues it. read_only is a flag, not a scope, but\n  the provider lists it under scopes_supported.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: ml_<hex24>\n  source: openapi/makeup-land-openapi.yml\n  issuance: Manual, by email (info@makeup.land / shop@makeup.land) — auth.md \"identity_assertion + email\"\n  discovery:\n  - https://makeup.land/.well-known/oauth-authorization-server\n\
  \  - https://makeup.land/.well-known/oauth-protected-resource\nscopes:\n- scope: full\n  description: Full read + write access. Default scope for first-party tokens.\n  operations: [listBrands, listProducts, getCustomer, upsertCustomer, patchCustomerTags, listCustomerOpportunities, getCustomerBestDeals, getCart, clearCart, addCartItem, patchCartItem, deleteCartItem, listOrders, listGiftCards, redeemGiftCard, listPaymentLinks, registerCustomer, listRegistrations, getRegistration, submitProposals]\n  sources:\n  - \"openapi x-scopes\"\n  - \"openapi security[]\"\n  - \"oauth-authorization-server\"\n  - \"oauth-protected-resource\"\n- scope: register\n  description: Issue new customer registrations and read registrations belonging to the token's registration_source. Restricted to the /register and /registrations endpoints (plus customer opportunities).\n  operations: [registerCustomer, listRegistrations, getRegistration, listCustomerOpportunities]\n  sources:\n  - \"openapi x-scopes\"\n \
  \ - \"openapi security[]\"\n  - \"oauth-authorization-server\"\n  - \"oauth-protected-resource\"\n- scope: giftcards\n  description: Redeem gift cards. Required only by POST /gift-cards/redeem. The public /gift-cards/validate endpoint requires no token.\n  operations: [redeemGiftCard]\n  sources:\n  - \"openapi x-scopes\"\n  - \"openapi security[]\"\n  - \"oauth-authorization-server\"\n  - \"oauth-protected-resource\"\n- scope: proposals\n  description: Submit catalog enrichment proposals to /proposals. Read-only against the rest of the catalog.\n  operations: [submitProposals]\n  sources:\n  - \"openapi x-scopes\"\n  - \"openapi security[]\"\n  - \"oauth-authorization-server\"\n  - \"oauth-protected-resource\"\n- scope: read_only\n  kind: flag\n  description: Marker for tokens whose read_only=true flag rejects every write with 403 read_only_token. Not negotiated at request time — set at token issuance.\n  operations: []\n  sources: [openapi x-scopes, oauth-authorization-server, oauth-protected-resource]\n\
  unauthenticated_operations:\n- validateGiftCard\n- listProducts (catalog filters only — bearer required once phone, include=inventory or relevant_to_phone is passed)\nselector_not_scope:\n  name: phoneIdentifier\n  note: The phone query/body parameter selects a customer and is declared as an apiKey securityScheme, but the provider's own description says it is not a credential and bearerAuth is always required alongside it.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/makeup-land/refs/heads/main/scopes/makeup-land-scopes.yml
summary_line: 5 scopes
tags:
- Cosmetics
- Beauty
- Retail
- E-Commerce
- Shopping
- Loyalty
- Gift Cards
- Product Search
- Agentic Commerce
- MCP
- Agent-Native
- Israel
- A2A
token_bound: false
token_urls: []
---
