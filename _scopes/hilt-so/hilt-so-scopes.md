---
api_specs:
- filename: hilt-so-openapi.yml
  format: yaml
  label: Hilt API (Pay API + Workspace)
  slug: hilt-pay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hilt-so/refs/heads/main/openapi/hilt-so-openapi.yml
- filename: hilt-so-transaction-evidence-openapi.yml
  format: yaml
  label: Hilt Solana Transaction Evidence API
  slug: transaction-evidence
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hilt-so/refs/heads/main/openapi/hilt-so-transaction-evidence-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.hilt.so/developers/pay-me-mcp
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Hilt So Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Hilt uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hilt
provider_slug: hilt-so
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: hilt-so-scopes
source_filename: hilt-so-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://api.hilt.so/.well-known/oauth-authorization-server (scopes_supported, probed 200); https://api.hilt.so/.well-known/oauth-protected-resource/mcp/pay-me;\n  https://docs.hilt.so/developers/pay-me-mcp (scope meanings); https://docs.hilt.so/developers/api-keys (API-key\n  permissions)\ndocs: https://docs.hilt.so/developers/pay-me-mcp\nspec_gap: openapi/hilt-so-openapi.yml declares no oauth2 securityScheme, so derive-oauth-scopes.py produced nothing;\n  the scope list is taken from the RFC 8414 document, which is authoritative.\noauth2:\n  authorization_server: https://api.hilt.so\n  authorization_endpoint: https://api.hilt.so/oauth/authorize\n  token_endpoint: https://api.hilt.so/oauth/token\n  registration_endpoint: https://api.hilt.so/oauth/register\n  revocation_endpoint: https://api.hilt.so/oauth/revoke\n  grant_types:\n  - authorization_code\n  - refresh_token\n  pkce:\n  - S256\n  token_endpoint_auth_methods:\n  -\
  \ none\n  resource: https://api.hilt.so/mcp/pay-me\n  scopes:\n  - scope: pay_me:read\n    description: Read connector-started payments and, when a receiving profile exists, received activity\n    tools:\n    - hilt_pay_me_account\n    - hilt_pay_me_get_payment\n    - hilt_pay_me_list_activity\n    - hilt_pay_me_list_payment_links\n    - hilt_pay_me_get_payment_link\n  - scope: pay_me:request\n    description: Create and manage self-shared payment links\n    tools:\n    - hilt_pay_me_create_payment_link\n    - hilt_pay_me_cancel_payment_link\n  - scope: pay_me:prepare\n    description: Start and manage wallet-approved payments to verified PayMe handles\n    tools:\n    - hilt_pay_me_resolve_handle\n    - hilt_pay_me_send_payment\n    - hilt_pay_me_cancel_payment\n  scope_count: 3\n  note: Tool-to-scope assignment is inferred from the docs' scope meanings and tool descriptions; the connector\n    schema is OAuth-gated so it was not confirmed against a live tools/list.\napi_key_permissions:\n\
  \  header: X-Hilt-Key\n  permissions:\n  - permission: access:read\n    description: Check entitlements and read Pay API rails\n  - permission: access:write\n    description: Create Pay API apps, products, and payment sessions\n  - permission: access:webhooks\n    description: Register webhook endpoints for Pay API flows\n  requested_via: requested_permissions[] on POST /v1/access/agent-bootstrap (MCP tool hilt_agent_bootstrap); requested_live_scopes[]\n    in the agent-setup example\n  guidance: Use the minimum permissions needed. Most server-side integrations need read; checkout creation or webhook\n    subscription workflows may also need execute.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hilt-so/refs/heads/main/scopes/hilt-so-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Payments
- Solana
- Stablecoins
- USDC
- Crypto Payments
- Agentic Payments
- x402
- Checkout
- Subscription
- Webhook
- MCP
- Entitlements
- Micropayments
- Developer Tools
- Fintech
token_urls: []
---
