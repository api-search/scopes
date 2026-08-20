---
api_specs:
- filename: mixmax-contact-groups-api-openapi.yml
  format: yaml
  label: Mixmax Contact Groups API
  slug: mixmax-contact-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixmax/refs/heads/main/openapi/mixmax-contact-groups-api-openapi.yml
- filename: mixmax-contacts-api-openapi.yml
  format: yaml
  label: Mixmax Contacts API
  slug: mixmax-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixmax/refs/heads/main/openapi/mixmax-contacts-api-openapi.yml
- filename: mixmax-file-requests-api-openapi.yml
  format: yaml
  label: Mixmax File Requests API
  slug: mixmax-file-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixmax/refs/heads/main/openapi/mixmax-file-requests-api-openapi.yml
- filename: mixmax-meetings-api-openapi.yml
  format: yaml
  label: Mixmax Meetings API
  slug: mixmax-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixmax/refs/heads/main/openapi/mixmax-meetings-api-openapi.yml
- filename: mixmax-sequences-api-openapi.yml
  format: yaml
  label: Mixmax Sequences API
  slug: mixmax-sequences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixmax/refs/heads/main/openapi/mixmax-sequences-api-openapi.yml
- filename: mixmax-snippet-tags-api-openapi.yml
  format: yaml
  label: Mixmax Snippet Tags API
  slug: mixmax-snippet-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixmax/refs/heads/main/openapi/mixmax-snippet-tags-api-openapi.yml
authorization_urls: []
description: ''
docs: https://success.mixmax.com/en/articles/14298142-mixmax-mcp-server
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Mixmax Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Mixmax uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Mixmax
provider_slug: mixmax
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: mixmax-scopes
source_filename: mixmax-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://app.mixmax.com/oidc/.well-known/openid-configuration\ndocs: https://success.mixmax.com/en/articles/14298142-mixmax-mcp-server\nsurface: >-\n  These scopes govern the Mixmax MCP server (https://mcp.mixmax.com/mcp), not the classic\n  REST API. The REST API at https://api.mixmax.com/v1 has no OAuth at all — it authenticates\n  with a static X-API-Token and therefore has no scope model. See\n  authentication/mixmax-authentication.yml.\n\nauthorization_server:\n  issuer: https://app.mixmax.com/oidc\n  authorization_endpoint: https://app.mixmax.com/oidc/auth\n  token_endpoint: https://app.mixmax.com/oidc/token\n  device_authorization_endpoint: https://app.mixmax.com/oidc/device/auth\n  registration_endpoint: https://app.mixmax.com/oidc/reg\n  revocation_endpoint: https://app.mixmax.com/oidc/token/revocation\n  userinfo_endpoint: https://app.mixmax.com/oidc/me\n  jwks_uri: https://app.mixmax.com/oidc/jwks\n  grant_types_supported:\
  \ [implicit, authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:device_code']\n  code_challenge_methods_supported: [S256]\n  dynamic_client_registration: true\n  public_clients_allowed: true\n\nresource_servers:\n- resource: https://mcp.mixmax.com\n  metadata: https://mcp.mixmax.com/.well-known/oauth-protected-resource\n  scopes_required: [meetings:read]\n  bearer_methods_supported: [header]\n\nscopes:\n- name: openid\n  standard: true\n  spec: OpenID Connect Core 1.0\n  description: Request an ID token identifying the signed-in Mixmax user.\n  source: https://app.mixmax.com/oidc/.well-known/openid-configuration\n- name: offline_access\n  standard: true\n  spec: OpenID Connect Core 1.0\n  description: Issue a refresh token so the client can keep calling after the access token\n    expires — this is how an MCP client stays connected between sessions.\n  source: https://app.mixmax.com/oidc/.well-known/openid-configuration\n- name: meetings:read\n  standard: false\n  resource:\
  \ https://mcp.mixmax.com\n  access: read\n  description: >-\n    Read-only access to the authenticated user's Mixmax Meeting Intelligence data — meeting\n    summaries, transcripts, participant lists and action items. This is the only Mixmax-specific\n    scope the authorization server advertises, and it is the only scope the MCP protected-resource\n    metadata requires.\n  source: https://mcp.mixmax.com/.well-known/oauth-protected-resource\n\nobservations:\n- >-\n    The scope catalog is deliberately narrow: one product scope, read-only. Mixmax states in its\n    own docs that write actions (sequence enrollment, email sending, template management) are on\n    the roadmap, so no write scope exists yet.\n- >-\n    The MCP server also surfaces sequence data (list_sequences, get_sequence, get_sequence_insights,\n    find_contact_in_sequences), but no `sequences:read` scope is advertised. Either sequence access\n    rides on meetings:read or it is authorized outside the published scope model\
  \ — Mixmax does not\n    document which, and we did not guess.\n- >-\n    token_endpoint_auth_methods_supported on the MCP-facing metadata is [\"none\"], i.e. public\n    clients with PKCE. Combined with the open registration_endpoint this is the standard\n    MCP-client onboarding shape.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mixmax/refs/heads/main/scopes/mixmax-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Software-as-a-Service
- MCP
- Agents
- Webhook
- Authentication
- Sales Engagement
- Email
- Sales
- CRM
- Productivity
- Meetings
- Sequences
token_urls: []
---
