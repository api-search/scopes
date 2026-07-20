---
authorization_urls: []
description: ''
docs: https://aps.autodesk.com/en/docs/oauth/v2/developers_guide/scopes/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Buildingconnected Scopes
name_suffix: OAuth Scopes
note: These are the OAuth 2.0 scopes advertised by the shared Autodesk Platform Services (APS) authorization server (scopes_supported) that fronts the BuildingConnected API. The list is platform-wide; the BuildingConnected /v2 endpoints consume the data:* and account:* scopes. Captured verbatim from the live authorization-server metadata — not a per-operation mapping.
overview: 'Buildingconnected publishes 16 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Buildingconnected API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Buildingconnected
provider_slug: buildingconnected
schemes:
- authorizationUrl: https://developer.api.autodesk.com/authentication/v2/authorize
  name: APS OAuth 2.0
  source: well-known/buildingconnected-oauth-authorization-server.json
  tokenUrl: https://developer.api.autodesk.com/authentication/v2/token
scope_count: 16
scope_names:
- data:read
- data:write
- data:create
- data:search
- account:read
- account:write
- user:read
- user:write
- user-profile:read
- viewables:read
- bucket:create
- bucket:read
- bucket:update
- bucket:delete
- code:all
- openid
scopes:
- description: Read access to Autodesk platform data (BuildingConnected opportunities, bid packages, users).
  flows: []
  scope: data:read
- description: Write/update access to platform data.
  flows: []
  scope: data:write
- description: Create new platform data resources.
  flows: []
  scope: data:create
- description: Search platform data.
  flows: []
  scope: data:search
- description: Read account/hub-level information.
  flows: []
  scope: account:read
- description: Write account/hub-level information.
  flows: []
  scope: account:write
- description: Read the authenticated user's profile.
  flows: []
  scope: user:read
- description: Update the authenticated user's profile.
  flows: []
  scope: user:write
- description: Read the authenticated user's profile (legacy scope).
  flows: []
  scope: user-profile:read
- description: Read access to viewable/derivative data.
  flows: []
  scope: viewables:read
- description: Create OSS storage buckets.
  flows: []
  scope: bucket:create
- description: Read OSS storage buckets.
  flows: []
  scope: bucket:read
- description: Update OSS storage buckets.
  flows: []
  scope: bucket:update
- description: Delete OSS storage buckets.
  flows: []
  scope: bucket:delete
- description: Design Automation code execution scope.
  flows: []
  scope: code:all
- description: OpenID Connect authentication scope.
  flows: []
  scope: openid
slug: buildingconnected-scopes
source_filename: buildingconnected-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developer.api.autodesk.com/.well-known/oauth-authorization-server\ndocs: https://aps.autodesk.com/en/docs/oauth/v2/developers_guide/scopes/\nnote: >-\n  These are the OAuth 2.0 scopes advertised by the shared Autodesk Platform Services (APS)\n  authorization server (scopes_supported) that fronts the BuildingConnected API. The list is\n  platform-wide; the BuildingConnected /v2 endpoints consume the data:* and account:* scopes.\n  Captured verbatim from the live authorization-server metadata — not a per-operation mapping.\nschemes:\n- name: APS OAuth 2.0\n  source: well-known/buildingconnected-oauth-authorization-server.json\n  authorizationUrl: https://developer.api.autodesk.com/authentication/v2/authorize\n  tokenUrl: https://developer.api.autodesk.com/authentication/v2/token\nscopes:\n- scope: data:read\n  description: Read access to Autodesk platform data (BuildingConnected opportunities, bid packages, users).\n\
  - scope: data:write\n  description: Write/update access to platform data.\n- scope: data:create\n  description: Create new platform data resources.\n- scope: data:search\n  description: Search platform data.\n- scope: account:read\n  description: Read account/hub-level information.\n- scope: account:write\n  description: Write account/hub-level information.\n- scope: user:read\n  description: Read the authenticated user's profile.\n- scope: user:write\n  description: Update the authenticated user's profile.\n- scope: user-profile:read\n  description: Read the authenticated user's profile (legacy scope).\n- scope: viewables:read\n  description: Read access to viewable/derivative data.\n- scope: bucket:create\n  description: Create OSS storage buckets.\n- scope: bucket:read\n  description: Read OSS storage buckets.\n- scope: bucket:update\n  description: Update OSS storage buckets.\n- scope: bucket:delete\n  description: Delete OSS storage buckets.\n- scope: code:all\n  description: Design\
  \ Automation code execution scope.\n- scope: openid\n  description: OpenID Connect authentication scope.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buildingconnected/refs/heads/main/scopes/buildingconnected-scopes.yml
summary_line: 16 scopes
tags:
- Company
- Construction
- Preconstruction
- Bid Management
- Construction Technology
- Autodesk
- Autodesk Platform Services
- Subcontractor Management
token_urls: []
---
