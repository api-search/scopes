---
api_specs:
- filename: lili-lili-api-openapi.yml
  format: yaml
  label: Lili Lili API
  slug: lili-lili-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lili/refs/heads/main/openapi/lili-lili-api-openapi.yml
authorization_urls: []
description: ''
docs: https://dev.lili.co/guides/lili-mcp-connect
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Lili Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Lili uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Lili
provider_slug: lili
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: lili-scopes
source_filename: lili-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: https://mcp.lili.co/.well-known/oauth-authorization-server\ndocs: https://dev.lili.co/guides/lili-mcp-connect\nsummary: >-\n  Lili runs a real OAuth 2.0 authorization server for its MCP endpoint, and that server declares NO\n  scopes. Authorization is all-or-nothing per authenticated user: consenting once grants an agent\n  every one of the 44 tools, including full transaction history, statements, tax filings, beneficial\n  owners and — for accountants — every connected client's data.\nauthorization_server:\n  issuer: https://mcp.lili.co\n  metadata: well-known/lili-mcp-oauth-authorization-server.json\n  metadata_http_status: 200\n  authorization_endpoint: https://mcp.lili.co/oauth/authorize\n  token_endpoint: https://mcp.lili.co/oauth/token\n  revocation_endpoint: https://mcp.lili.co/oauth/revoke\n  registration_endpoint: https://mcp.lili.co/oauth/register\n  response_types_supported: [code]\n  grant_types_supported: [authorization_code,\
  \ refresh_token]\n  code_challenge_methods_supported: [S256]\n  token_endpoint_auth_methods_supported: [none]\n  scopes_supported: null\nprotected_resource:\n  metadata: well-known/lili-mcp-oauth-protected-resource.json\n  metadata_http_status: 200\n  resource: https://mcp.lili.co\n  bearer_methods_supported: [header]\n  authorization_servers:\n  - https://mcp.lili.co\n  - https://mcp.lilibanking.com\n  - http://mcp.lilibanking.com:8080\n  - http://localhost:8080\n  - http://127.0.0.1:8080\n  hygiene_finding: >-\n    Three of the six declared authorization_servers are non-production values (two localhost, one\n    plaintext http on the retired lilibanking domain) shipping in live RFC 9728 discovery metadata.\nscope_count: 0\nscopes: []\nscopes_note: >-\n  `scopes_supported` is absent from the RFC 8414 metadata and no scope, permission or consent\n  reference page exists anywhere on dev.lili.co or lili.co. This is recorded as a measured zero, not\n  as an unchecked field.\neffective_authorization:\n\
  \  model: user-identity\n  detail: >-\n    Lili's own documentation states that \"access tokens are scoped to the authenticated user\".\n    The only differentiation is USER TYPE, enforced server-side rather than by scope: a business\n    user reaches their own account without a businessUserId, while an accountant must pass\n    businessUserId (or call select_customer) and is additionally granted the nine Accountant Tools.\n  revocation: https://mcp.lili.co/oauth/revoke\n  refresh: Refresh tokens are issued automatically; users typically log in once per device.\n  source: https://dev.lili.co/guides/lili-mcp-connect\nrest_api:\n  oauth2: false\n  note: >-\n    The three partner REST APIs do not use OAuth at all — they authenticate with a static\n    accessKey:secretKey pair in the Authorization header, which carries no scope concept either.\n    See authentication/lili-authentication.yml.\nchecked: '2026-08-25'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lili/refs/heads/main/scopes/lili-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- banking
- business-banking
- Financial-Services
- Fintech
- embedded-finance
- Onboarding
- kyc
- Webhook
- MCP
- agent-native
- Invoicing
- bill-pay
- accounting
- small-business
token_urls: []
---
