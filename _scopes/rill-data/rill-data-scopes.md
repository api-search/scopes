---
api_specs:
- filename: rill-data-admin-openapi.yaml
  format: yaml
  label: Rill Admin API
  slug: rill-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rill-data/refs/heads/main/openapi/rill-data-admin-openapi.yaml
authorization_urls:
- https://admin.rilldata.com/auth/oauth/authorize
description: ''
docs: https://docs.rilldata.com/guide/ai/mcp
flows:
- authorizationCode
- deviceCode
kind: oauth-scopes
layout: scope
method: searched
name: Rill Data Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Rill Data publishes 1 OAuth 2.0 scope via the authorizationCode and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Rill Data API on a user''s behalf.


  Tokens are issued from https://admin.rilldata.com/auth/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Rill Data
provider_slug: rill-data
schemes:
- flows:
  - authorizationUrl: https://admin.rilldata.com/auth/oauth/authorize
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://admin.rilldata.com/auth/oauth/register
    tokenUrl: https://admin.rilldata.com/auth/oauth/token
  - flow: deviceCode
    tokenUrl: https://admin.rilldata.com/auth/oauth/token
  name: OAuth2
  source: well-known/rill-data-oauth-authorization-server.json
scope_count: 1
scope_names:
- offline_access
scopes:
- description: Issue a refresh token so the client (e.g. an MCP connector) can maintain long-lived access without re-authorizing. This is the only scope Rill's OAuth authorization server advertises as supported.
  flows:
  - authorizationCode
  - deviceCode
  scope: offline_access
slug: rill-data-scopes
source_filename: rill-data-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: well-known/rill-data-oauth-authorization-server.json\ndocs: https://docs.rilldata.com/guide/ai/mcp\nschemes:\n  - name: OAuth2\n    source: well-known/rill-data-oauth-authorization-server.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://admin.rilldata.com/auth/oauth/authorize\n        tokenUrl: https://admin.rilldata.com/auth/oauth/token\n        registrationUrl: https://admin.rilldata.com/auth/oauth/register\n        pkce: S256\n      - flow: deviceCode\n        tokenUrl: https://admin.rilldata.com/auth/oauth/token\nscopes:\n  - scope: offline_access\n    description: >-\n      Issue a refresh token so the client (e.g. an MCP connector) can maintain\n      long-lived access without re-authorizing. This is the only scope Rill's\n      OAuth authorization server advertises as supported.\n    flows: [authorizationCode, deviceCode]\n    sources: [well-known/rill-data-oauth-authorization-server.json]\n\
  notes: >-\n  Rill's OAuth authorization server advertises a single scope (offline_access);\n  effective authorization is governed by the user's org/project roles rather\n  than fine-grained OAuth scopes. Once authorized, data-plane access is scoped\n  to the specific org/project/branch encoded in the MCP/runtime URL.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rill-data/refs/heads/main/scopes/rill-data-scopes.yml
summary_line: 1 scope · authorizationCode/deviceCode
tags:
- Company
- Analytics
- Business Intelligence
- Dashboards
- Metrics
- Data
- OLAP
- Open Source
- Developer Tools
token_urls:
- https://admin.rilldata.com/auth/oauth/token
---
