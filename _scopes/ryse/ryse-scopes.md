---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Ryse Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'RYSE uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: RYSE
provider_slug: ryse
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: ryse-scopes
source_filename: ryse-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://account.helloryse.com/.well-known/oauth-authorization-server\ndocs: null\ndocs_note: >-\n  RYSE publishes no scopes/permissions reference page of its own. The scope list below is read\n  verbatim from the scopes_supported array of RYSE's own OAuth 2.0 authorization-server metadata\n  document, fetched anonymously on 2026-08-26 (HTTP 200).\nauthorization_server: https://account.helloryse.com\nissuer: https://shopify.com/authentication/51479806112\nauthorization_url: https://account.helloryse.com/authentication/oauth/authorize\ntoken_url: https://account.helloryse.com/authentication/oauth/token\nflow: authorization_code\npkce: S256\nscope_count: 4\nscopes:\n- name: openid\n  description: >-\n    Standard OpenID Connect scope. Requests an ID token identifying the RYSE customer.\n  standard: OpenID Connect Core 1.0\n- name: email\n  description: >-\n    Standard OpenID Connect scope. Releases the email and email_verified\
  \ claims for the RYSE\n    customer.\n  standard: OpenID Connect Core 1.0\n- name: customer-account-api:full\n  description: >-\n    Full access to the RYSE customer-account API on behalf of the signed-in customer — orders,\n    profile, addresses, store credit. Observed in the live login redirect on\n    https://www.helloryse.com/account/login.\n  granularity: coarse\n  note: >-\n    There is no read-only or per-resource variant published; the only offered granularity is \":full\".\n- name: customer-account-mcp-api:full\n  description: >-\n    Full access to the customer-account MCP surface at\n    https://account.helloryse.com/customer/api/mcp — the scope an agent needs to actually execute\n    get_most_recent_order_status, get_order_status, get_store_credit_balances and request_return.\n  granularity: coarse\n  covers_tools:\n  - get_most_recent_order_status\n  - get_order_status\n  - get_store_credit_balances\n  - request_return\nunscoped_surfaces:\n- endpoint: https://www.helloryse.com/api/ucp/mcp\n\
  \  reason: >-\n    The UCP commerce MCP is anonymous. It has no OAuth scopes at all; admission is controlled by a\n    dereferenceable UCP agent profile (meta[\"ucp-agent\"].profile), not by a token.\n- endpoint: https://www.helloryse.com/api/mcp\n  reason: The Storefront MCP is anonymous and carries no OAuth surface.\nfindings:\n- >-\n  Coarse-only. Both RYSE-specific scopes end in \":full\" — an agent that needs to read one order\n  status must be granted the same scope that authorizes request_return, a write. There is no\n  least-privilege option for an agent operating on a customer's behalf.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ryse/refs/heads/main/scopes/ryse-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Smart Home
- Internet of Things
- Consumer Electronics
- Home Automation
- Window Coverings
- Agentic Commerce
- Model Context Protocol
- Universal Commerce Protocol
- E-commerce
- Shopify
token_urls: []
---
