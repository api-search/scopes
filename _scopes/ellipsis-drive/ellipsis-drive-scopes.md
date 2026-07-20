---
authorization_urls:
- https://api.ellipsis-drive.com/v3/oauth/authorize
description: ''
docs: https://docs.ellipsis-drive.com/developers/api-v3/oauth/authorization
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Ellipsis Drive Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Ellipsis Drive publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Ellipsis Drive API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Ellipsis Drive
provider_slug: ellipsis-drive
schemes:
- flows:
  - authorizationUrl: https://api.ellipsis-drive.com/v3/oauth/authorize
    flow: authorizationCode
  name: oauth2
  source: docs
scope_count: 1
scope_names:
- projects
scopes:
- description: Allows the use of all API calls except those in /settings/account. This is the default and currently the only supported OAuth scope.
  flows:
  - authorizationCode
  scope: projects
slug: ellipsis-drive-scopes
source_filename: ellipsis-drive-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.ellipsis-drive.com/developers/api-v3/oauth/authorization\ndocs: https://docs.ellipsis-drive.com/developers/api-v3/oauth/authorization\nschemes:\n- name: oauth2\n  source: docs\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.ellipsis-drive.com/v3/oauth/authorize\nscopes:\n- scope: projects\n  description: >-\n    Allows the use of all API calls except those in /settings/account. This is the default and\n    currently the only supported OAuth scope.\n  flows: [authorizationCode]\n  sources: [docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ellipsis-drive/refs/heads/main/scopes/ellipsis-drive-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Geospatial
- Spatial Data
- GIS
- Mapping
- Data Management
- Raster
- Vector
- OGC
- Cloud Storage
- Remote Sensing
token_urls: []
---
