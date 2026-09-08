---
api_specs:
- filename: dialnexa-agents-api-openapi.yml
  format: yaml
  label: DialNexa Agents API
  slug: dialnexa-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/openapi/dialnexa-agents-api-openapi.yml
- filename: dialnexa-batch-calls-api-openapi.yml
  format: yaml
  label: DialNexa Batch Calls API
  slug: dialnexa-batch-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/openapi/dialnexa-batch-calls-api-openapi.yml
- filename: dialnexa-calls-api-openapi.yml
  format: yaml
  label: DialNexa Calls API
  slug: dialnexa-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/openapi/dialnexa-calls-api-openapi.yml
- filename: dialnexa-knowledge-base-api-openapi.yml
  format: yaml
  label: DialNexa Knowledge Base API
  slug: dialnexa-knowledge-base-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/openapi/dialnexa-knowledge-base-api-openapi.yml
- filename: dialnexa-languages-api-openapi.yml
  format: yaml
  label: DialNexa Languages API
  slug: dialnexa-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/openapi/dialnexa-languages-api-openapi.yml
- filename: dialnexa-llms-api-openapi.yml
  format: yaml
  label: DialNexa LL Ms API
  slug: dialnexa-llms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/openapi/dialnexa-llms-api-openapi.yml
- filename: dialnexa-organization-folders-api-openapi.yml
  format: yaml
  label: DialNexa Organization Folders API
  slug: dialnexa-organization-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/openapi/dialnexa-organization-folders-api-openapi.yml
- filename: dialnexa-phone-numbers-api-openapi.yml
  format: yaml
  label: DialNexa Phone Numbers API
  slug: dialnexa-phone-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/openapi/dialnexa-phone-numbers-api-openapi.yml
- filename: dialnexa-transcribers-api-openapi.yml
  format: yaml
  label: DialNexa Transcribers API
  slug: dialnexa-transcribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/openapi/dialnexa-transcribers-api-openapi.yml
- filename: dialnexa-voices-api-openapi.yml
  format: yaml
  label: DialNexa Voices API
  slug: dialnexa-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/openapi/dialnexa-voices-api-openapi.yml
- filename: dialnexa-webhooks-api-openapi.yml
  format: yaml
  label: DialNexa Webhooks API
  slug: dialnexa-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/openapi/dialnexa-webhooks-api-openapi.yml
- filename: dialnexa-workflow-leads-api-openapi.yml
  format: yaml
  label: DialNexa Workflow Leads API
  slug: dialnexa-workflow-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/openapi/dialnexa-workflow-leads-api-openapi.yml
- filename: dialnexa-workflows-api-openapi.yml
  format: yaml
  label: DialNexa Workflows API
  slug: dialnexa-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/openapi/dialnexa-workflows-api-openapi.yml
authorization_urls: []
description: OAuth scopes apply to the MCP surface only. The REST /v1 API uses dashboard-provisioned API keys (bearer) and declares no oauth2 securityScheme in its OpenAPI; the dialnexa.com oauth-authorization-server metadata says plainly that public OAuth token issuance is not available for the REST API. The api.dialnexa.com authorization server (OAuth 2.1, authorization-code + PKCE S256, PAR, DPoP) issues tokens for the MCP endpoint https://api.dialnexa.com/v1/mcp.
docs: https://dialnexa.com/docs/mcp-tools/overview
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Dialnexa Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'DialNexa uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: DialNexa
provider_slug: dialnexa
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: dialnexa-scopes
source_filename: dialnexa-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: searched\nsource: https://api.dialnexa.com/.well-known/oauth-authorization-server + https://dialnexa.com/docs/mcp-tools/overview.md\ndocs: https://dialnexa.com/docs/mcp-tools/overview\ndescription: >-\n  OAuth scopes apply to the MCP surface only. The REST /v1 API uses dashboard-provisioned API keys\n  (bearer) and declares no oauth2 securityScheme in its OpenAPI; the dialnexa.com\n  oauth-authorization-server metadata says plainly that public OAuth token issuance is not\n  available for the REST API. The api.dialnexa.com authorization server (OAuth 2.1,\n  authorization-code + PKCE S256, PAR, DPoP) issues tokens for the MCP endpoint\n  https://api.dialnexa.com/v1/mcp.\noauth_surface: https://api.dialnexa.com/v1/mcp\nauthorization_server: https://api.dialnexa.com\nscopes:\n- name: mcp:read\n  description: Read DialNexa workspace data through MCP tools.\n- name: mcp:write\n  description: Run state-changing MCP tools after any tool-specific confirmation\
  \ requirements are satisfied.\n- name: offline_access\n  description: Let a compatible client refresh access without re-authenticating every request.\n- name: openid\n  description: OpenID Connect scope advertised by the authorization server metadata (id_token issuance).\nscope_count: 4\nnotes:\n- OAuth grants are tied to the approving user AND the workspace chosen on the consent screen; tool arguments cannot switch workspaces.\n- API-key Bearer auth is the alternative for MCP clients that support custom headers; the key resolves the workspace.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/scopes/dialnexa-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Voice AI
- AI Agents
- Telephony
- Lead Qualification
- Multilingual
token_urls: []
---
