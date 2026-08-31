---
api_specs:
- filename: mikmak-authentication-api-openapi.yml
  format: yaml
  label: MikMak Authentication API
  slug: mikmak-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mikmak/refs/heads/main/openapi/mikmak-authentication-api-openapi.yml
- filename: mikmak-availabilities-api-openapi.yml
  format: yaml
  label: MikMak Availabilities API
  slug: mikmak-availabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mikmak/refs/heads/main/openapi/mikmak-availabilities-api-openapi.yml
- filename: mikmak-cart-api-openapi.yml
  format: yaml
  label: MikMak Cart API
  slug: mikmak-cart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mikmak/refs/heads/main/openapi/mikmak-cart-api-openapi.yml
- filename: mikmak-custom-reports-api-openapi.yml
  format: yaml
  label: MikMak Custom Reports API
  slug: mikmak-custom-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mikmak/refs/heads/main/openapi/mikmak-custom-reports-api-openapi.yml
- filename: mikmak-experiences-api-openapi.yml
  format: yaml
  label: MikMak Experiences API
  slug: mikmak-experiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mikmak/refs/heads/main/openapi/mikmak-experiences-api-openapi.yml
- filename: mikmak-facet-api-openapi.yml
  format: yaml
  label: MikMak Facet API
  slug: mikmak-facet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mikmak/refs/heads/main/openapi/mikmak-facet-api-openapi.yml
- filename: mikmak-historical-pricing-reports-api-openapi.yml
  format: yaml
  label: MikMak Historical Pricing Reports API
  slug: mikmak-historical-pricing-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mikmak/refs/heads/main/openapi/mikmak-historical-pricing-reports-api-openapi.yml
- filename: mikmak-offers-api-openapi.yml
  format: yaml
  label: MikMak Offers API
  slug: mikmak-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mikmak/refs/heads/main/openapi/mikmak-offers-api-openapi.yml
- filename: mikmak-product-api-openapi.yml
  format: yaml
  label: MikMak Product API
  slug: mikmak-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mikmak/refs/heads/main/openapi/mikmak-product-api-openapi.yml
- filename: mikmak-product-search-api-openapi.yml
  format: yaml
  label: MikMak Product Search API
  slug: mikmak-product-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mikmak/refs/heads/main/openapi/mikmak-product-search-api-openapi.yml
- filename: mikmak-shoppable-recipe-reports-api-openapi.yml
  format: yaml
  label: MikMak Shoppable Recipe Reports API
  slug: mikmak-shoppable-recipe-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mikmak/refs/heads/main/openapi/mikmak-shoppable-recipe-reports-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.mikmak.ai/reference/commerce-api-authentication
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Mikmak Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'MikMak uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: MikMak
provider_slug: mikmak
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: mikmak-scopes
source_filename: mikmak-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://docs.mikmak.ai/reference/authorization-code-flow\ndocs: https://docs.mikmak.ai/reference/commerce-api-authentication\nprovider: MikMak\nproviderId: mikmak\nsummary: >-\n  MikMak publishes two OAuth 2.0 grants against a single authorization server hosted on the API\n  domain, but does NOT publish a scope reference. The only scope value that appears anywhere in\n  the documentation is `offline_access`, returned in the authorization-code token response.\n  Neither OpenAPI declares an oauth2 security scheme, so there is no spec-derived scope map to\n  reconcile against; permissions are described in prose as \"the permissions your app is\n  requesting\", shown to the user on a consent screen configured by MikMak per client.\nauthorization_servers:\n  - name: MikMak Authorization Server\n    authorizationUrl: https://api.mikmak.ai/commerce/v1/authorize\n    tokenUrl: https://api.mikmak.ai/commerce/v1/oauth/token\n    grants:\n\
  \      - authorization_code\n      - client_credentials\n      - refresh_token\n    consent_screen: true\n    note: >-\n      The client-credentials response documents an empty `scope` on the MCP path\n      (\"scope\": \"\") — a token minted for an audience, with no scope segmentation.\nscopes:\n  - name: offline_access\n    description: >-\n      Issues a refresh_token alongside the access token so the application can renew access\n      without sending the user back through the authorization screen. Returned in the\n      authorization-code and refresh-token grant responses.\n    grants:\n      - authorization_code\n      - refresh_token\n    source: https://docs.mikmak.ai/reference/authorization-code-flow\nscope_count: 1\ngaps:\n  - >-\n    No scopes/permissions reference page is published. An integrator cannot see, before\n    onboarding, which permissions a MikMak OAuth client can request or what the consent screen\n    will list.\n  - >-\n    Neither published OpenAPI declares an\
  \ oauth2 securityScheme, so the authorization-code and\n    client-credentials flows are invisible to any tool that reads the spec — they exist only in\n    prose on the ReadMe reference pages.\n  - >-\n    Access scoping is done by identity headers (x-api-key, x-wtb-id) and by the Auth0\n    `audience`, not by OAuth scope.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mikmak/refs/heads/main/scopes/mikmak-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Analytics
- Commerce
- E-Commerce
- Multichannel
- Retail Media
- Where to Buy
- Shoppable Media
- Product Availability
- MCP
- Agent Native
- Reporting
- CPG
token_urls: []
---
