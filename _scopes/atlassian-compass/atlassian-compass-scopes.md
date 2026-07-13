---
api_specs:
- filename: atlassian-compass-openapi.yml
  format: yaml
  label: Atlassian Compass REST API
  slug: atlassian-compass-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlassian-compass/refs/heads/main/openapi/atlassian-compass-openapi.yml
authorization_urls:
- https://auth.atlassian.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Atlassian Compass Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Atlassian Compass publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Atlassian Compass API on a user''s behalf.


  Tokens are issued from https://auth.atlassian.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Atlassian Compass
provider_slug: atlassian-compass
schemes:
- description: OAuth 2.0 (3LO) for Atlassian Cloud
  flows:
  - authorizationUrl: https://auth.atlassian.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.atlassian.com/oauth/token
  name: oauth2
  source: openapi/atlassian-compass-openapi.yml
scope_count: 4
scope_names:
- read:component:compass
- write:component:compass
- write:event:compass
- write:metric:compass
scopes:
- description: Read component data
  flows:
  - authorizationCode
  scope: read:component:compass
- description: Write component data
  flows:
  - authorizationCode
  scope: write:component:compass
- description: Send events
  flows:
  - authorizationCode
  scope: write:event:compass
- description: Send metric values
  flows:
  - authorizationCode
  scope: write:metric:compass
slug: atlassian-compass-scopes
source_filename: atlassian-compass-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/atlassian-compass-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/atlassian-compass-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.atlassian.com/authorize\n    tokenUrl: https://auth.atlassian.com/oauth/token\n  description: OAuth 2.0 (3LO) for Atlassian Cloud\nscopes:\n- scope: read:component:compass\n  description: Read component data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-compass-openapi.yml\n- scope: write:component:compass\n  description: Write component data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-compass-openapi.yml\n- scope: write:event:compass\n  description: Send events\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-compass-openapi.yml\n- scope: write:metric:compass\n  description: Send metric values\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-compass-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atlassian-compass/refs/heads/main/scopes/atlassian-compass-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Atlassian
- Component Management
- Developer Experience
- Software Catalog
- GraphQL
token_urls:
- https://auth.atlassian.com/oauth/token
---
