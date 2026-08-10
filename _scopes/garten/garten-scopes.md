---
authorization_urls:
- https://tv.garten.co/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Garten Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Garten publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Garten API on a user''s behalf.


  Tokens are issued from https://tv.garten.co/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Garten
provider_slug: garten
schemes:
- flows:
  - authorizationUrl: https://tv.garten.co/oauth/authorize
    flow: authorizationCode
    pkce: S256
    refreshUrl: https://tv.garten.co/oauth/token
    tokenUrl: https://tv.garten.co/oauth/token
  issuer: https://tv.garten.co
  name: garten TV OAuth 2.1
  source: well-known/garten-tv-oauth-authorization-server.json
scope_count: 7
scope_names:
- content_analytics.read
- finance_analytics.read
- crm.read
- cms.read
- products.read
- cms.write
- crm.write
scopes:
- description: Read content analytics for the garten TV catalog (scope name as published; garten publishes no description text).
  flows:
  - authorizationCode
  scope: content_analytics.read
- description: Read finance analytics for the garten TV property (scope name as published).
  flows:
  - authorizationCode
  scope: finance_analytics.read
- description: Read CRM / customer records (scope name as published).
  flows:
  - authorizationCode
  scope: crm.read
- description: Read CMS content objects (scope name as published).
  flows:
  - authorizationCode
  scope: cms.read
- description: Read products / catalog offerings (scope name as published).
  flows:
  - authorizationCode
  scope: products.read
- description: Create or modify CMS content objects (scope name as published).
  flows:
  - authorizationCode
  scope: cms.write
- description: Create or modify CRM / customer records (scope name as published).
  flows:
  - authorizationCode
  scope: crm.write
slug: garten-scopes
source_filename: garten-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: https://tv.garten.co/.well-known/oauth-authorization-server\nalso_declared_in: https://tv.garten.co/.well-known/oauth-protected-resource\ndocs: null\ndocs_note: garten publishes no scope reference page; the scope list below is exactly\n  what the two live discovery documents advertise, with nothing added.\nschemes:\n- name: garten TV OAuth 2.1\n  source: well-known/garten-tv-oauth-authorization-server.json\n  issuer: https://tv.garten.co\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://tv.garten.co/oauth/authorize\n    tokenUrl: https://tv.garten.co/oauth/token\n    refreshUrl: https://tv.garten.co/oauth/token\n    pkce: S256\nscopes:\n- scope: content_analytics.read\n  description: Read content analytics for the garten TV catalog (scope name as published;\n    garten publishes no description text).\n  flows: [authorizationCode]\n  access: read\n  sources: [well-known/garten-tv-oauth-authorization-server.json]\n\
  - scope: finance_analytics.read\n  description: Read finance analytics for the garten TV property (scope name as published).\n  flows: [authorizationCode]\n  access: read\n  sources: [well-known/garten-tv-oauth-authorization-server.json]\n- scope: crm.read\n  description: Read CRM / customer records (scope name as published).\n  flows: [authorizationCode]\n  access: read\n  sources: [well-known/garten-tv-oauth-authorization-server.json]\n- scope: cms.read\n  description: Read CMS content objects (scope name as published).\n  flows: [authorizationCode]\n  access: read\n  sources: [well-known/garten-tv-oauth-authorization-server.json]\n- scope: products.read\n  description: Read products / catalog offerings (scope name as published).\n  flows: [authorizationCode]\n  access: read\n  sources: [well-known/garten-tv-oauth-authorization-server.json]\n- scope: cms.write\n  description: Create or modify CMS content objects (scope name as published).\n  flows: [authorizationCode]\n  access: write\n\
  \  sources: [well-known/garten-tv-oauth-authorization-server.json]\n- scope: crm.write\n  description: Create or modify CRM / customer records (scope name as published).\n  flows: [authorizationCode]\n  access: write\n  sources: [well-known/garten-tv-oauth-authorization-server.json]\nsummary:\n  scope_count: 7\n  read_scopes: 5\n  write_scopes: 2\n  domains: [content_analytics, finance_analytics, crm, cms, products]\n  protected_resource: https://tv.garten.co/mcp\nx-evidence:\n  fetched: '2026-08-04'\n  url: https://tv.garten.co/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/garten/refs/heads/main/scopes/garten-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Company
- Food Service
- Corporate Wellness
- Workplace
- Catering
- Employee Benefits
- Micro Market
- Facilities Management
- Hospitality
- Streaming Video
- MCP
token_urls:
- https://tv.garten.co/oauth/token
---
