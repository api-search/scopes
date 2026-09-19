---
api_specs:
- filename: cloudhealth-aws-accounts-api-openapi.yml
  format: yaml
  label: CloudHealth AWS Accounts API
  slug: cloudhealth-aws-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudhealth/refs/heads/main/openapi/cloudhealth-aws-accounts-api-openapi.yml
- filename: cloudhealth-perspectives-api-openapi.yml
  format: yaml
  label: CloudHealth Perspectives API
  slug: cloudhealth-perspectives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudhealth/refs/heads/main/openapi/cloudhealth-perspectives-api-openapi.yml
- filename: cloudhealth-reports-api-openapi.yml
  format: yaml
  label: CloudHealth Reports API
  slug: cloudhealth-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudhealth/refs/heads/main/openapi/cloudhealth-reports-api-openapi.yml
- filename: cloudhealth-search-api-openapi.yml
  format: yaml
  label: CloudHealth Search API
  slug: cloudhealth-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudhealth/refs/heads/main/openapi/cloudhealth-search-api-openapi.yml
- filename: cloudhealth-sso-api-openapi.yml
  format: yaml
  label: CloudHealth SSO API
  slug: cloudhealth-sso-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudhealth/refs/heads/main/openapi/cloudhealth-sso-api-openapi.yml
authorization_urls:
- https://apps.cloudhealthtech.com/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: probed
name: Cloudhealth Scopes
name_suffix: OAuth Scopes
note: No OAuth scheme is declared in the (API Evangelist-authored) OpenAPI and the docs publish no scope reference page; these scopes are read verbatim from the authorization server's RFC 8414 metadata (scopes_supported), which protects the MCP server at https://apps.cloudhealthtech.com/mcp. Descriptions are not published by the provider.
overview: 'CloudHealth publishes 4 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the CloudHealth API on a user''s behalf.


  Tokens are issued from https://apps.cloudhealthtech.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CloudHealth
provider_slug: cloudhealth
schemes:
- flows:
  - authorizationUrl: https://apps.cloudhealthtech.com/oauth2/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://apps.cloudhealthtech.com/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://apps.cloudhealthtech.com/oauth2/token
  name: CloudHealthOAuth
  protects: https://apps.cloudhealthtech.com/mcp
  source: well-known/cloudhealth-oauth-authorization-server.json
scope_count: 4
scope_names:
- mcp:datasets:read
- mcp:query:run
- mcp:flexorgs:read
- mcp:customers:read
scopes:
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: mcp:datasets:read
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: mcp:query:run
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: mcp:flexorgs:read
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: mcp:customers:read
slug: cloudhealth-scopes
source_filename: cloudhealth-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: probed\nsource: https://apps.cloudhealthtech.com/.well-known/oauth-authorization-server\nnote: No OAuth scheme is declared in the (API Evangelist-authored) OpenAPI and the docs publish no scope reference\n  page; these scopes are read verbatim from the authorization server's RFC 8414 metadata (scopes_supported), which\n  protects the MCP server at https://apps.cloudhealthtech.com/mcp. Descriptions are not published by the provider.\ndocs: null\nschemes:\n  - name: CloudHealthOAuth\n    source: well-known/cloudhealth-oauth-authorization-server.json\n    protects: https://apps.cloudhealthtech.com/mcp\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://apps.cloudhealthtech.com/oauth2/authorize\n        tokenUrl: https://apps.cloudhealthtech.com/oauth2/token\n        pkce: S256\n      - flow: clientCredentials\n        tokenUrl: https://apps.cloudhealthtech.com/oauth2/token\nscopes:\n  - scope: mcp:datasets:read\n   \
  \ description: null\n    flows: [authorizationCode, clientCredentials]\n    sources: [well-known/cloudhealth-oauth-authorization-server.json]\n  - scope: mcp:query:run\n    description: null\n    flows: [authorizationCode, clientCredentials]\n    sources: [well-known/cloudhealth-oauth-authorization-server.json]\n  - scope: mcp:flexorgs:read\n    description: null\n    flows: [authorizationCode, clientCredentials]\n    sources: [well-known/cloudhealth-oauth-authorization-server.json]\n  - scope: mcp:customers:read\n    description: null\n    flows: [authorizationCode, clientCredentials]\n    sources: [well-known/cloudhealth-oauth-authorization-server.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudhealth/refs/heads/main/scopes/cloudhealth-scopes.yml
summary_line: 4 scopes · authorizationCode/clientCredentials
tags:
- Cloud Cost
- Cloud Governance
- Cloud Management
- Cost Optimization
- FinOps
- Multi-Cloud
token_urls:
- https://apps.cloudhealthtech.com/oauth2/token
---
