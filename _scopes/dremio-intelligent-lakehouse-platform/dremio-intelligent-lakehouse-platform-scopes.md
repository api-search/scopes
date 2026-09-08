---
api_specs:
- filename: dremio-intelligent-lakehouse-platform-authentication-api-openapi.yml
  format: yaml
  label: Dremio | Intelligent Lakehouse Platform Authentication API
  slug: dremio-intelligent-lakehouse-platform-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dremio-intelligent-lakehouse-platform/refs/heads/main/openapi/dremio-intelligent-lakehouse-platform-authentication-api-openapi.yml
- filename: dremio-intelligent-lakehouse-platform-catalog-api-openapi.yml
  format: yaml
  label: Dremio | Intelligent Lakehouse Platform Catalog API
  slug: dremio-intelligent-lakehouse-platform-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dremio-intelligent-lakehouse-platform/refs/heads/main/openapi/dremio-intelligent-lakehouse-platform-catalog-api-openapi.yml
- filename: dremio-intelligent-lakehouse-platform-jobs-api-openapi.yml
  format: yaml
  label: Dremio | Intelligent Lakehouse Platform Jobs API
  slug: dremio-intelligent-lakehouse-platform-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dremio-intelligent-lakehouse-platform/refs/heads/main/openapi/dremio-intelligent-lakehouse-platform-jobs-api-openapi.yml
- filename: dremio-intelligent-lakehouse-platform-pat-api-openapi.yml
  format: yaml
  label: Dremio | Intelligent Lakehouse Platform PAT API
  slug: dremio-intelligent-lakehouse-platform-pat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dremio-intelligent-lakehouse-platform/refs/heads/main/openapi/dremio-intelligent-lakehouse-platform-pat-api-openapi.yml
- filename: dremio-intelligent-lakehouse-platform-reflections-api-openapi.yml
  format: yaml
  label: Dremio | Intelligent Lakehouse Platform Reflections API
  slug: dremio-intelligent-lakehouse-platform-reflections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dremio-intelligent-lakehouse-platform/refs/heads/main/openapi/dremio-intelligent-lakehouse-platform-reflections-api-openapi.yml
- filename: dremio-intelligent-lakehouse-platform-roles-api-openapi.yml
  format: yaml
  label: Dremio | Intelligent Lakehouse Platform Roles API
  slug: dremio-intelligent-lakehouse-platform-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dremio-intelligent-lakehouse-platform/refs/heads/main/openapi/dremio-intelligent-lakehouse-platform-roles-api-openapi.yml
- filename: dremio-intelligent-lakehouse-platform-scripts-api-openapi.yml
  format: yaml
  label: Dremio | Intelligent Lakehouse Platform Scripts API
  slug: dremio-intelligent-lakehouse-platform-scripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dremio-intelligent-lakehouse-platform/refs/heads/main/openapi/dremio-intelligent-lakehouse-platform-scripts-api-openapi.yml
- filename: dremio-intelligent-lakehouse-platform-sources-api-openapi.yml
  format: yaml
  label: Dremio | Intelligent Lakehouse Platform Sources API
  slug: dremio-intelligent-lakehouse-platform-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dremio-intelligent-lakehouse-platform/refs/heads/main/openapi/dremio-intelligent-lakehouse-platform-sources-api-openapi.yml
authorization_urls:
- https://login.dremio.cloud/oauth/authorize
description: ''
docs: https://docs.dremio.com/dremio-cloud/api/oauth-token
flows:
- clientCredentials
- authorizationCode
- tokenExchange
kind: oauth-scopes
layout: scope
method: searched
name: Dremio Intelligent Lakehouse Platform Scopes
name_suffix: OAuth Scopes
note: 'No OpenAPI in this repo declares an oauth2 securityScheme, so derive-oauth-scopes.py found nothing (0 providers with oauth2). These scopes are real all the same: they are published in Dremio''s OAuth Token documentation and advertised in the live RFC 8414 discovery document the hosted MCP server serves. The scope surface is deliberately coarse.'
overview: 'Dremio | Intelligent Lakehouse Platform publishes 2 OAuth 2.0 scopes via the clientCredentials, authorizationCode, and tokenExchange flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Dremio | Intelligent Lakehouse Platform API on a user''s behalf.


  Tokens are issued from https://login.dremio.cloud/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Dremio | Intelligent Lakehouse Platform
provider_slug: dremio-intelligent-lakehouse-platform
schemes:
- flows:
  - flow: clientCredentials
    note: For service users, using client_id + client_secret. Token lifetime one hour.
    tokenUrl: https://login.dremio.cloud/oauth/token
  - authorizationUrl: https://login.dremio.cloud/oauth/authorize
    flow: authorizationCode
    note: Used by MCP clients; dynamic client registration at https://login.dremio.cloud/oauth/register.
    pkce: S256
    tokenUrl: https://login.dremio.cloud/oauth/token
  - flow: tokenExchange
    grant_type: urn:ietf:params:oauth:grant-type:token-exchange
    note: Exchange an external OIDC JWT (subject_token_type urn:ietf:params:oauth:token-type:jwt) or a personal access token for a Dremio access token.
    tokenUrl: https://login.dremio.cloud/oauth/token
  issuer: https://login.dremio.cloud
  name: DremioOAuth
  source: https://mcp.dremio.cloud/.well-known/oauth-authorization-server
  type: oauth2
