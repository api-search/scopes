---
api_specs:
- filename: lucent-openapi-original.json
  format: json
  label: Lucent API
  slug: lucent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucent/refs/heads/main/openapi/lucent-openapi-original.json
authorization_urls: []
description: ''
docs: https://docs.lucenthq.com/api-reference/authentication
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Lucent Scopes
name_suffix: OAuth Scopes
note: Scopes govern the Data API bearer tokens and the OAuth 2.1 authorization server that fronts the MCP endpoint. The OpenAPI declares an http bearer scheme (lucentBearer); the scope model is documented in the auth/OAuth docs and advertised in RFC 8414/9728 metadata.
overview: 'Lucent publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Lucent API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Lucent
provider_slug: lucent
schemes:
- authorizationUrl: https://app.lucenthq.com/oauth/authorize
  dynamic_client_registration: true
  grant_types:
  - authorization_code
  - refresh_token
  name: OAuth2.1
  pkce: S256
  registrationUrl: https://app.lucenthq.com/api/oauth/register
  revocationUrl: https://app.lucenthq.com/api/oauth/revoke
  tokenUrl: https://app.lucenthq.com/api/oauth/token
  type: oauth2
scope_count: 2
scope_names:
- read:lucent
- write:issues
scopes:
- description: Read access to all Data API read endpoints and the four read MCP tools (list_issues, get_issue, list_signals, list_insights). Included with every token.
  flows: []
  scope: read:lucent
- description: Permits updating issue status via PATCH /api/v1/issues/{issueId} and the update_issue MCP tool. Must be explicitly requested in the OAuth flow or enabled at API-key creation ("Allow issue status updates").
  flows: []
  scope: write:issues
slug: lucent-scopes
source_filename: lucent-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.lucenthq.com/mcp/oauth\ndocs: https://docs.lucenthq.com/api-reference/authentication\nwell_known:\n- well-known/lucent-oauth-authorization-server.json\n- well-known/lucent-oauth-protected-resource.json\nnote: >-\n  Scopes govern the Data API bearer tokens and the OAuth 2.1 authorization server that\n  fronts the MCP endpoint. The OpenAPI declares an http bearer scheme (lucentBearer); the\n  scope model is documented in the auth/OAuth docs and advertised in RFC 8414/9728 metadata.\nschemes:\n- name: OAuth2.1\n  type: oauth2\n  authorizationUrl: https://app.lucenthq.com/oauth/authorize\n  tokenUrl: https://app.lucenthq.com/api/oauth/token\n  registrationUrl: https://app.lucenthq.com/api/oauth/register\n  revocationUrl: https://app.lucenthq.com/api/oauth/revoke\n  grant_types: [authorization_code, refresh_token]\n  pkce: S256\n  dynamic_client_registration: true\nscopes:\n- scope: read:lucent\n  description: Read\
  \ access to all Data API read endpoints and the four read MCP tools (list_issues, get_issue, list_signals, list_insights). Included with every token.\n  grants: [listIssues, getIssue, listSignals, listInsights]\n- scope: write:issues\n  description: Permits updating issue status via PATCH /api/v1/issues/{issueId} and the update_issue MCP tool. Must be explicitly requested in the OAuth flow or enabled at API-key creation (\"Allow issue status updates\").\n  grants: [updateIssueStatus]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lucent/refs/heads/main/scopes/lucent-scopes.yml
summary_line: 2 scopes
tags:
- Company
- Session Replay
- Product Analytics
- Bug Detection
- Observability
- Artificial Intelligence
- Developer Tools
- MCP
- Webhooks
token_urls: []
---
