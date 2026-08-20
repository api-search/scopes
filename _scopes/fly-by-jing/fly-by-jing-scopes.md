---
authorization_urls: []
description: ''
docs: https://flybyjing.com/.well-known/openid-configuration
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Fly By Jing Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Fly By Jing uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Fly By Jing
provider_slug: fly-by-jing
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: fly-by-jing-scopes
source_filename: fly-by-jing-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\ndocs: https://flybyjing.com/.well-known/openid-configuration\nsource: >-\n  scopes_supported advertised in the live OIDC discovery document for the Fly By\n  Jing storefront (Shopify Customer Account API).\nflow: authorization_code\nauthorization_endpoint: https://account.flybyjing.com/authentication/oauth/authorize\ntoken_endpoint: https://account.flybyjing.com/authentication/oauth/token\nscopes:\n- name: openid\n  description: OpenID Connect sign-in; returns an ID token identifying the customer.\n- name: email\n  description: Access to the authenticated customer's email address and email_verified claim.\n- name: 'customer-account-api:full'\n  description: >-\n    Full access to the Shopify Customer Account API for the signed-in customer\n    (orders, profile, addresses, subscriptions, and other account data).\n- name: 'customer-account-mcp-api:full'\n  description: >-\n    Full access to the Customer Account MCP API surface, exposing\
  \ the customer's\n    account data to MCP-based agents on behalf of the signed-in customer.\nnotes: >-\n  Scopes are defined and enforced by Shopify's Customer Account platform, not by\n  Fly By Jing directly. This is the storefront-facing customer identity surface;\n  there is no separate first-party OAuth server.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fly-by-jing/refs/heads/main/scopes/fly-by-jing-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Food and Beverage
- Consumer Packaged Goods
- E-Commerce
- Shopify
- Direct to Consumer
- MCP
- Agentic Commerce
token_urls: []
---
