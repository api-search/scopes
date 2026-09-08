---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Zbiotics Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ZBiotics uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ZBiotics
provider_slug: zbiotics
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: zbiotics-scopes
source_filename: zbiotics-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: https://zbiotics.com/.well-known/openid-configuration\ndocs: null\nsummary: >-\n  Four OAuth scopes are advertised by the OIDC discovery document served on zbiotics.com and\n  account.zbiotics.com. They belong to the Shopify Customer Accounts identity that ZBiotics runs\n  on its own hosts, not to the anonymous UCP MCP commerce endpoint, which requires no scope. There\n  is no published scope reference page on the ZBiotics site - the discovery document is the only\n  place these are stated, so descriptions below are the standard meanings and are marked as such.\nflows:\n- type: authorization_code\n  authorization_url: https://account.zbiotics.com/authentication/oauth/authorize\n  token_url: https://account.zbiotics.com/authentication/oauth/token\n  pkce: S256\nscope_count: 4\nscopes:\n- name: openid\n  description: Standard OIDC scope requesting an ID token for the authenticated customer.\n  source: scopes_supported\n  description_source:\
  \ rfc-standard\n- name: email\n  description: Releases the customer's email and email_verified claims.\n  source: scopes_supported\n  description_source: rfc-standard\n- name: customer-account-api:full\n  description: >-\n    Full access to the Shopify Customer Account API for the signed-in customer - orders,\n    addresses, subscriptions and profile on this store.\n  source: scopes_supported\n  description_source: vendor-naming-convention\n- name: customer-account-mcp-api:full\n  description: >-\n    Full access to the Customer Account MCP API for the signed-in customer. This is the\n    authenticated counterpart to the anonymous storefront UCP MCP endpoint; it was not probed\n    because doing so requires a customer credential.\n  source: scopes_supported\n  description_source: vendor-naming-convention\ngaps:\n- >-\n  No scopes/permissions reference page exists on zbiotics.com. Descriptions above are inferred\n  from the scope names and the OIDC specification, not read from provider\
  \ prose.\nx-evidence:\n  fetched: '2026-09-05'\n  url: https://zbiotics.com/.well-known/openid-configuration\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zbiotics/refs/heads/main/scopes/zbiotics-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Biotechnology
- Probiotics
- Consumer Health
- Direct to Consumer
- E-Commerce
- Agentic Commerce
- Model Context Protocol
- Universal Commerce Protocol
- Shopify
- Company
token_urls: []
---
