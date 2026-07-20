---
api_specs:
- filename: bridge-openapi-original.json
  format: json
  label: Bridge API
  slug: bridge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge/refs/heads/main/openapi/bridge-openapi-original.json
authorization_urls: []
description: ''
docs: https://apidocs.bridge.xyz/api-reference/api-keys/create-a-scoped-api-key
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Bridge Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Bridge uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bridge
provider_slug: bridge
schemes:
- in: header
  name: ApiKey
  parameter: Api-Key
  source: openapi/bridge-openapi-original.json
  type: apiKey
scope_count: 0
scope_names: []
scopes: []
slug: bridge-scopes
source_filename: bridge-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/bridge-openapi-original.json (components.schemas.ApiKeyScope)\ndocs: https://apidocs.bridge.xyz/api-reference/api-keys/create-a-scoped-api-key\nmodel: api-key-scopes\nnotes: >\n  Bridge does not use OAuth2. It issues static API keys that may be restricted to\n  a subset of scopes (\"scoped API keys\"). Callers may only grant scopes they\n  themselves hold (scope subsetting); unrestricted keys may create scoped keys,\n  while scoped keys need the api_key:create scope. Up to 500 scoped keys may exist\n  per developer. Scopes below are enumerated verbatim from the ApiKeyScope enum in\n  the published OpenAPI. Scopes follow a resource:action (and resource:sub:action)\n  convention.\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: Api-Key\n  source: openapi/bridge-openapi-original.json\nscopes:\n- api_key:create\n- api_key:self:read\n- audit_log:read\n- batch_settlement:create\n- batch_settlement:read\n\
  - card:create\n- card:delete\n- card:read\n- card:update\n- crypto_return_policy:create\n- crypto_return_policy:delete\n- crypto_return_policy:read\n- crypto_return_policy:update\n- customer:create\n- customer:delete\n- customer:read\n- customer:update\n- customer_creation_request:create\n- customer_creation_request:read\n- developer_fee:create\n- developer_fee:read\n- developer_fee:update\n- developer_trade_configuration:read\n- developer_trade_configuration:update\n- exchange_rate:read\n- external_account:create\n- external_account:delete\n- external_account:read\n- external_account:update\n- inquiry:read\n- inquiry:resume\n- liquidation_address:create\n- liquidation_address:drain:read\n- liquidation_address:drain:update\n- liquidation_address:read\n- liquidation_address:update\n- prefunded_account:create\n- prefunded_account:history:read\n- prefunded_account:read\n- rewards:read\n- sandbox:simulate\n- spender_contract:approval:create\n- spender_contract:approval:read\n- spender_contract:create\n\
  - spender_contract:read\n- tos_link:create\n- tos_link:read\n- transfer:create\n- transfer:create:privy_custodial_wallet\n- transfer:delete\n- transfer:read\n- transfer:update\n- virtual_account:create\n- virtual_account:delete\n- virtual_account:history:read\n- virtual_account:read\n- virtual_account:transaction:read\n- virtual_account:update\n- wallet:create\n- wallet:create:privy_custodial_wallet\n- wallet:customer:read\n- wallet:delete\n- wallet:developer:read\n- wallet:update\n- webhook:create\n- webhook:delete\n- webhook:read\n- webhook:update\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bridge/refs/heads/main/scopes/bridge-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Crypto
- Stablecoins
- Payments
- Money Movement
- Cross-Border Payments
- Virtual Accounts
- Wallets
- Cards
- Fintech
token_urls: []
---
