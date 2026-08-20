---
api_specs:
- filename: salsify-digital-assets-api-openapi.yml
  format: yaml
  label: Salsify Digital Assets API
  slug: salsify-digital-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsify/refs/heads/main/openapi/salsify-digital-assets-api-openapi.yml
- filename: salsify-export-runs-api-openapi.yml
  format: yaml
  label: Salsify Export Runs API
  slug: salsify-export-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsify/refs/heads/main/openapi/salsify-export-runs-api-openapi.yml
- filename: salsify-imports-api-openapi.yml
  format: yaml
  label: Salsify Imports API
  slug: salsify-imports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsify/refs/heads/main/openapi/salsify-imports-api-openapi.yml
- filename: salsify-lists-api-openapi.yml
  format: yaml
  label: Salsify Lists API
  slug: salsify-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsify/refs/heads/main/openapi/salsify-lists-api-openapi.yml
- filename: salsify-org-id-api-openapi.yml
  format: yaml
  label: Salsify <org ID> API
  slug: salsify-org-id-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsify/refs/heads/main/openapi/salsify-org-id-api-openapi.yml
- filename: salsify-products-api-openapi.yml
  format: yaml
  label: Salsify Products API
  slug: salsify-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsify/refs/heads/main/openapi/salsify-products-api-openapi.yml
- filename: salsify-properties-api-openapi.yml
  format: yaml
  label: Salsify Properties API
  slug: salsify-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsify/refs/heads/main/openapi/salsify-properties-api-openapi.yml
- filename: salsify-record-types-api-openapi.yml
  format: yaml
  label: Salsify Record Types API
  slug: salsify-record-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsify/refs/heads/main/openapi/salsify-record-types-api-openapi.yml
- filename: salsify-records-api-openapi.yml
  format: yaml
  label: Salsify Records API
  slug: salsify-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsify/refs/heads/main/openapi/salsify-records-api-openapi.yml
authorization_urls:
- https://app.salsify.com/oauth/authorize
description: ''
docs: https://developers.salsify.com/docs/oauth2
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Salsify Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Salsify publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Salsify API on a user''s behalf.


  Tokens are issued from https://app.salsify.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Salsify
provider_slug: salsify
schemes:
- flows:
  - authorizationUrl: https://app.salsify.com/oauth/authorize
    code_challenge_methods_supported:
    - S256
    flow: authorizationCode
    refreshUrl: https://app.salsify.com/oauth/token
    tokenUrl: https://app.salsify.com/oauth/token
  issuer: https://app.salsify.com
  name: Salsify OAuth 2.0
  source: https://developers.salsify.com/docs/oauth2
scope_count: 2
scope_names:
- all
- claudeai
scopes:
- description: The only scope Salsify's OAuth 2.0 implementation currently issues for third-party integrations. It grants the full set of permissions the authorizing user holds - there is no finer-grained read/write or per-resource scope surface.
  flows:
  - authorizationCode
  scope: all
- description: Scope advertised in scopes_supported by the RFC 8414 authorization-server metadata at https://app.salsify.com/.well-known/oauth-authorization-server. It is the scope used by the first-party Salsify MCP server at https://app.salsify.com/mcp.
  flows:
  - authorizationCode
  scope: claudeai
slug: salsify-scopes
source_filename: salsify-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://developers.salsify.com/docs/oauth2\ndocs: https://developers.salsify.com/docs/oauth2\nmetadata: well-known/salsify-oauth-authorization-server.json\nschemes:\n- name: Salsify OAuth 2.0\n  source: https://developers.salsify.com/docs/oauth2\n  issuer: https://app.salsify.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.salsify.com/oauth/authorize\n    tokenUrl: https://app.salsify.com/oauth/token\n    refreshUrl: https://app.salsify.com/oauth/token\n    code_challenge_methods_supported:\n    - S256\nscopes:\n- scope: all\n  description: >-\n    The only scope Salsify's OAuth 2.0 implementation currently issues for third-party\n    integrations. It grants the full set of permissions the authorizing user holds -\n    there is no finer-grained read/write or per-resource scope surface.\n  flows:\n  - authorizationCode\n  sources:\n  - https://developers.salsify.com/docs/oauth2\n- scope: claudeai\n\
  \  description: >-\n    Scope advertised in scopes_supported by the RFC 8414 authorization-server metadata\n    at https://app.salsify.com/.well-known/oauth-authorization-server. It is the scope\n    used by the first-party Salsify MCP server at https://app.salsify.com/mcp.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/salsify-oauth-authorization-server.json\nnotes:\n- >-\n  Scope granularity is coarse. Salsify's own documentation states \"We only support the\n  all scope at the moment which includes the full set of permissions that the user has.\"\n  Least privilege is therefore enforced by the permissions of the user the integration\n  authenticates as, not by OAuth scopes.\n- >-\n  None of the three published OpenAPI documents declare an oauth2 securityScheme, so this\n  artifact could not be derived mechanically from the specs; it was read from the docs\n  and the live authorization-server metadata.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salsify/refs/heads/main/scopes/salsify-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Product Experience Management
- Product Information Management
- Digital Asset Management
- Commerce
- Retail
- Syndication
- Data Management
- Software-as-a-Service
token_urls:
- https://app.salsify.com/oauth/token
---
