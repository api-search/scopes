---
api_specs:
- filename: blnkfinance-accounts-api-openapi.yml
  format: yaml
  label: Blnk Finance Accounts API
  slug: blnkfinance-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blnkfinance/refs/heads/main/openapi/blnkfinance-accounts-api-openapi.yml
- filename: blnkfinance-backup-api-openapi.yml
  format: yaml
  label: Blnk Finance Backup API
  slug: blnkfinance-backup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blnkfinance/refs/heads/main/openapi/blnkfinance-backup-api-openapi.yml
- filename: blnkfinance-balance-monitors-api-openapi.yml
  format: yaml
  label: Blnk Finance Balance Monitors API
  slug: blnkfinance-balance-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blnkfinance/refs/heads/main/openapi/blnkfinance-balance-monitors-api-openapi.yml
- filename: blnkfinance-balances-api-openapi.yml
  format: yaml
  label: Blnk Finance Balances API
  slug: blnkfinance-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blnkfinance/refs/heads/main/openapi/blnkfinance-balances-api-openapi.yml
- filename: blnkfinance-identities-api-openapi.yml
  format: yaml
  label: Blnk Finance Identities API
  slug: blnkfinance-identities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blnkfinance/refs/heads/main/openapi/blnkfinance-identities-api-openapi.yml
- filename: blnkfinance-ledgers-api-openapi.yml
  format: yaml
  label: Blnk Finance Ledgers API
  slug: blnkfinance-ledgers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blnkfinance/refs/heads/main/openapi/blnkfinance-ledgers-api-openapi.yml
- filename: blnkfinance-refund-transaction-api-openapi.yml
  format: yaml
  label: Blnk Finance Refund Transaction API
  slug: blnkfinance-refund-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blnkfinance/refs/heads/main/openapi/blnkfinance-refund-transaction-api-openapi.yml
- filename: blnkfinance-transactions-api-openapi.yml
  format: yaml
  label: Blnk Finance Transactions API
  slug: blnkfinance-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blnkfinance/refs/heads/main/openapi/blnkfinance-transactions-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.blnkfinance.com/api-keys/scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Blnkfinance Scopes
name_suffix: OAuth Scopes
note: Blnk Core's scope model is attached to API KEYS, not to an OAuth flow -- derive-oauth-scopes.py found nothing because the published OpenAPI declares only http/basic and no oauth2 securityScheme. The model is real and fully documented anyway, and it is the same vocabulary the Blnk Cloud OAuth clients use, so it is captured here. Scopes are `resource:action` pairs; Blnk maps HTTP methods to actions automatically rather than naming a scope per endpoint, so the scope list is a small grid rather than a long registry.
overview: 'Blnk Finance publishes 24 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Blnk Finance API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Blnk Finance
provider_slug: blnkfinance
schemes: []
scope_count: 24
scope_names:
- ledgers:read
- ledgers:write
- balances:read
- balances:write
- accounts:read
- accounts:write
- identities:read
- identities:write
- identities:delete
- transactions:read
- transactions:write
- balance-monitors:read
- balance-monitors:write
- balance-monitors:delete
- api-keys:read
- api-keys:write
- api-keys:delete
- search:read
- reconciliation:read
- reconciliation:write
- metadata:write
- backup:write
- mcp:read
- mcp:write
scopes:
- description: View ledgers
  flows: []
  scope: ledgers:read
- description: Create ledgers
  flows: []
  scope: ledgers:write
- description: View balances
  flows: []
  scope: balances:read
- description: Create and update balances
  flows: []
  scope: balances:write
- description: View accounts
  flows: []
  scope: accounts:read
- description: Create and update accounts
  flows: []
  scope: accounts:write
- description: View identities
  flows: []
  scope: identities:read
- description: Create and update identities
  flows: []
  scope: identities:write
- description: Delete identities
  flows: []
  scope: identities:delete
- description: View transactions
  flows: []
  scope: transactions:read
- description: Create transactions
  flows: []
  scope: transactions:write
