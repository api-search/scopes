---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Create Wellness Scopes
name_suffix: OAuth Scopes
note: Read verbatim from the scopes_supported array of the OpenID Connect discovery document served at trycreate.co. These are Shopify Customer Accounts scopes exposed on the brand host; Create Wellness publishes no scope reference page of its own, so descriptions below are marked with their source rather than quoted from brand documentation.
overview: 'Create Wellness uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Create Wellness
provider_slug: create-wellness
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: create-wellness-scopes
source_filename: create-wellness-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: https://trycreate.co/.well-known/openid-configuration\nnote: >-\n  Read verbatim from the scopes_supported array of the OpenID Connect discovery\n  document served at trycreate.co. These are Shopify Customer Accounts scopes\n  exposed on the brand host; Create Wellness publishes no scope reference page\n  of its own, so descriptions below are marked with their source rather than\n  quoted from brand documentation.\nauthorization_server: https://shopify.com/authentication/61192044732\ndocs: null\ndocs_note: >-\n  No scopes/permissions reference page exists on trycreate.co. The upstream\n  platform reference is https://shopify.dev/docs/api/customer — that is\n  Shopify's documentation, not the provider's, and is recorded here as context\n  only.\nscope_count: 4\nscopes:\n- name: openid\n  description: Standard OpenID Connect scope requesting an ID token.\n  source: openid-configuration scopes_supported\n  standard: true\n- name:\
  \ email\n  description: Standard OpenID Connect scope releasing the email and email_verified claims.\n  source: openid-configuration scopes_supported\n  standard: true\n- name: customer-account-api:full\n  description: >-\n    Full access to the Shopify Customer Account API on behalf of the signed-in\n    buyer. Not described anywhere on the provider's own surface.\n  source: openid-configuration scopes_supported\n  standard: false\n- name: customer-account-mcp-api:full\n  description: >-\n    Full access to the Shopify Customer Account MCP API on behalf of the signed-in\n    buyer. Not described anywhere on the provider's own surface.\n  source: openid-configuration scopes_supported\n  standard: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/create-wellness/refs/heads/main/scopes/create-wellness-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Health and Wellness
- Supplements
- Consumer Products
- E-Commerce
- Direct to Consumer
- Agentic Commerce
- MCP
- Shopify
- Nutrition
token_urls: []
---