scope_count: 2
scope_names:
- dremio.all
- offline_access
scopes:
- description: Full access to Dremio resources. Dremio's documentation states the scope "must be set to dremio.all" for the client-credentials flow and that a token exchange returns dremio.all.
  flows:
  - clientCredentials
  - authorizationCode
  - tokenExchange
  scope: dremio.all
- description: Issues a refresh_token alongside the access token so a client can renew without re-consent.
  flows:
  - clientCredentials
  - authorizationCode
  scope: offline_access
slug: dremio-intelligent-lakehouse-platform-scopes
source_filename: dremio-intelligent-lakehouse-platform-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: https://docs.dremio.com/dremio-cloud/api/oauth-token\ndocs: https://docs.dremio.com/dremio-cloud/api/oauth-token\ndiscovery:\n- url: https://mcp.dremio.cloud/.well-known/oauth-authorization-server\n  status: 200\n  file: well-known/dremio-intelligent-lakehouse-platform-mcp-oauth-authorization-server.json\n- url: https://login.dremio.cloud/.well-known/oauth-authorization-server\n  status: 200\n  file: well-known/dremio-intelligent-lakehouse-platform-login-oauth-authorization-server.json\nnote: >-\n  No OpenAPI in this repo declares an oauth2 securityScheme, so derive-oauth-scopes.py found\n  nothing (0 providers with oauth2). These scopes are real all the same: they are published in\n  Dremio's OAuth Token documentation and advertised in the live RFC 8414 discovery document the\n  hosted MCP server serves. The scope surface is deliberately coarse.\nschemes:\n- name: DremioOAuth\n  type: oauth2\n  issuer: https://login.dremio.cloud\n\
  \  source: https://mcp.dremio.cloud/.well-known/oauth-authorization-server\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.dremio.cloud/oauth/token\n    note: For service users, using client_id + client_secret. Token lifetime one hour.\n  - flow: authorizationCode\n    authorizationUrl: https://login.dremio.cloud/oauth/authorize\n    tokenUrl: https://login.dremio.cloud/oauth/token\n    pkce: S256\n    note: Used by MCP clients; dynamic client registration at https://login.dremio.cloud/oauth/register.\n  - flow: tokenExchange\n    tokenUrl: https://login.dremio.cloud/oauth/token\n    grant_type: urn:ietf:params:oauth:grant-type:token-exchange\n    note: >-\n      Exchange an external OIDC JWT (subject_token_type urn:ietf:params:oauth:token-type:jwt)\n      or a personal access token for a Dremio access token.\nscopes:\n- scope: dremio.all\n  description: >-\n    Full access to Dremio resources. Dremio's documentation states the scope \"must be set to\n    dremio.all\"\
  \ for the client-credentials flow and that a token exchange returns dremio.all.\n  flows: [clientCredentials, authorizationCode, tokenExchange]\n  sources:\n  - https://docs.dremio.com/dremio-cloud/api/oauth-token\n  - https://mcp.dremio.cloud/.well-known/oauth-authorization-server\n- scope: offline_access\n  description: Issues a refresh_token alongside the access token so a client can renew without re-consent.\n  flows: [clientCredentials, authorizationCode]\n  sources:\n  - https://mcp.dremio.cloud/.well-known/oauth-authorization-server\n  - https://docs.dremio.com/dremio-cloud/api/oauth-token\ngranularity:\n  level: coarse\n  assessment: >-\n    There is exactly one access scope and it is all-or-nothing. An agent cannot be issued a\n    read-only Dremio token through OAuth; least privilege has to be expressed through Dremio's\n    own RBAC (roles, grants, row-access and column-masking policies) on the user or service user\n    the token represents, not through the token's scope. For\
  \ an agent deployment that is the\n    load-bearing fact: scope the service user, because the scope string will not scope anything.\n  rbac_docs:\n  - https://docs.dremio.com/dremio-cloud/manage-govern/row-column-policies\n  - https://docs.dremio.com/dremio-cloud/admin/users\ntoken_lifetimes:\n  access_token: 3600 seconds (documented default; expires_in returned as 3599)\n  refresh_token: issued with offline_access\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dremio-intelligent-lakehouse-platform/refs/heads/main/scopes/dremio-intelligent-lakehouse-platform-scopes.yml
summary_line: 2 scopes · clientCredentials/authorizationCode/tokenExchange
tags:
- Data
- Analytics
- Lakehouse
- Apache Iceberg
- SQL
- Artificial Intelligence
token_urls:
- https://login.dremio.cloud/oauth/token
---
