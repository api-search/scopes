---
api_specs:
- filename: elemental-machines-api-openapi.yml
  format: yaml
  label: Elemental Machines API
  slug: elemental-machines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elemental-machines/refs/heads/main/openapi/elemental-machines-api-openapi.yml
authorization_urls:
- https://elementalmachines.com/oauth/authorize
description: ''
docs: ''
flows:
- password
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Elemental Machines Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Elemental Machines uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.elementalmachines.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Elemental Machines
provider_slug: elemental-machines
schemes:
- authorization_model: Tenancy-scoped, not scope-scoped. GET /api/machines/{uuid}.json and the alert-log operation both declare 403 Forbidden, which is the customer-group boundary being enforced. A single token carries every permission that user has.
  description: Resource Owner Password Credentials grant taking username, password, client_id, client_secret and grant_type. The provider's Swagger 1.2 declaration for /oauth/token declares no scope parameter and the authorizations block of the resource listing is null, so no scope can be requested and none is returned.
  flows:
  - flow: password
    scopes: {}
    tokenUrl: https://api.elementalmachines.io/oauth/token
  host: https://api.elementalmachines.io
  name: oauth2_password
  risk_note: An access token with no scope, carried in a query string, on a password grant, with no published expiry — every one of the four is a downgrade from current OAuth practice, and together they mean a leaked log line is a full-permission credential.
  scope_count: 0
  source: openapi/elemental-machines-api-openapi.yml
  surface: LabOps REST API
- client_id_metadata_document_supported: true
  dynamic_client_registration: false
  flows:
  - authorizationUrl: https://elementalmachines.com/oauth/authorize
    flow: authorizationCode
    pkce: S256
    refreshUrl: https://elementalmachines.com/oauth/token
    revocationUrl: https://elementalmachines.com/oauth/revoke
    scopes:
      mcp: The single scope advertised in scopes_supported by both the authorization-server metadata and the protected-resource metadata. Its meaning is not documented anywhere; it gates https://elementalmachines.com/wp-json/mcp/mcp-oauth-server.
    tokenUrl: https://elementalmachines.com/oauth/token
  host: https://elementalmachines.com
  http_status: 200
  name: mcp_oauth
  scope_count: 1
  source: https://elementalmachines.com/.well-known/oauth-authorization-server
  surface: WordPress MCP server
  token_endpoint_auth_methods_supported:
  - none
scope_count: 0
scope_names: []
scopes: []
slug: elemental-machines-scopes
source_filename: elemental-machines-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  openapi/elemental-machines-api-openapi.yml (derived baseline) +\n  https://elementalmachines.com/.well-known/oauth-authorization-server (HTTP 200) +\n  https://elementalmachines.com/.well-known/oauth-protected-resource (HTTP 200)\nsummary: >-\n  Two OAuth surfaces exist and they have completely different scope postures. The LabOps REST API at\n  api.elementalmachines.io uses an OAuth 2.0 password grant with an EMPTY scope set — the token is\n  all-or-nothing, and authorization is enforced entirely by customer-group tenancy (403 Forbidden on\n  another group's machine) rather than by scope. The WordPress MCP server on elementalmachines.com\n  publishes exactly one scope, \"mcp\", in its RFC 8414 metadata. No scopes/permissions reference page\n  exists anywhere in the provider's documentation.\nscope_count: 1\nschemes:\n- name: oauth2_password\n  surface: LabOps REST API\n  host: https://api.elementalmachines.io\n  source:\
  \ openapi/elemental-machines-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: https://api.elementalmachines.io/oauth/token\n    scopes: {}\n  scope_count: 0\n  description: >-\n    Resource Owner Password Credentials grant taking username, password, client_id, client_secret\n    and grant_type. The provider's Swagger 1.2 declaration for /oauth/token declares no scope\n    parameter and the authorizations block of the resource listing is null, so no scope can be\n    requested and none is returned.\n  authorization_model: >-\n    Tenancy-scoped, not scope-scoped. GET /api/machines/{uuid}.json and the alert-log operation both\n    declare 403 Forbidden, which is the customer-group boundary being enforced. A single token\n    carries every permission that user has.\n  risk_note: >-\n    An access token with no scope, carried in a query string, on a password grant, with no published\n    expiry — every one of the four is a downgrade from current OAuth practice, and together they\n\
  \    mean a leaked log line is a full-permission credential.\n- name: mcp_oauth\n  surface: WordPress MCP server\n  host: https://elementalmachines.com\n  source: https://elementalmachines.com/.well-known/oauth-authorization-server\n  http_status: 200\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://elementalmachines.com/oauth/authorize\n    tokenUrl: https://elementalmachines.com/oauth/token\n    refreshUrl: https://elementalmachines.com/oauth/token\n    revocationUrl: https://elementalmachines.com/oauth/revoke\n    pkce: S256\n    scopes:\n      mcp: >-\n        The single scope advertised in scopes_supported by both the authorization-server metadata\n        and the protected-resource metadata. Its meaning is not documented anywhere; it gates\n        https://elementalmachines.com/wp-json/mcp/mcp-oauth-server.\n  scope_count: 1\n  token_endpoint_auth_methods_supported: [none]\n  client_id_metadata_document_supported: true\n  dynamic_client_registration: false\n\
  docs: null\ndocs_note: >-\n  No scopes, permissions or access-control reference page is published. Neither\n  https://api.elementalmachines.io/ (the Swagger UI console) nor the Freshdesk knowledge base\n  documents what a token can and cannot reach.\ncross_links:\n  authentication: authentication/elemental-machines-authentication.yml\n  mcp: mcp/elemental-machines-mcp.yml\n  well_known: well-known/elemental-machines-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elemental-machines/refs/heads/main/scopes/elemental-machines-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- lab-operations
- laboratory-monitoring
- IoT
- Sensors
- Life Sciences
- Cold Chain
- Environmental Monitoring
- equipment-utilization
- Asset Management
- Alerting
- Compliance
- GxP
- Manufacturing
- Time Series
token_urls:
- https://api.elementalmachines.io/oauth/token
- https://elementalmachines.com/oauth/token
---
