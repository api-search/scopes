---
api_specs:
- filename: squarespace-orders-api-openapi.yml
  format: yaml
  label: Squarespace Orders API
  slug: squarespace-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/openapi/squarespace-orders-api-openapi.yml
- filename: squarespace-products-api-openapi.yml
  format: yaml
  label: Squarespace Products API
  slug: squarespace-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/openapi/squarespace-products-api-openapi.yml
- filename: squarespace-inventory-api-openapi.yml
  format: yaml
  label: Squarespace Inventory API
  slug: squarespace-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/openapi/squarespace-inventory-api-openapi.yml
- filename: squarespace-profiles-api-openapi.yml
  format: yaml
  label: Squarespace Profiles API
  slug: squarespace-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/openapi/squarespace-profiles-api-openapi.yml
- filename: squarespace-transactions-api-openapi.yml
  format: yaml
  label: Squarespace Transactions API
  slug: squarespace-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/openapi/squarespace-transactions-api-openapi.yml
- filename: squarespace-webhook-subscriptions-api-openapi.yml
  format: yaml
  label: Squarespace Webhook Subscriptions API
  slug: squarespace-webhook-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/openapi/squarespace-webhook-subscriptions-api-openapi.yml
- filename: squarespace-site-api-openapi.yml
  format: yaml
  label: Squarespace Site API
  slug: squarespace-site-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/openapi/squarespace-site-api-openapi.yml
- filename: squarespace-commerce-api-v2-openapi.json
  format: json
  label: Squarespace Commerce API
  slug: squarespace-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/openapi/squarespace-commerce-api-v2-openapi.json
authorization_urls: []
description: Squarespace authorizes third-party applications (Squarespace Extensions) with OAuth 2.0 authorization code grant. The scope parameter on the authorize endpoint takes a COMMA-separated list of permission values — not the space-separated list RFC 6749 describes — and the confirmation page always presents the merchant's website(s) for selection because every scope is rooted at `website.*`. The scope list below is transcribed verbatim from the provider's OAuth guide. Note that the published OpenAPI declares only a single `http bearer` security scheme and no `oauth2` scheme, so these scopes exist ONLY in prose documentation and cannot be derived from the machine-readable contract — `derive-oauth-scopes.py` finds zero.
docs: https://developers.squarespace.com/oauth
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Squarespace Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Squarespace uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Squarespace
provider_slug: squarespace
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: squarespace-scopes
source_filename: squarespace-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developers.squarespace.com/oauth\ndocs: https://developers.squarespace.com/oauth\nprovider: Squarespace\nproviderId: squarespace\ndescription: >-\n  Squarespace authorizes third-party applications (Squarespace Extensions) with OAuth 2.0\n  authorization code grant. The scope parameter on the authorize endpoint takes a COMMA-separated\n  list of permission values — not the space-separated list RFC 6749 describes — and the\n  confirmation page always presents the merchant's website(s) for selection because every scope is\n  rooted at `website.*`. The scope list below is transcribed verbatim from the provider's OAuth\n  guide. Note that the published OpenAPI declares only a single `http bearer` security scheme and\n  no `oauth2` scheme, so these scopes exist ONLY in prose documentation and cannot be derived from\n  the machine-readable contract — `derive-oauth-scopes.py` finds zero.\nflow: authorization_code\ngrant_types:\n\
  \  - authorization_code\n  - refresh_token\nendpoints:\n  authorization: https://login.squarespace.com/api/1/login/oauth/provider/authorize\n  token: https://login.squarespace.com/api/1/login/oauth/provider/tokens\n  registration: https://developers.squarespace.com/oauth\nscope_delimiter: ','\nscope_delimiter_note: >-\n  Squarespace documents \"comma-separated list of client permission values\", e.g.\n  scope=website.inventory,website.orders. This deviates from the space-delimited convention in\n  RFC 6749 §3.3 and is a common integration failure.\ntoken_lifetimes:\n  access_token: 30m\n  refresh_token: long-term (requires access_type=offline)\n  authorization_code: 2m, single use\nlong_term_access:\n  parameter: access_type=offline\n  note: >-\n    Omit access_type for short-term API access. Use offline to receive a refresh token for\n    long-term access; subsequent token requests use grant_type=refresh_token.\ncsrf:\n  parameter: state\n  required: true\n  note: Squarespace requires\
  \ state and documents verifying it on the redirect URI to prevent CSRF.\nscope_count: 10\nscopes:\n  - name: website.orders\n    description: Send order data and mark orders as fulfilled.\n    access: write\n    api: Orders\n  - name: website.orders.read\n    description: View order and fulfillment information.\n    access: read\n    api: Orders\n  - name: website.transactions.read\n    description: Access transactional order and donation data.\n    access: read\n    api: Transactions\n  - name: website.inventory\n    description: View and update inventory stock levels.\n    access: write\n    api: Inventory\n  - name: website.inventory.read\n    description: View inventory stock levels.\n    access: read\n    api: Inventory\n  - name: website.products\n    description: View product information and modify products.\n    access: write\n    api: Products\n  - name: website.products.read\n    description: View product information.\n    access: read\n    api: Products\n  - name: website.contacts\n\
  \    description: >-\n      View customer contact information and address book entries; create, update, and delete\n      contacts and address book entries.\n    access: write\n    api: Contacts\n  - name: website.contacts.read\n    description: View customer contact information and address book entries.\n    access: read\n    api: Contacts\n  - name: website.discounts\n    description: View and manage discounts.\n    access: write\n    api: Discounts\n  - name: website.discounts.read\n    description: View discounts.\n    access: read\n    api: Discounts\napi_key_permissions:\n  note: >-\n    API keys are a separate authorization path from OAuth and use permission LEVELS selected in the\n    Squarespace admin (Settings > Advanced > Developer API Keys), not scope strings. Permissions on\n    an issued key or token can never be modified — a new key must be generated, and OAuth clients\n    must have the merchant re-initiate the connection.\n  source: https://developers.squarespace.com/commerce-apis/authentication-and-permissions\n\
  \  apis:\n    - api: Forms\n      levels: [read]\n      note: For Zapier integration only.\n    - api: Inventory\n      levels: [read, read-write]\n    - api: Orders\n      levels: [read, read-write]\n    - api: Products\n      levels: [read, read-write]\n    - api: Contacts\n      levels: [read, read-write]\n      note: API key support added 2026-06-17; previously OAuth only.\n    - api: Discounts\n      levels: [read, read-write]\n    - api: Webhook Subscriptions\n      levels: [read-write]\n      note: OAuth only — no API key path.\n    - api: Profiles\n      levels: [read]\n      note: Maintenance mode; new integrations should use Contacts.\n    - api: Transactions\n      levels: [read]\ngaps:\n  - The published OpenAPI declares no oauth2 securityScheme, so scopes are not machine-readable.\n  - >-\n    No scope is documented for the Webhook Subscriptions API even though it is OAuth-only; the docs\n    describe the permission by name but do not publish a website.* scope string for it.\n\
  \  - No scope is published for the Analytics API surfaced in the OpenAPI (POST /v1/analytics/transaction-summaries).\nevidence:\n  - url: https://developers.squarespace.com/oauth\n    status: 200\n  - url: https://developers.squarespace.com/commerce-apis/authentication-and-permissions\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/scopes/squarespace-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Commerce
- E-Commerce
- Marketing
- Payments
- Retail
- Website Builder
- Webhooks
token_urls: []
---
