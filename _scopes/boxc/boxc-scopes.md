---
api_specs:
- filename: boxc-openapi-original.yml
  format: yaml
  label: BoxC API
  slug: boxc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boxc/refs/heads/main/openapi/boxc-openapi-original.yml
authorization_urls:
- https://accounts.boxc.com/auth/v1/authorize
description: ''
docs: https://support.boxc.com/support/solutions/articles/65000182700-configuring-the-oauth-2-0-client-permissions
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Boxc Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Boxc publishes 19 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Boxc API on a user''s behalf.


  Tokens are issued from https://accounts.boxc.com/auth/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Boxc
provider_slug: boxc
schemes:
- flows:
  - authorizationUrl: https://accounts.boxc.com/auth/v1/authorize
    flow: authorizationCode
    tokenUrl: https://accounts.boxc.com/auth/v1/token
  name: OAuth2
  source: https://accounts.boxc.com/.well-known/openid-configuration
  type: oauth2
scope_count: 19
scope_names:
- openid
- email
- profile
- read_shipments
- write_shipments
- read_orders
- write_orders
- read_products
- write_products
- classify
- read_shops
- write_shops
- read_webhooks
- write_webhooks
- returns
- billing
- validate
- read_credentials
- write_credentials
scopes:
- description: OpenID Connect sign-in; enables issuance of an ID token.
  flows:
  - authorizationCode
  scope: openid
- description: Access the authorized user's email address claim.
  flows:
  - authorizationCode
  scope: email
- description: Access the authorized user's profile claims (name, locale, zoneinfo).
  flows:
  - authorizationCode
  scope: profile
- description: Read access to shipments, labels, estimates and tracking.
  flows:
  - authorizationCode
  scope: read_shipments
- description: Create, update, process and cancel shipments and labels.
  flows:
  - authorizationCode
  scope: write_shipments
- description: Read access to orders and fulfillments.
  flows:
  - authorizationCode
  scope: read_orders
- description: Create, update, delete orders and change order status.
  flows:
  - authorizationCode
  scope: write_orders
- description: Read access to products and SKUs.
  flows:
  - authorizationCode
  scope: read_products
- description: Create, update, delete products and SKUs.
  flows:
  - authorizationCode
  scope: write_products
- description: Classify products for HS codes / customs (Classify resource).
  flows:
  - authorizationCode
  scope: classify
- description: Read access to connected shops.
  flows:
  - authorizationCode
  scope: read_shops
- description: Create, update, delete shop connections.
  flows:
  - authorizationCode
  scope: write_shops
- description: Read access to webhook subscriptions.
  flows:
  - authorizationCode
  scope: read_webhooks
- description: Create, update, delete webhook subscriptions and queue events.
  flows:
  - authorizationCode
  scope: write_webhooks
- description: Access the Returns and Reshipments resources.
  flows:
  - authorizationCode
  scope: returns
- description: Access invoices and account balance / billing operations.
  flows:
  - authorizationCode
  scope: billing
- description: Validate addresses (ValidateAddress resource).
  flows:
  - authorizationCode
  scope: validate
- description: Read access to stored carrier credentials.
  flows:
  - authorizationCode
  scope: read_credentials
- description: Create, update, delete carrier credentials.
  flows:
  - authorizationCode
  scope: write_credentials
slug: boxc-scopes
source_filename: boxc-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://accounts.boxc.com/.well-known/openid-configuration\ndocs: https://support.boxc.com/support/solutions/articles/65000182700-configuring-the-oauth-2-0-client-permissions\nschemes:\n- name: OAuth2\n  type: oauth2\n  source: https://accounts.boxc.com/.well-known/openid-configuration\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.boxc.com/auth/v1/authorize\n    tokenUrl: https://accounts.boxc.com/auth/v1/token\nscopes:\n- scope: openid\n  description: OpenID Connect sign-in; enables issuance of an ID token.\n  flows: [authorizationCode]\n- scope: email\n  description: Access the authorized user's email address claim.\n  flows: [authorizationCode]\n- scope: profile\n  description: Access the authorized user's profile claims (name, locale, zoneinfo).\n  flows: [authorizationCode]\n- scope: read_shipments\n  description: Read access to shipments, labels, estimates and tracking.\n  flows: [authorizationCode]\n\
  - scope: write_shipments\n  description: Create, update, process and cancel shipments and labels.\n  flows: [authorizationCode]\n- scope: read_orders\n  description: Read access to orders and fulfillments.\n  flows: [authorizationCode]\n- scope: write_orders\n  description: Create, update, delete orders and change order status.\n  flows: [authorizationCode]\n- scope: read_products\n  description: Read access to products and SKUs.\n  flows: [authorizationCode]\n- scope: write_products\n  description: Create, update, delete products and SKUs.\n  flows: [authorizationCode]\n- scope: classify\n  description: Classify products for HS codes / customs (Classify resource).\n  flows: [authorizationCode]\n- scope: read_shops\n  description: Read access to connected shops.\n  flows: [authorizationCode]\n- scope: write_shops\n  description: Create, update, delete shop connections.\n  flows: [authorizationCode]\n- scope: read_webhooks\n  description: Read access to webhook subscriptions.\n  flows:\
  \ [authorizationCode]\n- scope: write_webhooks\n  description: Create, update, delete webhook subscriptions and queue events.\n  flows: [authorizationCode]\n- scope: returns\n  description: Access the Returns and Reshipments resources.\n  flows: [authorizationCode]\n- scope: billing\n  description: Access invoices and account balance / billing operations.\n  flows: [authorizationCode]\n- scope: validate\n  description: Validate addresses (ValidateAddress resource).\n  flows: [authorizationCode]\n- scope: read_credentials\n  description: Read access to stored carrier credentials.\n  flows: [authorizationCode]\n- scope: write_credentials\n  description: Create, update, delete carrier credentials.\n  flows: [authorizationCode]\nnotes: >-\n  Scopes are taken verbatim from the BoxC OIDC discovery document's scopes_supported.\n  A client's effective scope is configured in the BoxC account (OAuth 2.0 Client\n  Permissions) and inherited into issued tokens. The Calculate Duty resource additionally\n\
  \  requires a token minted with the documented `calculate` scope per the changelog\n  (v1.118); descriptions here are derived from the resource each scope governs.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boxc/refs/heads/main/scopes/boxc-scopes.yml
summary_line: 19 scopes · authorizationCode
tags:
- Company
- Logistics
- Shipping
- Ecommerce
- Cross-Border
- Fulfillment
- Customs
- Tracking
- Webhooks
token_urls:
- https://accounts.boxc.com/auth/v1/token
---
