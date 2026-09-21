---
api_specs:
- filename: relmcrm-com-openapi.yml
  format: yaml
  label: Relm CRM REST API
  slug: relm-crm-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relmcrm-com/refs/heads/main/openapi/relmcrm-com-openapi.yml
authorization_urls:
- https://api.relmcrm.com/oauth/authorize
description: ''
docs: https://relmcrm.com/docs
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Relmcrm Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Relm publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Relm API on a user''s behalf.


  Tokens are issued from https://api.relmcrm.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Relm
provider_slug: relmcrm-com
schemes:
- code_challenge_methods_supported:
  - S256
  description: 'OAuth 2.1 with PKCE (S256) and dynamic client registration (RFC 7591). Live mode only; test mode is API-key only. Discovery: /.well-known/oauth-authorization-server.'
  discovery:
    authorization_server: well-known/relmcrm-com-oauth-authorization-server.json
    protected_resource: well-known/relmcrm-com-oauth-protected-resource.json
    resource: https://api.relmcrm.com/mcp
  dynamic_client_registration: RFC 7591 — clients register themselves; the dashboard lists connected apps and disconnecting one revokes all of its access immediately (changelog v0.17.0)
  flows:
  - authorizationUrl: https://api.relmcrm.com/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://api.relmcrm.com/oauth/token
    tokenUrl: https://api.relmcrm.com/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  issuer: https://api.relmcrm.com
  live_only: true
  name: oauth2
  registration_endpoint: https://api.relmcrm.com/oauth/register
  response_types_supported:
  - code
  revocation_endpoint: https://api.relmcrm.com/oauth/revoke
  source: openapi/relmcrm-com-openapi.yml
  token_endpoint_auth_methods_supported:
  - none
  - client_secret_post
  - client_secret_basic
  version: OAuth 2.1 (authorization code + PKCE S256 + refresh-token rotation)
scope_count: 1
scope_names:
- crm
scopes:
- description: Read and write the connected Relm workspace
  flows:
  - authorizationCode
  scope: crm
slug: relmcrm-com-scopes
source_filename: relmcrm-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/relmcrm-com-openapi.yml (components.securitySchemes.oauth2) + well-known/relmcrm-com-oauth-authorization-server.json (RFC 8414, fetched live from https://api.relmcrm.com/.well-known/oauth-authorization-server) + well-known/relmcrm-com-oauth-protected-resource.json (RFC 9728) + https://relmcrm.com/docs (OAuth 2.1 section)\ndocs: https://relmcrm.com/docs\nsummary: >-\n  One scope. Relm's OAuth 2.1 server issues a single coarse scope, crm, that grants read and write over the\n  connected workspace; there is no read-only scope, no per-object scope and no admin/billing split. The scope\n  set is the same in the OpenAPI, the RFC 8414 metadata (scopes_supported), the RFC 9728 protected-resource\n  document (scopes_supported), the agent card, the MCP descriptor and every MCP tool's securitySchemes[]\n  (oauth2, scopes [crm]). OAuth acts on live data only; test mode is API-key only.\nschemes:\n- name: oauth2\n  source: openapi/relmcrm-com-openapi.yml\n\
  \  version: OAuth 2.1 (authorization code + PKCE S256 + refresh-token rotation)\n  issuer: https://api.relmcrm.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.relmcrm.com/oauth/authorize\n    tokenUrl: https://api.relmcrm.com/oauth/token\n    refreshUrl: https://api.relmcrm.com/oauth/token\n  registration_endpoint: https://api.relmcrm.com/oauth/register\n  revocation_endpoint: https://api.relmcrm.com/oauth/revoke\n  grant_types_supported: [authorization_code, refresh_token]\n  response_types_supported: [code]\n  code_challenge_methods_supported: [S256]\n  token_endpoint_auth_methods_supported: [none, client_secret_post, client_secret_basic]\n  dynamic_client_registration: RFC 7591 — clients register themselves; the dashboard lists connected apps and disconnecting one revokes all of its access immediately (changelog v0.17.0)\n  discovery:\n    authorization_server: well-known/relmcrm-com-oauth-authorization-server.json\n    protected_resource: well-known/relmcrm-com-oauth-protected-resource.json\n\
  \    resource: https://api.relmcrm.com/mcp\n  live_only: true\n  description: 'OAuth 2.1 with PKCE (S256) and dynamic client registration (RFC 7591). Live mode only; test mode is API-key only. Discovery: /.well-known/oauth-authorization-server.'\nscopes:\n- scope: crm\n  description: Read and write the connected Relm workspace\n  access: read-write over contacts, companies, deals, activities, pipelines, registry, automations, sequences, templates, connections, webhooks, usage and settings\n  flows:\n  - authorizationCode\n  required_by: >-\n    every MCP tool (securitySchemes oauth2 / scopes [crm] on all 41 tools in mcp/relmcrm-com-mcp-tools-list.json);\n    the OpenAPI root security requirement; the agent card security[]\n  sources:\n  - openapi/relmcrm-com-openapi.yml\n  - well-known/relmcrm-com-oauth-authorization-server.json\n  - well-known/relmcrm-com-oauth-protected-resource.json\ngranularity_note: >-\n  Coarse by design for a workspace-scoped product; least-privilege for an agent\
  \ is achieved by the MCP tool\n  annotations (readOnlyHint / destructiveHint) that let a client gate confirmation, not by scope. An operator\n  who needs a read-only credential has no scope to ask for.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/relmcrm-com/refs/heads/main/scopes/relmcrm-com-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- CRM
- Sales
- Contacts
- Deals
- Sales Pipeline
- Automation
- Webhook
- MCP
- A2A
- AI Agents
- agent-native
- United Arab Emirates
token_urls:
- https://api.relmcrm.com/oauth/token
---
