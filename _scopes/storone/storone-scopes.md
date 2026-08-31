---
authorization_urls: []
description: Only one of StorONE's two API surfaces uses OAuth at all. The S1 REST API on a customer's controller nodes authenticates with a session token and has no scope model whatsoever — access is governed by the S1 user account, not by scopes. The MCP server on www.storone.com publishes an RFC 8414 authorization server metadata document declaring exactly one scope.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Storone Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'StorONE uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: StorONE
provider_slug: storone
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: storone-scopes
source_filename: storone-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: https://www.storone.com/.well-known/oauth-authorization-server\nname: StorONE OAuth scopes\ndescription: >-\n  Only one of StorONE's two API surfaces uses OAuth at all. The S1 REST API on a customer's\n  controller nodes authenticates with a session token and has no scope model whatsoever — access is\n  governed by the S1 user account, not by scopes. The MCP server on www.storone.com publishes an\n  RFC 8414 authorization server metadata document declaring exactly one scope.\nsurfaces:\n  - id: mcp-oauth\n    authorization_server: https://www.storone.com\n    scope_count: 1\n    scopes:\n      - name: mcp\n        description: >-\n          The single scope advertised in scopes_supported. StorONE publishes no scope reference page\n          and no finer-grained scopes, so what this scope grants inside the MCP server cannot be\n          stated from public material — enumerating the tools it covers requires an authenticated\n\
  \          tools/list call.\n        source: https://www.storone.com/.well-known/oauth-authorization-server\n  - id: s1-rest-api\n    scope_count: 0\n    scopes: []\n    note: >-\n      No oauth2 security scheme and no scope vocabulary in the REST API reference. Authorization is\n      the S1 user's own role on the system; object-store access keys carry a separate `role`\n      parameter (see POST /applications/objects/access_keys/create) but that is an S3-style object\n      permission, not an OAuth scope.\ndocs: null\ndocs_note: StorONE publishes no scopes/permissions reference page for either surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/storone/refs/heads/main/scopes/storone-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Storage
- Enterprise Storage
- Software Defined Storage
- Data Management
- Infrastructure
- Block Storage
- File Storage
- Object Storage
- Backup
- Replication
- Snapshots
- Company
token_urls: []
---
