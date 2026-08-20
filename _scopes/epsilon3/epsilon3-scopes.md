---
authorization_urls:
- https://app.epsilon3.io/oauth/authorize
- https://api.epsilon3.io/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Epsilon3 Scopes
name_suffix: OAuth Scopes
note: 'Epsilon3 publishes no OpenAPI, so derive-oauth-scopes.py had nothing to read. These fifteen scopes are the verbatim scopes_supported array served by Epsilon3''s own RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata. The identical set is advertised on four hosts: mcp.epsilon3.io, api.epsilon3.io, app.epsilon3.io and api.uk.epsilon3.io. No scopes reference page exists in the API Guide, so the DESCRIPTIONS below are read from the scope names and the documented REST surface they correspond to - they are not provider prose.'
overview: 'Epsilon3 publishes 15 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Epsilon3 API on a user''s behalf.


  Tokens are issued from https://app.epsilon3.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Epsilon3
provider_slug: epsilon3
schemes:
- authorization_servers:
  - https://app.epsilon3.io
  bearer_methods_supported:
  - header
  flows:
  - authorizationUrl: https://app.epsilon3.io/oauth/authorize
    code_challenge_methods_supported:
    - S256
    flow: authorizationCode
    registrationUrl: https://app.epsilon3.io/oauth/register
    tokenUrl: https://app.epsilon3.io/oauth/token
  name: MCPOAuth
  resource: https://mcp.epsilon3.io
  source: well-known/epsilon3-mcp-oauth-protected-resource.json
- flows:
  - authorizationUrl: https://api.epsilon3.io/oauth/authorize
    flow: authorizationCode
    registrationUrl: https://api.epsilon3.io/oauth/register
    tokenUrl: https://api.epsilon3.io/oauth/token
  issuer: https://api.epsilon3.io
  name: PlatformOAuth
  source: well-known/epsilon3-oauth-authorization-server.json
scope_count: 15
scope_names:
- procedures:read
- procedures:comment
- procedures:draft
- procedures:signoff
- runs:read
- runs:comment
- runs:start
- issues:read
- issues:comment
- issues:write
- parts:read
- work_orders:read
- work_orders:write
- shift_logs:read
- shift_logs:write
scopes:
- description: Read procedures and procedure summaries.
  flows: []
  scope: procedures:read
- description: Add comments to a procedure.
  flows: []
  scope: procedures:comment
- description: Create or modify draft (unreleased) procedure versions.
  flows: []
  scope: procedures:draft
- description: Sign off procedure steps - the highest-consequence scope in the set, because a signoff is the auditable record that a step was performed correctly.
  flows: []
  scope: procedures:signoff
- description: Read running and completed procedure runs.
  flows: []
  scope: runs:read
- description: Add comments to a run.
  flows: []
  scope: runs:comment
- description: Start a procedure run.
  flows: []
  scope: runs:start
- description: Read issues and issue metadata options.
  flows: []
  scope: issues:read
- description: Add comments to an issue.
  flows: []
  scope: issues:comment
- description: Create and update issues.
  flows: []
  scope: issues:write
- description: Read parts, part details and inventory.
  flows: []
  scope: parts:read
- description: Read work orders.
  flows: []
  scope: work_orders:read
- description: Create and update work orders.
  flows: []
  scope: work_orders:write
- description: Read shift logs.
  flows: []
  scope: shift_logs:read
- description: Create and update shift log entries.
  flows: []
  scope: shift_logs:write
