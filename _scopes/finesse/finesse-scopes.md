---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Finesse Scopes
name_suffix: OAuth Scopes
note: Scopes are read verbatim from the `scopes_supported` array of the OAuth 2.0 / OpenID Connect metadata FINESSE serves at its own apex domain. FINESSE publishes no scope reference page of its own, so the descriptions below state only what the scope name asserts plus what the metadata itself proves; nothing is inferred beyond that. The authorization server is the Shopify-hosted customer identity provider for this merchant (issuer https://shopify.com/authentication/23733469261), with endpoints on account.finesse.us.
overview: 'FINESSE uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: FINESSE
provider_slug: finesse
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: finesse-scopes
source_filename: finesse-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://finesse.us/.well-known/openid-configuration\ndocs: null\nnote: >-\n  Scopes are read verbatim from the `scopes_supported` array of the OAuth 2.0 / OpenID Connect\n  metadata FINESSE serves at its own apex domain. FINESSE publishes no scope reference page of its\n  own, so the descriptions below state only what the scope name asserts plus what the metadata\n  itself proves; nothing is inferred beyond that. The authorization server is the Shopify-hosted\n  customer identity provider for this merchant (issuer\n  https://shopify.com/authentication/23733469261), with endpoints on account.finesse.us.\nauthorization_server: https://account.finesse.us/authentication/oauth/authorize\ntoken_endpoint: https://account.finesse.us/authentication/oauth/token\npkce: S256\nscope_count: 4\nscopes:\n  - name: openid\n    standard: true\n    spec: OpenID Connect Core 1.0\n    description: Request an ID token identifying the signed-in FINESSE\
  \ shopper.\n  - name: email\n    standard: true\n    spec: OpenID Connect Core 1.0\n    description: Release the shopper's email address and email_verified claim.\n  - name: 'customer-account-api:full'\n    standard: false\n    description: >-\n      Full access to the customer account API on behalf of the signed-in shopper — the surface behind\n      account.finesse.us (orders, addresses, profile). Not documented on any FINESSE page.\n  - name: 'customer-account-mcp-api:full'\n    standard: false\n    description: >-\n      Full access to a customer-account MCP API on behalf of the signed-in shopper. This is a\n      logged-in agent surface distinct from the anonymous storefront MCP endpoint at\n      /api/ucp/mcp; FINESSE publishes no documentation for it, and its tool manifest was not\n      retrievable without a customer session.\nnotes: >-\n  These are end-user consent scopes for shopper identity, not developer API scopes. The public\n  agent commerce endpoint (https://finesse.us/api/ucp/mcp)\
  \ carries no OAuth scope requirement at\n  all — see authentication/finesse-authentication.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finesse/refs/heads/main/scopes/finesse-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- retail
- ecommerce
- fashion
- apparel
- direct-to-consumer
- agentic-commerce
- ucp
- mcp
- agent-native
- shopify
- consumer
token_urls: []
---
