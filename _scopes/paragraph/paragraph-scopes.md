---
api_specs:
- filename: paragraph-analytics-api-openapi.yml
  format: yaml
  label: Paragraph analytics API
  slug: paragraph-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/openapi/paragraph-analytics-api-openapi.yml
- filename: paragraph-auth-api-openapi.yml
  format: yaml
  label: Paragraph auth API
  slug: paragraph-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/openapi/paragraph-auth-api-openapi.yml
- filename: paragraph-coins-api-openapi.yml
  format: yaml
  label: Paragraph coins API
  slug: paragraph-coins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/openapi/paragraph-coins-api-openapi.yml
- filename: paragraph-discover-api-openapi.yml
  format: yaml
  label: Paragraph discover API
  slug: paragraph-discover-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/openapi/paragraph-discover-api-openapi.yml
- filename: paragraph-emails-api-openapi.yml
  format: yaml
  label: Paragraph emails API
  slug: paragraph-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/openapi/paragraph-emails-api-openapi.yml
- filename: paragraph-me-api-openapi.yml
  format: yaml
  label: Paragraph me API
  slug: paragraph-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/openapi/paragraph-me-api-openapi.yml
- filename: paragraph-posts-api-openapi.yml
  format: yaml
  label: Paragraph posts API
  slug: paragraph-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/openapi/paragraph-posts-api-openapi.yml
- filename: paragraph-publications-api-openapi.yml
  format: yaml
  label: Paragraph publications API
  slug: paragraph-publications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/openapi/paragraph-publications-api-openapi.yml
- filename: paragraph-subscribers-api-openapi.yml
  format: yaml
  label: Paragraph subscribers API
  slug: paragraph-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/openapi/paragraph-subscribers-api-openapi.yml
- filename: paragraph-users-api-openapi.yml
  format: yaml
  label: Paragraph users API
  slug: paragraph-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/openapi/paragraph-users-api-openapi.yml
authorization_urls: []
description: ''
docs: https://paragraph.com/auth.md
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Paragraph Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Paragraph uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Paragraph
provider_slug: paragraph
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: paragraph-scopes
source_filename: paragraph-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://paragraph.com/.well-known/oauth-authorization-server\ndocs: https://paragraph.com/auth.md\nsummary:\n  scope_count: 2\n  granularity: coarse\n  source_of_truth: RFC 8414 / RFC 9728 discovery metadata (NOT the OpenAPI)\n  note: >-\n    The published OpenAPI declares only an HTTP bearer securityScheme (`apiKey`) with no oauth2\n    flows, so `derive-oauth-scopes.py` finds nothing to derive. Paragraph nonetheless publishes\n    scopes in its OAuth discovery documents at paragraph.com, which is where these come from.\nresource:\n  identifier: https://public.api.paragraph.com/api\n  resource_name: Paragraph\n  authorization_servers:\n    - https://paragraph.com\n  bearer_methods_supported:\n    - header\nscopes:\n  - name: api.read\n    description: >-\n      Read access to the publication the user selects during approval — publications, posts,\n      subscribers, coins, analytics, and profile reads.\n    evidence: scopes_supported\
  \ in both the RFC 8414 and RFC 9728 documents at paragraph.com\n  - name: api.write\n    description: >-\n      Write access to the publication the user selects during approval — create/update/delete\n      posts, add/remove subscribers, send test and custom emails, update publication settings.\n    evidence: scopes_supported in both the RFC 8414 and RFC 9728 documents at paragraph.com\ngranularity_caveat: >-\n  Paragraph's own auth.md states plainly: \"Paragraph API keys grant read and write access to the\n  publication the user selects during approval. The keys are not currently fine-grained.\" The two\n  advertised scopes therefore describe the coarse read/write split, not per-resource permissions,\n  and the issued credential is an API key rather than a scoped OAuth access token.\nagent_auth:\n  flow: anonymous registration + user claim\n  skill: https://paragraph.com/auth.md\n  register_uri: https://public.api.paragraph.com/api/v1/api/auth/sessions\n  claim_uri: https://paragraph.com/api/auth\n\
  \  identity_types_supported: [anonymous]\n  credential_types_supported: [api_key]\n  credential_transport: 'Authorization: Bearer <api-key>'\n  backing_operations:\n    - createAuthSession   # POST /v1/api/auth/sessions\n    - getAuthSession      # GET  /v1/api/auth/sessions/{sessionId}\n    - deleteAuthSession   # DELETE /v1/api/auth/sessions/{sessionId}\nmcp_authorization_server:\n  issuer: https://mcp.paragraph.com\n  note: >-\n    The hosted MCP endpoint runs a SEPARATE authorization server from the REST API resource, and\n    it advertises NO scopes_supported — authorization is all-or-nothing for the connected account.\n  authorization_endpoint: https://mcp.paragraph.com/authorize\n  token_endpoint: https://mcp.paragraph.com/token\n  registration_endpoint: https://mcp.paragraph.com/register\n  grant_types_supported: [authorization_code, refresh_token]\n  code_challenge_methods_supported: [plain, S256]\n  scopes_supported: []\ncross_ref:\n  - authentication/paragraph-authentication.yml\n\
  \  - well-known/paragraph-well-known.yml\n  - mcp/paragraph-mcp.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/scopes/paragraph-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Publishing
- Newsletters
- Web3
- Content
- Blogging
- Creator Economy
token_urls: []
---