slug: epsilon3-scopes
source_filename: epsilon3-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://mcp.epsilon3.io/.well-known/oauth-protected-resource\nnote: >-\n  Epsilon3 publishes no OpenAPI, so derive-oauth-scopes.py had nothing to read. These\n  fifteen scopes are the verbatim scopes_supported array served by Epsilon3's own RFC\n  8414 authorization-server metadata and RFC 9728 protected-resource metadata. The\n  identical set is advertised on four hosts: mcp.epsilon3.io, api.epsilon3.io,\n  app.epsilon3.io and api.uk.epsilon3.io. No scopes reference page exists in the API\n  Guide, so the DESCRIPTIONS below are read from the scope names and the documented REST\n  surface they correspond to - they are not provider prose.\ndocs: null\ndocs_gap: >-\n  Epsilon3 documents no scopes/permissions reference page. The only public description\n  of these scopes is the machine-readable metadata itself.\nschemes:\n- name: MCPOAuth\n  source: well-known/epsilon3-mcp-oauth-protected-resource.json\n  resource: https://mcp.epsilon3.io\n\
  \  authorization_servers: [https://app.epsilon3.io]\n  bearer_methods_supported: [header]\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.epsilon3.io/oauth/authorize\n    tokenUrl: https://app.epsilon3.io/oauth/token\n    registrationUrl: https://app.epsilon3.io/oauth/register\n    code_challenge_methods_supported: [S256]\n- name: PlatformOAuth\n  source: well-known/epsilon3-oauth-authorization-server.json\n  issuer: https://api.epsilon3.io\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.epsilon3.io/oauth/authorize\n    tokenUrl: https://api.epsilon3.io/oauth/token\n    registrationUrl: https://api.epsilon3.io/oauth/register\nscope_count: 15\nscopes:\n- scope: procedures:read\n  access: read\n  domain: procedures\n  description: Read procedures and procedure summaries.\n- scope: procedures:comment\n  access: write\n  domain: procedures\n  description: Add comments to a procedure.\n- scope: procedures:draft\n  access: write\n  domain:\
  \ procedures\n  description: Create or modify draft (unreleased) procedure versions.\n- scope: procedures:signoff\n  access: write\n  domain: procedures\n  description: Sign off procedure steps - the highest-consequence scope in the set,\n    because a signoff is the auditable record that a step was performed correctly.\n- scope: runs:read\n  access: read\n  domain: runs\n  description: Read running and completed procedure runs.\n- scope: runs:comment\n  access: write\n  domain: runs\n  description: Add comments to a run.\n- scope: runs:start\n  access: write\n  domain: runs\n  description: Start a procedure run.\n- scope: issues:read\n  access: read\n  domain: issues\n  description: Read issues and issue metadata options.\n- scope: issues:comment\n  access: write\n  domain: issues\n  description: Add comments to an issue.\n- scope: issues:write\n  access: write\n  domain: issues\n  description: Create and update issues.\n- scope: parts:read\n  access: read\n  domain: builds\n  description:\
  \ Read parts, part details and inventory.\n- scope: work_orders:read\n  access: read\n  domain: builds\n  description: Read work orders.\n- scope: work_orders:write\n  access: write\n  domain: builds\n  description: Create and update work orders.\n- scope: shift_logs:read\n  access: read\n  domain: operations\n  description: Read shift logs.\n- scope: shift_logs:write\n  access: write\n  domain: operations\n  description: Create and update shift log entries.\nsummary:\n  read_scopes: 6\n  write_scopes: 9\n  domains: [procedures, runs, issues, builds, operations]\n  observation: >-\n    Nine write scopes are advertised but the current MCP preview exposes no write tool,\n    so the granted authority of a token materially exceeds what any published client can\n    exercise today. There is no scope covering the large Builds write surface (purchase\n    orders, sale orders, tooling, shipments), Test Management, Project Schedule,\n    Telemetry or Commanding - those remain API-key-only.\nx-evidence:\n\
  \  fetched: '2026-08-12'\n  probes:\n  - {url: 'https://mcp.epsilon3.io/.well-known/oauth-protected-resource', http_status: 200}\n  - {url: 'https://mcp.epsilon3.io/.well-known/oauth-authorization-server', http_status: 200}\n  - {url: 'https://api.epsilon3.io/.well-known/oauth-authorization-server', http_status: 200}\n  - {url: 'https://api.uk.epsilon3.io/.well-known/oauth-authorization-server', http_status: 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/epsilon3/refs/heads/main/scopes/epsilon3-scopes.yml
summary_line: 15 scopes · authorizationCode
tags:
- Company
- Aerospace
- Space
- Defense
- Manufacturing
- Procedures
- Workflows
- Inventory
- Telemetry
- Test Management
- Project Management
- MCP
token_urls:
- https://app.epsilon3.io/oauth/token
- https://api.epsilon3.io/oauth/token
---
