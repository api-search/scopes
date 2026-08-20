---
api_specs:
- filename: unionai-domains-api-openapi.yml
  format: yaml
  label: Union.ai Domains API
  slug: unionai-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unionai/refs/heads/main/openapi/unionai-domains-api-openapi.yml
- filename: unionai-executions-api-openapi.yml
  format: yaml
  label: Union.ai Executions API
  slug: unionai-executions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unionai/refs/heads/main/openapi/unionai-executions-api-openapi.yml
- filename: unionai-launch-plans-api-openapi.yml
  format: yaml
  label: Union.ai Launch Plans API
  slug: unionai-launch-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unionai/refs/heads/main/openapi/unionai-launch-plans-api-openapi.yml
- filename: unionai-node-executions-api-openapi.yml
  format: yaml
  label: Union.ai Node Executions API
  slug: unionai-node-executions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unionai/refs/heads/main/openapi/unionai-node-executions-api-openapi.yml
- filename: unionai-projects-api-openapi.yml
  format: yaml
  label: Union.ai Projects API
  slug: unionai-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unionai/refs/heads/main/openapi/unionai-projects-api-openapi.yml
- filename: unionai-tasks-api-openapi.yml
  format: yaml
  label: Union.ai Tasks API
  slug: unionai-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unionai/refs/heads/main/openapi/unionai-tasks-api-openapi.yml
- filename: unionai-version-api-openapi.yml
  format: yaml
  label: Union.ai Version API
  slug: unionai-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unionai/refs/heads/main/openapi/unionai-version-api-openapi.yml
- filename: unionai-workflows-api-openapi.yml
  format: yaml
  label: Union.ai Workflows API
  slug: unionai-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unionai/refs/heads/main/openapi/unionai-workflows-api-openapi.yml
authorization_urls:
- https://{org}.app.union.ai/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Unionai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Union.ai publishes 1 OAuth 2.0 scope via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Union.ai API on a user''s behalf.


  Tokens are issued from https://{org}.app.union.ai/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Union.ai
provider_slug: unionai
schemes:
- description: FlyteAdmin secures client connections with OAuth2. Interactive CLI/UI clients use the Authorization Code + PKCE flow; machine clients use the Client Credentials flow. User authentication to the console is via OpenID Connect. Tokens are presented as a Bearer access token.
  flows:
  - authorizationUrl: https://{org}.app.union.ai/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://{org}.app.union.ai/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://{org}.app.union.ai/oauth2/token
  name: OAuth2
  source: openapi/unionai-openapi.yml
scope_count: 1
scope_names:
- all
scopes:
- description: Full control-plane access.
  flows:
  - authorizationCode
  - clientCredentials
  scope: all
slug: unionai-scopes
source_filename: unionai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/unionai-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/unionai-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{org}.app.union.ai/oauth2/authorize\n    tokenUrl: https://{org}.app.union.ai/oauth2/token\n  - flow: clientCredentials\n    tokenUrl: https://{org}.app.union.ai/oauth2/token\n  description: FlyteAdmin secures client connections with OAuth2. Interactive CLI/UI clients\n    use the Authorization Code + PKCE flow; machine clients use the Client Credentials flow.\n    User authentication to the console is via OpenID Connect. Tokens are presented as a Bearer\n    access token.\nscopes:\n- scope: all\n  description: Full control-plane access.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/unionai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unionai/refs/heads/main/scopes/unionai-scopes.yml
summary_line: 1 scope · authorizationCode/clientCredentials
tags:
- Artificial Intelligence
- ML
- Orchestration
- Workflows
- MLOps
- Flyte
- Serverless
token_urls:
- https://{org}.app.union.ai/oauth2/token
---
