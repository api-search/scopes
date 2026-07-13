---
api_specs:
- filename: microsoft-visio-graph-api.yaml
  format: yaml
  label: Microsoft Graph Visio API
  slug: microsoft-graph-visio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-visio/refs/heads/main/openapi/microsoft-visio-graph-api.yaml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Microsoft Visio Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Visio publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Visio API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Visio
provider_slug: microsoft-visio
schemes:
- description: OAuth 2.0 authorization using Microsoft Identity Platform
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-visio-graph-api.yaml
scope_count: 2
scope_names:
- Files.Read
- Files.ReadWrite
scopes:
- description: Read user files
  flows:
  - authorizationCode
  scope: Files.Read
- description: Read and write user files
  flows:
  - authorizationCode
  scope: Files.ReadWrite
slug: microsoft-visio-scopes
source_filename: microsoft-visio-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-visio-graph-api.yaml\nschemes:\n- name: oauth2\n  source: openapi/microsoft-visio-graph-api.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: OAuth 2.0 authorization using Microsoft Identity Platform\nscopes:\n- scope: Files.Read\n  description: Read user files\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-visio-graph-api.yaml\n- scope: Files.ReadWrite\n  description: Read and write user files\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-visio-graph-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-visio/refs/heads/main/scopes/microsoft-visio-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Business Process
- Diagramming
- Flowcharts
- Microsoft 365
- Visualization
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
