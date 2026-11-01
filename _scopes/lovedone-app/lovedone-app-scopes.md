---
api_specs:
- filename: lovedone-app-content-api-openapi.yml
  format: yaml
  label: lovedone-app Content API
  slug: lovedone-app-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lovedone-app/openapi/lovedone-app-content-api-openapi.yml
- filename: lovedone-app-discovery-api-openapi.yml
  format: yaml
  label: lovedone-app Discovery API
  slug: lovedone-app-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lovedone-app/openapi/lovedone-app-discovery-api-openapi.yml
- filename: lovedone-app-mcp-api-openapi.yml
  format: yaml
  label: lovedone-app MCP API
  slug: lovedone-app-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lovedone-app/openapi/lovedone-app-mcp-api-openapi.yml
authorization_urls:
- https://inbox.lovedone.app/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Lovedone App Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'lovedone-app publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the lovedone-app API on a user''s behalf.


  Tokens are issued from https://inbox.lovedone.app/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: lovedone-app
provider_slug: lovedone-app
schemes:
- description: 'OAuth 2.1 authorization-code + PKCE for MCP clients. Issuer https://inbox.lovedone.app. Metadata: https://inbox.lovedone.app/.well-known/oauth-authorization-server and https://inbox.lovedone.app/.well-known/oauth-protected-resource. Public scopes match packages/auth MCP_SCOPES (profile:read, care_circle:read, care_circle:write). audit:read exists in the schema but is not offered by default (public: false).'
  flows:
  - authorizationUrl: https://inbox.lovedone.app/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://inbox.lovedone.app/oauth/token
  name: LovedOneOAuth
  source: openapi/lovedone-app-openapi.json
scope_count: 4
scope_names:
- audit:read
- care_circle:read
- care_circle:write
- profile:read
scopes:
- description: Read the caller's agent activity log (internal — not advertised on the authorization server by default).
  flows:
  - authorizationCode
  scope: audit:read
- description: List loved ones and read recent care events. Required by list_loved_ones and list_care_events.
  flows:
  - authorizationCode
  scope: care_circle:read
- description: Invite family, add providers, send replies, and add notes or visits on your behalf. Required by invite_family_member, create_provider_code, reply_to_inbox_message, add_visit_note, and schedule_visit.
  flows:
  - authorizationCode
  scope: care_circle:write
- description: See the caller's name, email, and LovedOne workspace membership. Required by get_user_profile.
  flows:
  - authorizationCode
  scope: profile:read
slug: lovedone-app-scopes
source_filename: lovedone-app-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/lovedone-app-openapi.json\nschemes:\n- name: LovedOneOAuth\n  source: openapi/lovedone-app-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://inbox.lovedone.app/oauth/authorize\n    tokenUrl: https://inbox.lovedone.app/oauth/token\n  description: 'OAuth 2.1 authorization-code + PKCE for MCP clients. Issuer https://inbox.lovedone.app.\n    Metadata: https://inbox.lovedone.app/.well-known/oauth-authorization-server and https://inbox.lovedone.app/.well-known/oauth-protected-resource.\n    Public scopes match packages/auth MCP_SCOPES (profile:read, care_circle:read, care_circle:write).\n    audit:read exists in the schema but is not offered by default (public: false).'\nscopes:\n- scope: audit:read\n  description: Read the caller's agent activity log (internal — not advertised on the authorization\n    server by default).\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lovedone-app-openapi.json\n\
  - scope: care_circle:read\n  description: List loved ones and read recent care events. Required by list_loved_ones and\n    list_care_events.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lovedone-app-openapi.json\n- scope: care_circle:write\n  description: Invite family, add providers, send replies, and add notes or visits on your behalf.\n    Required by invite_family_member, create_provider_code, reply_to_inbox_message, add_visit_note,\n    and schedule_visit.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lovedone-app-openapi.json\n- scope: profile:read\n  description: See the caller's name, email, and LovedOne workspace membership. Required by\n    get_user_profile.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lovedone-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/lovedone-app/scopes/lovedone-app-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Family Care
- Inbox
- Healthcare
- Communication
- Privacy
token_bound: false
token_urls:
- https://inbox.lovedone.app/oauth/token
---
