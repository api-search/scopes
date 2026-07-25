---
api_specs:
- filename: clarifeye-agent-settings-api-openapi.yml
  format: yaml
  label: Clarifeye Agent Settings API
  slug: clarifeye-agent-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarifeye/refs/heads/main/openapi/clarifeye-agent-settings-api-openapi.yml
- filename: clarifeye-conversations-api-openapi.yml
  format: yaml
  label: Clarifeye Conversations API
  slug: clarifeye-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarifeye/refs/heads/main/openapi/clarifeye-conversations-api-openapi.yml
- filename: clarifeye-documents-api-openapi.yml
  format: yaml
  label: Clarifeye Documents API
  slug: clarifeye-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarifeye/refs/heads/main/openapi/clarifeye-documents-api-openapi.yml
- filename: clarifeye-extraction-flows-api-openapi.yml
  format: yaml
  label: Clarifeye Extraction Flows API
  slug: clarifeye-extraction-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarifeye/refs/heads/main/openapi/clarifeye-extraction-flows-api-openapi.yml
- filename: clarifeye-feedback-api-openapi.yml
  format: yaml
  label: Clarifeye Feedback API
  slug: clarifeye-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarifeye/refs/heads/main/openapi/clarifeye-feedback-api-openapi.yml
- filename: clarifeye-interviews-api-openapi.yml
  format: yaml
  label: Clarifeye Interviews API
  slug: clarifeye-interviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarifeye/refs/heads/main/openapi/clarifeye-interviews-api-openapi.yml
- filename: clarifeye-invitations-api-openapi.yml
  format: yaml
  label: Clarifeye Invitations API
  slug: clarifeye-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarifeye/refs/heads/main/openapi/clarifeye-invitations-api-openapi.yml
- filename: clarifeye-notifications-api-openapi.yml
  format: yaml
  label: Clarifeye Notifications API
  slug: clarifeye-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarifeye/refs/heads/main/openapi/clarifeye-notifications-api-openapi.yml
- filename: clarifeye-pipeline-runs-api-openapi.yml
  format: yaml
  label: Clarifeye Pipeline Runs API
  slug: clarifeye-pipeline-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarifeye/refs/heads/main/openapi/clarifeye-pipeline-runs-api-openapi.yml
- filename: clarifeye-signals-api-openapi.yml
  format: yaml
  label: Clarifeye Signals API
  slug: clarifeye-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarifeye/refs/heads/main/openapi/clarifeye-signals-api-openapi.yml
- filename: clarifeye-tables-api-openapi.yml
  format: yaml
  label: Clarifeye Tables API
  slug: clarifeye-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarifeye/refs/heads/main/openapi/clarifeye-tables-api-openapi.yml
- filename: clarifeye-tools-api-openapi.yml
  format: yaml
  label: Clarifeye Tools API
  slug: clarifeye-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarifeye/refs/heads/main/openapi/clarifeye-tools-api-openapi.yml
- filename: clarifeye-users-api-openapi.yml
  format: yaml
  label: Clarifeye Users API
  slug: clarifeye-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarifeye/refs/heads/main/openapi/clarifeye-users-api-openapi.yml
authorization_urls:
- https://eu.app.clarifeye.ai/o/authorize/
description: ''
docs: https://docs.clarifeye.ai/guides/mcp-authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Clarifeye Scopes
name_suffix: OAuth Scopes
note: Clarifeye's OAuth surface backs the hosted MCP server, not the REST API (the REST OpenAPI declares only Bearer token / Token apiKey auth). Scopes are enumerated by the OAuth authorization-server discovery document and by the MCP authentication guide. Dynamic Client Registration (RFC 7591) is supported at /o/register/; PKCE S256 required.
overview: 'Clarifeye publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Clarifeye API on a user''s behalf.


  Tokens are issued from https://eu.app.clarifeye.ai/o/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Clarifeye
provider_slug: clarifeye
schemes:
- flows:
  - authorizationUrl: https://eu.app.clarifeye.ai/o/authorize/
    flow: authorizationCode
    refreshUrl: https://eu.app.clarifeye.ai/o/token/
    registrationUrl: https://eu.app.clarifeye.ai/o/register/
    revocationUrl: https://eu.app.clarifeye.ai/o/revoke/
    tokenUrl: https://eu.app.clarifeye.ai/o/token/
  name: OAuth2
  source: https://eu.app.clarifeye.ai/.well-known/oauth-authorization-server
scope_count: 3
scope_names:
- claudeai
- openid
- offline_access
scopes:
- description: MCP access scope for Claude / AI-client connectors to the Clarifeye knowledge stores.
  flows:
  - authorizationCode
  scope: claudeai
- description: OpenID Connect scope; identifies the authenticated user (whoami).
  flows:
  - authorizationCode
  scope: openid
- description: Requests a refresh token so the client can maintain access without re-consent.
  flows:
  - authorizationCode
  scope: offline_access
slug: clarifeye-scopes
source_filename: clarifeye-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://eu.app.clarifeye.ai/.well-known/oauth-authorization-server\ndocs: https://docs.clarifeye.ai/guides/mcp-authentication\nnote: >\n  Clarifeye's OAuth surface backs the hosted MCP server, not the REST API\n  (the REST OpenAPI declares only Bearer token / Token apiKey auth). Scopes\n  are enumerated by the OAuth authorization-server discovery document and by\n  the MCP authentication guide. Dynamic Client Registration (RFC 7591) is\n  supported at /o/register/; PKCE S256 required.\nschemes:\n- name: OAuth2\n  source: https://eu.app.clarifeye.ai/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://eu.app.clarifeye.ai/o/authorize/\n    tokenUrl: https://eu.app.clarifeye.ai/o/token/\n    refreshUrl: https://eu.app.clarifeye.ai/o/token/\n    registrationUrl: https://eu.app.clarifeye.ai/o/register/\n    revocationUrl: https://eu.app.clarifeye.ai/o/revoke/\nscopes:\n- scope:\
  \ claudeai\n  description: MCP access scope for Claude / AI-client connectors to the Clarifeye knowledge stores.\n  flows: [authorizationCode]\n  sources: [https://eu.app.clarifeye.ai/.well-known/oauth-authorization-server]\n- scope: openid\n  description: OpenID Connect scope; identifies the authenticated user (whoami).\n  flows: [authorizationCode]\n  sources: [https://eu.app.clarifeye.ai/.well-known/oauth-authorization-server]\n- scope: offline_access\n  description: Requests a refresh token so the client can maintain access without re-consent.\n  flows: [authorizationCode]\n  sources: [https://eu.app.clarifeye.ai/.well-known/oauth-authorization-server]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clarifeye/refs/heads/main/scopes/clarifeye-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- Artificial Intelligence
- Knowledge Management
- Model Context Protocol
- Document Intelligence
- Agents
- Enterprise AI
- Retrieval
token_urls:
- https://eu.app.clarifeye.ai/o/token/
---
