---
authorization_urls: []
description: The only OAuth scopes L-Nutra advertises come from the Shopify customer-accounts OIDC discovery document served on each storefront. They govern a shopper signing into their own account, not a developer integration — there is no public client registration, so no third party can request them. Recorded verbatim from scopes_supported; L-Nutra publishes no scopes reference page of its own. The MCP endpoints themselves require no scope at all.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: L Nutra Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'L-Nutra uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: L-Nutra
provider_slug: l-nutra
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: l-nutra-scopes
source_filename: l-nutra-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: https://prolonlife.com/.well-known/openid-configuration\ndescription: >-\n  The only OAuth scopes L-Nutra advertises come from the Shopify customer-accounts OIDC discovery\n  document served on each storefront. They govern a shopper signing into their own account, not a\n  developer integration — there is no public client registration, so no third party can request\n  them. Recorded verbatim from scopes_supported; L-Nutra publishes no scopes reference page of its\n  own. The MCP endpoints themselves require no scope at all.\nauthorization_server: https://shopify.com/authentication/<shop-id>\ndocs: null\ndocs_note: No provider-published scope or permission reference exists.\nscopes:\n- name: openid\n  description: Standard OpenID Connect scope — request an ID token for the signed-in customer.\n  source: openid-configuration scopes_supported\n- name: email\n  description: Release the customer's email address and email_verified\
  \ claim.\n  source: openid-configuration scopes_supported\n- name: 'customer-account-api:full'\n  description: >-\n    Full access to the Shopify Customer Account API for the signed-in customer — their orders,\n    addresses, subscriptions and profile.\n  source: openid-configuration scopes_supported\n- name: 'customer-account-mcp-api:full'\n  description: >-\n    Full access to the Shopify Customer Account MCP API for the signed-in customer. This is the\n    authenticated, per-customer MCP surface, distinct from the anonymous storefront UCP endpoint.\n  source: openid-configuration scopes_supported\nhosts:\n- https://prolonlife.com\n- https://l-nutrahealth.com\n- https://l-nutraprofessional.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/l-nutra/refs/heads/main/scopes/l-nutra-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Nutrition
- Health
- Longevity
- Consumer Products
- E-Commerce
- Agentic Commerce
- Universal Commerce Protocol
- Model Context Protocol
- Shopify
token_urls: []
---
