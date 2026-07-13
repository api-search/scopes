---
api_specs:
- filename: linear-graphql-openapi.yml
  format: yaml
  label: Linear GraphQL API
  slug: linear-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linear/refs/heads/main/openapi/linear-graphql-openapi.yml
- filename: linear-webhooks-asyncapi.yml
  format: yaml
  label: Linear Webhooks API
  slug: linear-webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/linear/refs/heads/main/asyncapi/linear-webhooks-asyncapi.yml
authorization_urls:
- https://linear.app/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Linear Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'linear publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the linear API on a user''s behalf.


  Tokens are issued from https://api.linear.app/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: linear
provider_slug: linear
schemes:
- description: OAuth 2.0 authorization code flow
  flows:
  - authorizationUrl: https://linear.app/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.linear.app/oauth/token
  name: OAuth2
  source: openapi/linear-graphql-openapi.yml
scope_count: 4
scope_names:
- issues:create
- issues:read
- read
- write
scopes:
- description: Create issues
  flows:
  - authorizationCode
  scope: issues:create
- description: Read issues
  flows:
  - authorizationCode
  scope: issues:read
- description: Read access to all resources
  flows:
  - authorizationCode
  scope: read
- description: Write access to all resources
  flows:
  - authorizationCode
  scope: write
slug: linear-scopes
source_filename: linear-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/linear-graphql-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/linear-graphql-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://linear.app/oauth/authorize\n    tokenUrl: https://api.linear.app/oauth/token\n  description: OAuth 2.0 authorization code flow\nscopes:\n- scope: issues:create\n  description: Create issues\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/linear-graphql-openapi.yml\n- scope: issues:read\n  description: Read issues\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/linear-graphql-openapi.yml\n- scope: read\n  description: Read access to all resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/linear-graphql-openapi.yml\n- scope: write\n  description: Write access to all resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/linear-graphql-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linear/refs/heads/main/scopes/linear-scopes.yml
summary_line: 4 scopes · authorizationCode
tags: []
token_urls:
- https://api.linear.app/oauth/token
---
