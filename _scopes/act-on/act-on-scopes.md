---
api_specs:
- filename: act-on-rest-api-openapi.yml
  format: yaml
  label: Act-On REST API
  slug: act-on-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/act-on/refs/heads/main/openapi/act-on-rest-api-openapi.yml
- filename: act-on-custom-objects-service-openapi.yml
  format: yaml
  label: Act-On Custom Objects Service
  slug: act-on-custom-objects-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/act-on/refs/heads/main/openapi/act-on-custom-objects-service-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: derived
name: Act On Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Act-On uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Act-On
provider_slug: act-on
schemes:
- flows: []
  name: sec0
  note: The published securityScheme is literally `{"type":"oauth2","flows":{}}` — no authorizationUrl, no tokenUrl, no scopes object. The three grant types Act-On documents (password, refresh_token, authorization_code) are described in prose on the developer portal, not in the security scheme.
  source: openapi/act-on-oauth-openapi.yml
  type: oauth2
scope_count: 0
scope_names: []
scopes: []
slug: act-on-scopes
source_filename: act-on-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/act-on-oauth-openapi.yml + https://developer.act-on.com/reference/api-overview\n  + https://developer.act-on.com/reference/userspecs-overview\napi: Act-On REST API\nsummary: >-\n  Act-On runs OAuth 2.0 but publishes NO SCOPES. This file records a measured\n  absence, not a scope catalog, and no OAuthScopes pointer is emitted in apis.yml on\n  the strength of it.\nscope_count: 0\nscopes: []\nschemes:\n- name: sec0\n  type: oauth2\n  source: openapi/act-on-oauth-openapi.yml\n  flows: []\n  note: >-\n    The published securityScheme is literally `{\"type\":\"oauth2\",\"flows\":{}}` — no\n    authorizationUrl, no tokenUrl, no scopes object. The three grant types Act-On\n    documents (password, refresh_token, authorization_code) are described in prose on\n    the developer portal, not in the security scheme.\nsearched:\n- url: https://developer.act-on.com/reference/api-overview\n  status: 200\n  result: no scopes, no permissions\
  \ reference, no consent screen documentation\n- url: https://developer.act-on.com/llms.txt\n  status: 200\n  result: 161-page documentation index contains no scopes or permissions page\nauthorization_instead:\n  model: account user privileges\n  where: set on the Act-On user, in the Act-On UI or at user-creation time\n  documented_at: https://developer.act-on.com/reference/userspecs-overview\n  privileges:\n  - marketingPrivileges:launchPrivilege\n  - marketingPrivileges:admin\n  - contactLists:create\n  - contactLists:delete\n  - contactLists:download\n  - content:create\n  - content:delete\n  - programs:create\n  - programs:delete\n  - accountWideEmail:view\n  - accountWideEmail:manage\n  note: >-\n    These are USER privileges, not OAuth scopes. They bound what a token obtained via\n    the password grant for that user can do, but they are never requested, granted,\n    returned or introspected through the API — a client cannot ask for least\n    privilege, and cannot discover what\
  \ privilege it actually holds. They are listed\n    here as the real authorization surface, deliberately NOT as scopes.\nconsequence: >-\n  There is no downscoping. Any integration authenticating as an administrator holds\n  administrator power over the whole account, including irreversible sends and\n  deletes. See mcp/act-on-mcp.yml agent_safety_notes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/act-on/refs/heads/main/scopes/act-on-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Marketing
- Marketing Automation
- Email Marketing
- Email
- Marketing Technology
- Lead Generation
- Campaign Management
- Customer Data
- Webhooks
- API
token_urls: []
---
