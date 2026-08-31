---
authorization_urls: []
description: ''
docs:
- https://developer.kroger.com/documentation/public/security/guides-oauth
- https://developer.kroger.com/documentation/public/security/auth-tutorial
- https://developer.kroger.com/documentation/support/api-troubleshooting/troubleshooting
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Kroger Scopes
name_suffix: OAuth Scopes
note: Kroger does NOT publish a consolidated scope reference page. There is no OpenAPI in this repo to derive a securitySchemes.oauth2.scopes block from, and the portal's own API-catalog endpoints (/api/v1/developer/apis, /contracts/document/...) return 401 anonymously. Every scope listed below is a literal string quoted in a public Kroger doc page; nothing here is inferred from a naming pattern. Treat the list as incomplete by construction — the authoritative set is the one Kroger assigns to an application at registration.
overview: 'Kroger publishes 6 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Kroger API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kroger
provider_slug: kroger
schemes: []
scope_count: 6
scope_names:
- product.compact
- product.full.read
- product.personalized
- cart.basic:rw
- profile.full
- coupon.basic
scopes:
- description: Read the compact product response shape. Named in the Kroger Postman guide as the scope to configure for the Public API production collection, and present in the documented example JWT payload.
  flows: []
  scope: product.compact
- description: Read the full product response shape. Used as the worked example in the "Understanding OAuth2" scope section.
  flows: []
  scope: product.full.read
- description: Product data personalized to the authenticated customer. Requested alongside cart.basic:rw and profile.full in the Auth Code Tutorial.
  flows: []
  scope: product.personalized
- description: Read and write the authenticated customer's cart — the scope the Cart API tutorial requests before adding, updating or removing items.
  flows: []
  scope: cart.basic:rw
- description: Access the authenticated customer's profile. Requested in the Auth Code Tutorial's scope string.
  flows: []
  scope: profile.full
- description: 'Appears in the documented example access-token payload (scope: "product.compact coupon.basic"). Recorded because it is a real published string, and it is evidence of a Kroger API surface this catalog does not currently carry an entry for.'
  flows: []
  scope: coupon.basic
slug: kroger-scopes
source_filename: kroger-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "specification: API Commons OAuth Scopes\nspecificationVersion: '0.1'\nprovider: Kroger\nproviderId: kroger\ngenerated: '2026-08-27'\nmethod: searched\nsource: >-\n  Kroger developer documentation, read anonymously from the portal content API\n  (https://developer.kroger.com/api/v1/developer/content/search.json, HTTP 200).\ndocs:\n  - https://developer.kroger.com/documentation/public/security/guides-oauth\n  - https://developer.kroger.com/documentation/public/security/auth-tutorial\n  - https://developer.kroger.com/documentation/support/api-troubleshooting/troubleshooting\nnote: >-\n  Kroger does NOT publish a consolidated scope reference page. There is no\n  OpenAPI in this repo to derive a securitySchemes.oauth2.scopes block from, and\n  the portal's own API-catalog endpoints (/api/v1/developer/apis,\n  /contracts/document/...) return 401 anonymously. Every scope listed below is a\n  literal string quoted in a public Kroger doc page; nothing here is inferred\n  from a naming\
  \ pattern. Treat the list as incomplete by construction — the\n  authoritative set is the one Kroger assigns to an application at registration.\nnaming_convention:\n  documented: >-\n    \"In general, scopes are a composition of the resource, the shape of the data,\n    and the action, if available. For example, the scope product.full.read gives\n    the application permission to read the full response of the product\n    resource.\"\n  shape: '<resource>.<data-shape>[.<action>]  |  <resource>.<data-shape>:<rw>'\nassignment:\n  self_service: false\n  description: >-\n    Kroger assigns a set of scopes to the application during registration, driven\n    by which API Products were selected. An application is not authorized to use\n    any scope outside that set; changes are by request to Kroger.\nenforcement:\n  missing_scope_status: 403\n  missing_scope_body: '{\"errors\":{\"timestamp\":...,\"code\":\"Forbidden\",\"reason\":\"missing required scopes\"}}'\nscopes:\n  - scope: product.compact\n\
  \    api: Products API\n    grant: client_credentials\n    description: >-\n      Read the compact product response shape. Named in the Kroger Postman guide\n      as the scope to configure for the Public API production collection, and\n      present in the documented example JWT payload.\n    evidence: https://developer.kroger.com/documentation/public/getting-started/postman\n  - scope: product.full.read\n    api: Products API\n    grant: client_credentials\n    description: >-\n      Read the full product response shape. Used as the worked example in the\n      \"Understanding OAuth2\" scope section.\n    evidence: https://developer.kroger.com/documentation/public/security/guides-oauth\n  - scope: product.personalized\n    api: Products API\n    grant: authorization_code\n    description: >-\n      Product data personalized to the authenticated customer. Requested\n      alongside cart.basic:rw and profile.full in the Auth Code Tutorial.\n    evidence: https://developer.kroger.com/documentation/public/security/auth-tutorial\n\
  \  - scope: cart.basic:rw\n    api: Cart API\n    grant: authorization_code\n    description: >-\n      Read and write the authenticated customer's cart — the scope the Cart API\n      tutorial requests before adding, updating or removing items.\n    evidence: https://developer.kroger.com/documentation/public/security/auth-tutorial\n  - scope: profile.full\n    api: Identity API\n    grant: authorization_code\n    description: >-\n      Access the authenticated customer's profile. Requested in the Auth Code\n      Tutorial's scope string.\n    evidence: https://developer.kroger.com/documentation/public/security/auth-tutorial\n  - scope: coupon.basic\n    api: Coupon API (not listed in this repo's apis[])\n    grant: client_credentials\n    description: >-\n      Appears in the documented example access-token payload\n      (scope: \"product.compact coupon.basic\"). Recorded because it is a real\n      published string, and it is evidence of a Kroger API surface this catalog\n      does\
  \ not currently carry an entry for.\n    evidence: https://developer.kroger.com/documentation/public/security/service-to-service\n    confidence: medium\nscope_count: 6\ncompleteness: partial\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kroger/refs/heads/main/scopes/kroger-scopes.yml
summary_line: 6 scopes
tags:
- Groceries
- Grocery Retail
- Retail
- E-Commerce
- Product Catalog
- Store Locations
- Shopping Cart
- Loyalty
- Authentication
- Partner API
- Fortune 100
token_urls: []
---
