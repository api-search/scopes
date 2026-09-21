---
api_specs:
- filename: getemboss-ai-account-openapi.yml
  format: yaml
  label: Emboss Account API
  slug: emboss-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getemboss-ai/refs/heads/main/openapi/getemboss-ai-account-openapi.yml
- filename: getemboss-ai-pay-per-call-openapi.yml
  format: yaml
  label: Emboss Pay-per-call API
  slug: emboss-pay-per-call-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getemboss-ai/refs/heads/main/openapi/getemboss-ai-pay-per-call-openapi.yml
authorization_urls:
- https://api.getemboss.ai/oauth/authorize
description: ''
docs: https://getemboss.ai/docs/mcp-tools#scopes
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Getemboss Ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Emboss publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Emboss API on a user''s behalf.


  Tokens are issued from https://api.getemboss.ai/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Emboss
provider_slug: getemboss-ai
schemes:
- description: Sign in with your Emboss account. Used by MCP clients and A2A clients; the account REST API also accepts an OAuth token per the spec's global security.
  flows:
  - authorizationUrl: https://api.getemboss.ai/oauth/authorize
    flow: authorizationCode
    pkce: S256
    refresh: true
    registration_endpoint: https://api.getemboss.ai/oauth/register
    revocation_endpoint: https://api.getemboss.ai/oauth/revoke
    tokenUrl: https://api.getemboss.ai/oauth/token
    token_endpoint_auth_methods:
    - none
    - client_secret_post
  issuer: https://api.getemboss.ai
  name: oauth2
  resources:
  - https://api.getemboss.ai/mcp
  - https://api.getemboss.ai/a2a
  - 'https://api.getemboss.ai (account API — spec global security [{bearer}, {oauth2: [forms:read, forms:write]}])'
  source: openapi/getemboss-ai-account-openapi.yml
scope_count: 2
scope_names:
- forms:read
- forms:write
scopes:
- description: Read your forms
  flows:
  - authorizationCode
  scope: forms:read
- description: Create and fill forms
  flows:
  - authorizationCode
  scope: forms:write
slug: getemboss-ai-scopes
source_filename: getemboss-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/getemboss-ai-account-openapi.yml (derived baseline by derive-oauth-scopes.py) upgraded from https://getemboss.ai/docs/mcp-tools and the live RFC 8414 / RFC 9728 metadata under well-known/\ndocs: https://getemboss.ai/docs/mcp-tools#scopes\ndiscovery:\n  authorization_server_metadata: well-known/getemboss-ai-oauth-authorization-server.json\n  protected_resource_metadata: well-known/getemboss-ai-oauth-protected-resource-mcp.json\n  scopes_supported: [forms:read, forms:write]\n  note: Both discovery documents list exactly the two scopes the spec declares; there are no hidden or undocumented scopes.\nschemes:\n- name: oauth2\n  source: openapi/getemboss-ai-account-openapi.yml\n  issuer: https://api.getemboss.ai\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.getemboss.ai/oauth/authorize\n    tokenUrl: https://api.getemboss.ai/oauth/token\n    pkce: S256\n    refresh: true\n    registration_endpoint:\
  \ https://api.getemboss.ai/oauth/register\n    revocation_endpoint: https://api.getemboss.ai/oauth/revoke\n    token_endpoint_auth_methods: [none, client_secret_post]\n  description: Sign in with your Emboss account. Used by MCP clients and A2A clients; the account REST API also accepts an OAuth token per the spec's global security.\n  resources:\n  - https://api.getemboss.ai/mcp\n  - https://api.getemboss.ai/a2a\n  - 'https://api.getemboss.ai (account API — spec global security [{bearer}, {oauth2: [forms:read, forms:write]}])'\nscopes:\n- scope: forms:read\n  description: Read your forms\n  flows: [authorizationCode]\n  sources: [openapi/getemboss-ai-account-openapi.yml, well-known/getemboss-ai-oauth-authorization-server.json]\n  grants_mcp_tools: [list_forms, get_form, get_usage, find_form, get_job, get_batch, get_proposal, get_fax]\n- scope: forms:write\n  description: Create and fill forms\n  flows: [authorizationCode]\n  sources: [openapi/getemboss-ai-account-openapi.yml, well-known/getemboss-ai-oauth-authorization-server.json]\n\
  \  grants_mcp_tools: [create_form, delete_form, fill_form, fill_form_from_context, prepare_form, commit_proposal, verify_form, read_form, add_attachment, suggest_mapping, fill_batch, send_fax]\n  note: '\"everything else\" per the docs — delete_form, read_form and add_attachment sit under write even though delete and attach are free and read_form stores nothing.'\nbehaviour:\n  insufficient_scope: A tool call that needs a scope the connection does not have returns insufficient_scope; the fix is to disconnect (Dashboard > Account > Connected apps) and reconnect granting both permissions.\n  api_key_equivalence: An API key (sk_live_) is not scoped — it carries the whole owner's surface; the agent card's securityRequirements nonetheless list both scope names under bearer as well as oauth2.\n  granularity_gap: Two scopes cover a 20-tool / 115-operation surface; there is no per-resource or read-only-billing scope, and no scope distinguishes the paid writes (fill, fax) from the free ones (delete,\
  \ attach).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getemboss-ai/refs/heads/main/scopes/getemboss-ai-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- PDF
- Forms
- Document Processing
- Form Filling
- Fax
- Data Extraction
- agent-native
- MCP
- A2A
- x402
- pay-per-call
- Government Forms
- Company
token_urls:
- https://api.getemboss.ai/oauth/token
---
