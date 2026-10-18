---
api_specs:
- filename: idrive-reseller-api-openapi.yml
  format: yaml
  label: IDrive Reseller API
  slug: idrive-reseller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idrive/refs/heads/main/openapi/idrive-reseller-api-openapi.yml
- filename: idrive-subusers-api-openapi.yml
  format: yaml
  label: IDrive Subusers API
  slug: idrive-subusers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idrive/refs/heads/main/openapi/idrive-subusers-api-openapi.yml
authorization_urls: []
description: OAuth scopes advertised by the IDrive e2 authorization server (used by the hosted IDrive e2 MCP).
docs: https://www.idrive.com/s3-storage-e2/faq-mcp
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Idrive Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'IDrive publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the IDrive API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: IDrive
provider_slug: idrive
schemes:
- authorizationUrl: https://api.idrivee2.com/oauth/authorize
  grant_types:
  - authorization_code
  - refresh_token
  name: IDrive e2 OAuth
  pkce: S256
  tokenUrl: https://api.idrivee2.com/oauth/token
  type: oauth2
scope_count: 3
scope_names:
- e2:regions:read
- e2:buckets:read
- e2:buckets:write
scopes:
- description: ''
  flows: []
  scope: e2:regions:read
- description: ''
  flows: []
  scope: e2:buckets:read
- description: ''
  flows: []
  scope: e2:buckets:write
slug: idrive-scopes
source_filename: idrive-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: https://api.idrivee2.com/oauth/.well-known/oauth-authorization-server\ndocs: https://www.idrive.com/s3-storage-e2/faq-mcp\ndescription: OAuth scopes advertised by the IDrive e2 authorization server (used by the hosted IDrive e2 MCP).\nschemes:\n- name: IDrive e2 OAuth\n  type: oauth2\n  grant_types:\n  - authorization_code\n  - refresh_token\n  authorizationUrl: https://api.idrivee2.com/oauth/authorize\n  tokenUrl: https://api.idrivee2.com/oauth/token\n  pkce: S256\nscopes:\n- name: e2:regions:read\n- name: e2:buckets:read\n- name: e2:buckets:write\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/idrive/refs/heads/main/scopes/idrive-scopes.yml
summary_line: 3 scopes
tags:
- Company
- Object Storage
- S3 Compatible
- Cloud Storage
- Backup
- Reseller
- MCP
token_bound: false
token_urls: []
---
