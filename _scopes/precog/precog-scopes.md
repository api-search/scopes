---
api_specs:
- filename: precog-admin-api-openapi.yml
  format: yaml
  label: Precog Admin API
  slug: precog-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/precog/refs/heads/main/openapi/precog-admin-api-openapi.yml
- filename: precog-data-model-api-openapi.yml
  format: yaml
  label: Precog Data Model API
  slug: precog-data-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/precog/refs/heads/main/openapi/precog-data-model-api-openapi.yml
- filename: precog-datasets-api-openapi.yml
  format: yaml
  label: Precog Datasets API
  slug: precog-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/precog/refs/heads/main/openapi/precog-datasets-api-openapi.yml
- filename: precog-destinations-api-openapi.yml
  format: yaml
  label: Precog Destinations API
  slug: precog-destinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/precog/refs/heads/main/openapi/precog-destinations-api-openapi.yml
- filename: precog-issues-api-openapi.yml
  format: yaml
  label: Precog Issues API
  slug: precog-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/precog/refs/heads/main/openapi/precog-issues-api-openapi.yml
- filename: precog-kinds-api-openapi.yml
  format: yaml
  label: Precog Kinds API
  slug: precog-kinds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/precog/refs/heads/main/openapi/precog-kinds-api-openapi.yml
- filename: precog-loads-api-openapi.yml
  format: yaml
  label: Precog Loads API
  slug: precog-loads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/precog/refs/heads/main/openapi/precog-loads-api-openapi.yml
- filename: precog-log-api-openapi.yml
  format: yaml
  label: Precog Log API
  slug: precog-log-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/precog/refs/heads/main/openapi/precog-log-api-openapi.yml
- filename: precog-pipelines-api-openapi.yml
  format: yaml
  label: Precog Pipelines API
  slug: precog-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/precog/refs/heads/main/openapi/precog-pipelines-api-openapi.yml
- filename: precog-semantic-model-api-openapi.yml
  format: yaml
  label: Precog Semantic Model API
  slug: precog-semantic-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/precog/refs/heads/main/openapi/precog-semantic-model-api-openapi.yml
- filename: precog-sources-api-openapi.yml
  format: yaml
  label: Precog Sources API
  slug: precog-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/precog/refs/heads/main/openapi/precog-sources-api-openapi.yml
- filename: precog-stripe-api-openapi.yml
  format: yaml
  label: Precog Stripe API
  slug: precog-stripe-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/precog/refs/heads/main/openapi/precog-stripe-api-openapi.yml
authorization_urls:
- https://studio.precog.cloud/api/mcp/oauth/authorize
description: ''
docs: https://studio.precog.cloud/.well-known/oauth-protected-resource
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Precog Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Precog publishes 3 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Precog API on a user''s behalf.


  Tokens are issued from https://studio.precog.cloud/api/mcp/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Precog
provider_slug: precog
schemes:
- flows:
  - authorizationUrl: https://studio.precog.cloud/api/mcp/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://studio.precog.cloud/api/mcp/oauth/token
  - flow: clientCredentials
    tokenUrl: https://studio.precog.cloud/api/mcp/oauth/token
  name: PrecogMcpOAuth
  source: https://studio.precog.cloud/.well-known/oauth-authorization-server
  type: oauth2
scope_count: 3
scope_names:
- synesis:mcp
- admin:read
- admin:write
scopes:
- description: Access the Precog (Synesis) Model Context Protocol server and its tools.
  flows:
  - authorizationCode
  - clientCredentials
  scope: synesis:mcp
- description: Read access to administrative resources over the MCP surface.
  flows:
  - authorizationCode
  - clientCredentials
  scope: admin:read
- description: Write/administrative access over the MCP surface.
  flows:
  - authorizationCode
  - clientCredentials
  scope: admin:write
slug: precog-scopes
source_filename: precog-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://studio.precog.cloud/.well-known/oauth-authorization-server\ndocs: https://studio.precog.cloud/.well-known/oauth-protected-resource\nnotes: >-\n  These OAuth 2.0 scopes are advertised by Precog's MCP authorization server\n  (RFC 8414 metadata). They govern the OAuth-secured MCP surface at\n  studio.precog.cloud. The public HTTP REST API (openapi/) itself uses opaque\n  bearer tokens (HTTP Bearer) rather than scoped OAuth, so its scheme carries no\n  scope list.\nschemes:\n- name: PrecogMcpOAuth\n  type: oauth2\n  source: https://studio.precog.cloud/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://studio.precog.cloud/api/mcp/oauth/authorize\n    tokenUrl: https://studio.precog.cloud/api/mcp/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://studio.precog.cloud/api/mcp/oauth/token\nscopes:\n- scope: synesis:mcp\n  description: Access the Precog (Synesis)\
  \ Model Context Protocol server and its tools.\n  flows: [authorizationCode, clientCredentials]\n- scope: admin:read\n  description: Read access to administrative resources over the MCP surface.\n  flows: [authorizationCode, clientCredentials]\n- scope: admin:write\n  description: Write/administrative access over the MCP surface.\n  flows: [authorizationCode, clientCredentials]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/precog/refs/heads/main/scopes/precog-scopes.yml
summary_line: 3 scopes · authorizationCode/clientCredentials
tags:
- Company
- Data Integration
- ETL
- Artificial Intelligence
- Semantic Layer
- MCP
- Data Pipeline
- Analytics
- Enterprise
token_urls:
- https://studio.precog.cloud/api/mcp/oauth/token
---