- description: View balance monitors
  flows: []
  scope: balance-monitors:read
- description: Create and update balance monitors
  flows: []
  scope: balance-monitors:write
- description: Delete balance monitors
  flows: []
  scope: balance-monitors:delete
- description: List API keys within the owner context
  flows: []
  scope: api-keys:read
- description: Create API keys within the owner context
  flows: []
  scope: api-keys:write
- description: Revoke API keys within the owner context
  flows: []
  scope: api-keys:delete
- description: Run search queries
  flows: []
  scope: search:read
- description: View reconciliation runs and rules
  flows: []
  scope: reconciliation:read
- description: Start reconciliations and manage matching rules
  flows: []
  scope: reconciliation:write
- description: Update metadata on ledgers
  flows: []
  scope: metadata:write
- description: Trigger database backups
  flows: []
  scope: backup:write
- description: Read-only access to ledger data through Blnk Cloud MCP tools
  flows: []
  scope: mcp:read
- description: Read and write access through Blnk Cloud MCP tools
  flows: []
  scope: mcp:write
slug: blnkfinance-scopes
source_filename: blnkfinance-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: >-\n  https://docs.blnkfinance.com/api-keys/scopes, https://docs.blnkfinance.com/cloud/integrations/mcp,\n  https://docs.blnkfinance.com/cloud/auth/api-keys\ndocs: https://docs.blnkfinance.com/api-keys/scopes\nnote: >-\n  Blnk Core's scope model is attached to API KEYS, not to an OAuth flow -- derive-oauth-scopes.py found\n  nothing because the published OpenAPI declares only http/basic and no oauth2 securityScheme. The model\n  is real and fully documented anyway, and it is the same vocabulary the Blnk Cloud OAuth clients use,\n  so it is captured here. Scopes are `resource:action` pairs; Blnk maps HTTP methods to actions\n  automatically rather than naming a scope per endpoint, so the scope list is a small grid rather than a\n  long registry.\nmodel:\n  format: resource:action\n  wildcard: '*'\n  wildcard_note: 'Either side may be *: ledgers:* grants all ledger actions, *:read grants read on every resource.'\n  method_mapping:\n\
  \  - {action: read, http_methods: [GET, HEAD]}\n  - {action: write, http_methods: [POST, PUT, PATCH]}\n  - {action: delete, http_methods: [DELETE]}\n  - {action: '*', http_methods: [any]}\nresources:\n- {resource: '*', description: All resources}\n- {resource: ledgers, description: Ledger management}\n- {resource: balances, description: Balance operations}\n- {resource: accounts, description: Account operations}\n- {resource: identities, description: Identity management}\n- {resource: transactions, description: Transaction processing}\n- {resource: balance-monitors, description: Balance monitoring}\n- {resource: api-keys, description: API key management}\n- {resource: search, description: Search operations}\n- {resource: reconciliation, description: Reconciliation tasks}\n- {resource: metadata, description: 'Metadata management (POST /{id}/metadata maps here)'}\n- {resource: backup, description: Backup operations}\nscopes:\n- {scope: 'ledgers:read', description: View ledgers}\n- {scope:\
  \ 'ledgers:write', description: Create ledgers}\n- {scope: 'balances:read', description: View balances}\n- {scope: 'balances:write', description: Create and update balances}\n- {scope: 'accounts:read', description: View accounts}\n- {scope: 'accounts:write', description: Create and update accounts}\n- {scope: 'identities:read', description: View identities}\n- {scope: 'identities:write', description: Create and update identities}\n- {scope: 'identities:delete', description: Delete identities}\n- {scope: 'transactions:read', description: View transactions}\n- {scope: 'transactions:write', description: Create transactions, commit/void inflight, refund}\n- {scope: 'balance-monitors:read', description: View balance monitors}\n- {scope: 'balance-monitors:write', description: Create and update balance monitors}\n- {scope: 'balance-monitors:delete', description: Delete balance monitors}\n- {scope: 'api-keys:read', description: List API keys within the owner context}\n- {scope: 'api-keys:write',\
  \ description: Create API keys within the owner context}\n- {scope: 'api-keys:delete', description: Revoke API keys within the owner context}\n- {scope: 'search:read', description: Run search queries}\n- {scope: 'reconciliation:read', description: View reconciliation runs and rules}\n- {scope: 'reconciliation:write', description: Start reconciliations and manage matching rules}\n- {scope: 'metadata:write', description: Update metadata on ledgers, transactions, identities and balances}\n- {scope: 'backup:write', description: Trigger database backups}\n- {scope: 'mcp:read', description: Read-only access to ledger data through Blnk Cloud MCP tools, surface: blnk-cloud}\n- {scope: 'mcp:write', description: Read and write access through Blnk Cloud MCP tools, surface: blnk-cloud}\nscope_derivation_note: >-\n  The resource list and the action grid are published verbatim by Blnk; the individual resource:action\n  rows above are the documented cross-product of the two, restricted to the actions\
  \ each resource's\n  documented operations actually support. mcp:read and mcp:write are named explicitly in the Cloud MCP\n  docs. No scope here was invented.\ndocumented_patterns:\n- {use_case: Read-only reporting, scopes: ['ledgers:read', 'balances:read']}\n- {use_case: Payment processing, scopes: ['transactions:write', 'balances:read']}\n- {use_case: Identity management, scopes: ['identities:write', 'identities:read']}\n- {use_case: Metadata updates, scopes: ['metadata:write']}\n- {use_case: Key administration, scopes: ['api-keys:read', 'api-keys:write', 'api-keys:delete']}\n- {use_case: AI agent over MCP, scopes: ['mcp:read', 'mcp:write']}\nguidance:\n  least_privilege: 'Blnk explicitly warns against *:* unless full access is genuinely needed.'\n  escalation_guard: 'A non-master key cannot grant scopes broader than its own (AUTH_SCOPE_ESCALATION, 403), since 0.14.3.'\n  owner_scoping: 'A non-master key is limited to its own owner_id for key management (AUTH_CROSS_OWNER_ACCESS, 403).'\n\
  \  master_key_only:\n  - Hook management (create, update, view, list, delete) -- scoped keys get AUTH_MASTER_KEY_REQUIRED 403.\nerrors:\n- {code: AUTH_INSUFFICIENT_PERMISSIONS, status: 403, meaning: The key is missing the scope required for that endpoint}\n- {code: AUTH_UNKNOWN_RESOURCE, status: 403, meaning: The request path does not map to a known Blnk resource}\n- {code: AUTH_MASTER_KEY_REQUIRED, status: 403, meaning: The endpoint requires the master key}\n- {code: AUTH_SCOPE_ESCALATION, status: 403, meaning: Attempt to grant scopes broader than the caller's}\noauth:\n  supported: true\n  surface: Blnk Cloud\n  metadata_document: well-known/blnkfinance-oauth-authorization-server.json\n  issuer: https://api.cloud.blnkfinance.com\n  authorization_endpoint: https://api.cloud.blnkfinance.com/oauth/authorize\n  token_endpoint: https://api.cloud.blnkfinance.com/oauth/token\n  grant_types: [authorization_code, refresh_token]\n  pkce: [S256, plain]\n  token_endpoint_auth_methods: [client_secret_post,\
  \ client_secret_basic]\n  docs: https://docs.blnkfinance.com/cloud/auth/oauth\n  note: >-\n    The RFC 8414 metadata document declares no scopes_supported field, so the OAuth scope vocabulary is\n    only discoverable from the docs (mcp:read / mcp:write are the ones named).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blnkfinance/refs/heads/main/scopes/blnkfinance-scopes.yml
summary_line: 24 scopes
tags:
- Fintech
- Financial-Services
- Ledger
- double-entry-accounting
- Payments
- Wallets
- Lending
- Banking Infrastructure
- Open-Source
- MCP
- AI Agents
- Developer Tools
token_urls: []
---
