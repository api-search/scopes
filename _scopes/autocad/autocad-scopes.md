---
authorization_urls:
- https://developer.api.autodesk.com/authentication/v2/authorize
description: ''
docs: https://aps.autodesk.com/en/docs/oauth/v2/developers_guide/scopes/
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Autocad Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'AutoCAD publishes 16 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the AutoCAD API on a user''s behalf.


  Tokens are issued from https://developer.api.autodesk.com/authentication/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AutoCAD
provider_slug: autocad
schemes:
- flows:
  - authorizationUrl: https://developer.api.autodesk.com/authentication/v2/authorize
    flow: authorizationCode
    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token
  - flow: clientCredentials
    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token
  name: OAuth2
  source: https://developer.api.autodesk.com/.well-known/openid-configuration
  type: oauth2
scope_count: 16
scope_names:
- user-profile:read
- user:read
- user:write
- viewables:read
- data:read
- data:write
- data:create
- data:search
- bucket:create
- bucket:read
- bucket:update
- bucket:delete
- code:all
- account:read
- account:write
- openid
scopes:
- description: Read the end user's profile data (deprecated alias; prefer user:read).
  flows:
  - authorizationCode
  scope: user-profile:read
- description: Read the end user's profile data.
  flows:
  - authorizationCode
  scope: user:read
- description: Create, update, and delete the end user's profile data.
  flows:
  - authorizationCode
  scope: user:write
- description: Read viewable (translated derivative) data for the end user.
  flows:
  - authorizationCode
  - clientCredentials
  scope: viewables:read
- description: Read documents, folders, item versions, and other data the user can access.
  flows:
  - authorizationCode
  - clientCredentials
  scope: data:read
- description: Create, update, and delete data the user can access.
  flows:
  - authorizationCode
  - clientCredentials
  scope: data:write
- description: Create new data (e.g. new folders, items) in a project or hub.
  flows:
  - authorizationCode
  - clientCredentials
  scope: data:create
- description: Search across the end user's data.
  flows:
  - authorizationCode
  - clientCredentials
  scope: data:search
- description: Create an OSS (Object Storage Service) bucket.
  flows:
  - authorizationCode
  - clientCredentials
  scope: bucket:create
- description: Read the metadata and objects of an OSS bucket.
  flows:
  - authorizationCode
  - clientCredentials
  scope: bucket:read
- description: Update an OSS bucket (e.g. change access policies).
  flows:
  - authorizationCode
  - clientCredentials
  scope: bucket:update
- description: Delete an OSS bucket.
  flows:
  - authorizationCode
  - clientCredentials
  scope: bucket:delete
- description: Author or execute code (e.g. Design Automation AppBundles and Activities) on the user's behalf.
  flows:
  - authorizationCode
  - clientCredentials
  scope: code:all
- description: Read account/team data (BIM 360 / ACC administration).
  flows:
  - authorizationCode
  - clientCredentials
  scope: account:read
- description: Create, update, and delete account/team data (BIM 360 / ACC administration).
  flows:
  - authorizationCode
  - clientCredentials
  scope: account:write
- description: OpenID Connect - obtain an id_token identifying the end user.
  flows:
  - authorizationCode
  scope: openid
slug: autocad-scopes
source_filename: autocad-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: https://developer.api.autodesk.com/.well-known/openid-configuration\ndocs: https://aps.autodesk.com/en/docs/oauth/v2/developers_guide/scopes/\nschemes:\n  - name: OAuth2\n    type: oauth2\n    source: https://developer.api.autodesk.com/.well-known/openid-configuration\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://developer.api.autodesk.com/authentication/v2/authorize\n        tokenUrl: https://developer.api.autodesk.com/authentication/v2/token\n      - flow: clientCredentials\n        tokenUrl: https://developer.api.autodesk.com/authentication/v2/token\nscopes:\n  - scope: user-profile:read\n    description: Read the end user's profile data (deprecated alias; prefer user:read).\n    flows: [authorizationCode]\n  - scope: user:read\n    description: Read the end user's profile data.\n    flows: [authorizationCode]\n  - scope: user:write\n    description: Create, update, and delete the end user's\
  \ profile data.\n    flows: [authorizationCode]\n  - scope: viewables:read\n    description: Read viewable (translated derivative) data for the end user.\n    flows: [authorizationCode, clientCredentials]\n  - scope: data:read\n    description: Read documents, folders, item versions, and other data the user can access.\n    flows: [authorizationCode, clientCredentials]\n  - scope: data:write\n    description: Create, update, and delete data the user can access.\n    flows: [authorizationCode, clientCredentials]\n  - scope: data:create\n    description: Create new data (e.g. new folders, items) in a project or hub.\n    flows: [authorizationCode, clientCredentials]\n  - scope: data:search\n    description: Search across the end user's data.\n    flows: [authorizationCode, clientCredentials]\n  - scope: bucket:create\n    description: Create an OSS (Object Storage Service) bucket.\n    flows: [authorizationCode, clientCredentials]\n  - scope: bucket:read\n    description: Read the metadata\
  \ and objects of an OSS bucket.\n    flows: [authorizationCode, clientCredentials]\n  - scope: bucket:update\n    description: Update an OSS bucket (e.g. change access policies).\n    flows: [authorizationCode, clientCredentials]\n  - scope: bucket:delete\n    description: Delete an OSS bucket.\n    flows: [authorizationCode, clientCredentials]\n  - scope: code:all\n    description: Author or execute code (e.g. Design Automation AppBundles and Activities) on the user's behalf.\n    flows: [authorizationCode, clientCredentials]\n  - scope: account:read\n    description: Read account/team data (BIM 360 / ACC administration).\n    flows: [authorizationCode, clientCredentials]\n  - scope: account:write\n    description: Create, update, and delete account/team data (BIM 360 / ACC administration).\n    flows: [authorizationCode, clientCredentials]\n  - scope: openid\n    description: OpenID Connect - obtain an id_token identifying the end user.\n    flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autocad/refs/heads/main/scopes/autocad-scopes.yml
summary_line: 16 scopes · authorizationCode/clientCredentials
tags:
- 3D Modeling
- Architecture
- CAD
- Design
- Drawing
- Engineering
token_urls:
- https://developer.api.autodesk.com/authentication/v2/token
---
