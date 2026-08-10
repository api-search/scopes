---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Binske Scopes
name_suffix: OAuth Scopes
note: Scopes are advertised by the Shopify customer-account authorization server that binske's storefront delegates to via RFC 9728 protected-resource metadata. binske publishes no scope reference of its own; these are read verbatim from `scopes_supported` in the RFC 8414 metadata document.
overview: 'Binske uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Binske
provider_slug: binske
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: binske-scopes
source_filename: binske-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-07'\nmethod: probed\nsource: https://shopbinske.com/.well-known/oauth-authorization-server\nauthorization_server: https://shopify.com/authentication/64216269035\nprotected_resource: https://shopbinske.com\nnote: >-\n  Scopes are advertised by the Shopify customer-account authorization server that\n  binske's storefront delegates to via RFC 9728 protected-resource metadata.\n  binske publishes no scope reference of its own; these are read verbatim from\n  `scopes_supported` in the RFC 8414 metadata document.\nscopes:\n- name: openid\n  description: OpenID Connect — request an id_token identifying the buyer.\n  standard: true\n- name: email\n  description: Release the buyer's email address and email_verified claim.\n  standard: true\n- name: customer-account-api:full\n  description: Full access to the Shopify Customer Account API for the signed-in buyer.\n  standard: false\n- name: customer-account-mcp-api:full\n  description: >-\n    Full access to the Customer\
  \ Account MCP API for the signed-in buyer — the\n    authenticated counterpart to the anonymous UCP shopping MCP endpoint.\n  standard: false\ngranularity: coarse\nx-observation: >-\n  Both non-standard scopes are `:full`. There is no read/write split and no\n  per-resource scope, so an agent granted buyer access on this storefront holds\n  the whole customer-account surface.\nx-evidence:\n  fetched: '2026-08-07'\n  probes:\n  - url: https://shopbinske.com/.well-known/oauth-authorization-server\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/binske/refs/heads/main/scopes/binske-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- cannabis
- consumer-packaged-goods
- direct-to-consumer
- ecommerce
- retail
- shopify
- agent-commerce
- ucp
- mcp
- storefront
token_urls: []
---
