---
api_specs:
- filename: curlec-razorpay-openapi.json
  format: json
  label: Razorpay Curlec REST API
  slug: razorpay-curlec-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curlec/refs/heads/main/openapi/curlec-razorpay-openapi.json
authorization_urls:
- https://mcp.razorpay.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Curlec Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Curlec publishes 1 OAuth 2.0 scope via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Curlec API on a user''s behalf.


  Tokens are issued from https://mcp.razorpay.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Curlec
provider_slug: curlec
schemes:
- description: OAuth 2.0 via the Razorpay MCP server (mcp.razorpay.com). Supports Authorization Code with PKCE (S256) for user-delegated access and Client Credentials for server-to-server access. Tokens expire in 3600 seconds. Dynamic Client Registration available at the registration endpoint. For integration setup see https://razorpay.com/docs/build/llm-docs/mcp-server/oauth.md.
  flows:
  - authorizationUrl: https://mcp.razorpay.com/authorize
    flow: authorizationCode
    tokenUrl: https://mcp.razorpay.com/token
  - flow: clientCredentials
    tokenUrl: https://mcp.razorpay.com/token
  name: oauth2
  source: openapi/curlec-razorpay-openapi.json
scope_count: 1
scope_names:
- read_only
scopes:
- description: Read-only access to Razorpay account data (payments, orders, refunds, payouts, subscriptions, invoices)
  flows:
  - authorizationCode
  - clientCredentials
  scope: read_only
slug: curlec-scopes
source_filename: curlec-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/curlec-razorpay-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/curlec-razorpay-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.razorpay.com/authorize\n    tokenUrl: https://mcp.razorpay.com/token\n  - flow: clientCredentials\n    tokenUrl: https://mcp.razorpay.com/token\n  description: OAuth 2.0 via the Razorpay MCP server (mcp.razorpay.com). Supports Authorization\n    Code with PKCE (S256) for user-delegated access and Client Credentials for server-to-server\n    access. Tokens expire in 3600 seconds. Dynamic Client Registration available at the registration\n    endpoint. For integration setup see https://razorpay.com/docs/build/llm-docs/mcp-server/oauth.md.\nscopes:\n- scope: read_only\n  description: Read-only access to Razorpay account data (payments, orders, refunds, payouts,\n    subscriptions, invoices)\n  flows:\n  - authorizationCode\n  - clientCredentials\n\
  \  sources:\n  - openapi/curlec-razorpay-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curlec/refs/heads/main/scopes/curlec-scopes.yml
summary_line: 1 scope · authorizationCode/clientCredentials
tags:
- Company
- Payments
- Payment Gateway
- Recurring Payments
- Subscriptions
- Direct Debit
- FinTech
- Malaysia
- DuitNow
- FPX
- Webhooks
- Razorpay
token_urls:
- https://mcp.razorpay.com/token
---
