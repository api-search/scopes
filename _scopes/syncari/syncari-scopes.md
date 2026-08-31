---
authorization_urls: []
description: Syncari operates two OAuth 2.0 surfaces but publishes no scope vocabulary for either. This artifact records that measured absence rather than inventing one. The MCP protected-resource metadata is served anonymously and its scopes_supported array is empty; the Embed REST API documents the client-credentials flow with no scope parameter at all, and authorises instead by the role and instance assigned to the API user.
docs:
- https://support.syncari.com/hc/en-us/articles/18707594686100-Authenticating-with-Syncari-Embed-APIs
- https://support.syncari.com/hc/en-us/articles/4417399957908-Set-Up-an-API-User
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Syncari Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Syncari uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Syncari
provider_slug: syncari
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: syncari-scopes
source_filename: syncari-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: https://mcp.syncari.com/.well-known/oauth-protected-resource\nname: Syncari OAuth scopes\ndescription: >-\n  Syncari operates two OAuth 2.0 surfaces but publishes no scope vocabulary for either. This artifact records that\n  measured absence rather than inventing one. The MCP protected-resource metadata is served anonymously and its\n  scopes_supported array is empty; the Embed REST API documents the client-credentials flow with no scope parameter\n  at all, and authorises instead by the role and instance assigned to the API user.\ndocs:\n- https://support.syncari.com/hc/en-us/articles/18707594686100-Authenticating-with-Syncari-Embed-APIs\n- https://support.syncari.com/hc/en-us/articles/4417399957908-Set-Up-an-API-User\nscope_count: 0\nscopes: []\nevidence:\n- surface: Syncari MCP Server\n  url: https://mcp.syncari.com/.well-known/oauth-protected-resource\n  http_status: 200\n  finding: '\"scopes_supported\": [] - served, empty,\
  \ on 2026-08-29.'\n- surface: Syncari MCP Server\n  url: https://mcp.syncari.com/.well-known/oauth-authorization-server\n  http_status: 200\n  finding: >-\n    RFC 8414 metadata declares grant_types authorization_code and refresh_token with PKCE S256 and dynamic client\n    registration, but carries no scopes_supported key.\n- surface: Syncari Embed API\n  url: https://support.syncari.com/hc/en-us/articles/18707594686100-Authenticating-with-Syncari-Embed-APIs\n  http_status: 200\n  finding: >-\n    The documented token request is grant_type=client_credentials with client_id and client_secret only. No scope\n    parameter is documented and no scope appears in the sample token response.\nauthorization_instead_of_scopes:\n  model: role plus instance assignment on the API user\n  roles: [Org Admin, Instance Admin]\n  custom_roles_api: https://support.syncari.com/hc/en-us/articles/50465652460820-Role\n  note: >-\n    Access is decided when the API user is created in Settings > Users, not per\
  \ token. The Role API (June 2026)\n    lets an Org Admin manage custom roles and assign them to users programmatically, which is the closest thing\n    Syncari has to a machine-readable permission surface.\nconsent_surface_exists: true\nconsent_evidence: >-\n  Syncari's Claude connector walkthrough shows a \"Syncari MCP Authorization Request screen ... listing the\n  permissions being requested\" before the user clicks Accept, so permissions are named to the human but not\n  published to machines.\ngap: >-\n  A published scopes_supported list on the MCP protected-resource metadata, and a documented scope reference page,\n  would let an agent reason about least privilege before it connects. Today it cannot.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/syncari/refs/heads/main/scopes/syncari-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Master Data Management
- Data Unification
- Data Integration
- iPaaS
- Data Quality
- Data Governance
- Embedded Integration
- MCP
- agent-native
- RevOps
- Data Synchronization
token_urls: []
---
