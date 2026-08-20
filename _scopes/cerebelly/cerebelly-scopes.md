---
authorization_urls: []
description: The complete scopes_supported list published by Cerebelly's own OpenID Connect discovery document. Four scopes, no more — this is the whole authorization vocabulary the domain exposes. Cerebelly publishes no OpenAPI, so this was read directly from the live metadata document rather than derived from a spec.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Cerebelly Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cerebelly uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cerebelly
provider_slug: cerebelly
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: cerebelly-scopes
source_filename: cerebelly-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: https://cerebelly.com/.well-known/openid-configuration\nname: Cerebelly OAuth scopes\ndescription: >-\n  The complete scopes_supported list published by Cerebelly's own OpenID Connect\n  discovery document. Four scopes, no more — this is the whole authorization\n  vocabulary the domain exposes. Cerebelly publishes no OpenAPI, so this was read\n  directly from the live metadata document rather than derived from a spec.\nauthorization_server: https://shopify.com/authentication/74590912725\nauthorization_endpoint: https://account.cerebelly.com/authentication/oauth/authorize\ntoken_endpoint: https://account.cerebelly.com/authentication/oauth/token\nflow: authorization_code\npkce: S256\ngranularity: coarse\nscopes:\n- name: openid\n  description: >-\n    Standard OpenID Connect scope. Requests an ID token identifying the customer;\n    issues the sub, iss, aud, exp, iat, nonce and sid claims.\n  standard: true\n  spec: https://openid.net/specs/openid-connect-core-1_0.html\n\
  - name: email\n  description: >-\n    Standard OpenID Connect scope. Adds the email and email_verified claims to the\n    ID token.\n  standard: true\n  spec: https://openid.net/specs/openid-connect-core-1_0.html\n- name: 'customer-account-api:full'\n  description: >-\n    Full read and write access to the authenticated customer's account through the\n    Customer Account GraphQL API at account.cerebelly.com — profile, addresses,\n    orders, subscriptions and payment methods.\n  standard: false\n  granularity: all-or-nothing\n  note: >-\n    There is no read-only variant and no per-resource split. A customer consenting\n    to this scope consents to the entire account surface at once.\n- name: 'customer-account-mcp-api:full'\n  description: >-\n    Full access to the customer-account MCP API — the authenticated, per-customer\n    counterpart to the anonymous UCP commerce MCP endpoint on the storefront host.\n  standard: false\n  granularity: all-or-nothing\n  note: >-\n    Notable as\
  \ a first-class agent scope: the authorization server treats MCP as a\n    distinct protected surface with its own consent grant, rather than folding it\n    into the general account scope.\ncoverage:\n  total: 4\n  standard: 2\n  provider_specific: 2\n  read_only_variants: 0\nobservations:\n- >-\n  Both provider-specific scopes end in \":full\". Neither offers least-privilege\n  narrowing, so an agent that needs only order history must ask for write access to\n  the entire account.\n- >-\n  No scope governs the anonymous commerce surfaces. search_catalog, create_cart and\n  the Storefront GraphQL catalog fields require no grant at all.\nx-evidence:\n  fetched: '2026-08-09'\n  url: https://cerebelly.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json; charset=utf-8\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cerebelly/refs/heads/main/scopes/cerebelly-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Baby Food
- Consumer Packaged Goods
- Food and Beverage
- E-Commerce
- Retail
- Direct to Consumer
- Shopify
- Agentic Commerce
- Universal Commerce Protocol
- Nutrition
token_urls: []
---
