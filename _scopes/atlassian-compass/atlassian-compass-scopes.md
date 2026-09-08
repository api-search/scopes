---
api_specs:
- filename: atlassian-compass-compass-rest-api-openapi.json
  format: json
  label: Atlassian Compass REST API
  slug: atlassian-compass-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlassian-compass/refs/heads/main/openapi/atlassian-compass-compass-rest-api-openapi.json
- filename: atlassian-compass-events-api-openapi.yml
  format: yaml
  label: Atlassian Compass Events API
  slug: atlassian-compass-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlassian-compass/refs/heads/main/openapi/atlassian-compass-events-api-openapi.yml
- filename: atlassian-compass-metrics-api-openapi.yml
  format: yaml
  label: Atlassian Compass Metrics API
  slug: atlassian-compass-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlassian-compass/refs/heads/main/openapi/atlassian-compass-metrics-api-openapi.yml
authorization_urls:
- https://auth.atlassian.com/authorize
description: ''
docs: https://developer.atlassian.com/cloud/compass/rest/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Atlassian Compass Scopes
name_suffix: OAuth Scopes
note: 'The four Compass scopes are declared in Atlassian''s published OpenAPI oauth2 securityScheme. Atlassian does not publish a separate Compass scopes reference page - the contract is the reference. Two further scope namespaces reach Compass data from adjacent surfaces and are recorded below rather than merged into the list, because they are not Compass scopes: the Atlassian Rovo MCP Server grants Compass access through the read_compass and write_compass permission groups, and the Teamwork Graph scopes read:all:twg / write:all:twg reach Compass components through the MCP graph tools.'
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
  source: openapi/atlassian-compass-events-api-openapi.yml
- description: OAuth 2.0 (3LO) for Atlassian Cloud
  flows:
  - authorizationUrl: https://auth.atlassian.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.atlassian.com/oauth/token
  name: oauth2
  source: openapi/atlassian-compass-metrics-api-openapi.yml
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
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: openapi/atlassian-compass-events-api-openapi.yml, openapi/atlassian-compass-metrics-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/atlassian-compass-events-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.atlassian.com/authorize\n    tokenUrl: https://auth.atlassian.com/oauth/token\n  description: OAuth 2.0 (3LO) for Atlassian Cloud\n- name: oauth2\n  source: openapi/atlassian-compass-metrics-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.atlassian.com/authorize\n    tokenUrl: https://auth.atlassian.com/oauth/token\n  description: OAuth 2.0 (3LO) for Atlassian Cloud\nscopes:\n- scope: read:component:compass\n  description: Read component data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-compass-events-api-openapi.yml\n  - openapi/atlassian-compass-metrics-api-openapi.yml\n- scope: write:component:compass\n\
  \  description: Write component data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-compass-events-api-openapi.yml\n  - openapi/atlassian-compass-metrics-api-openapi.yml\n- scope: write:event:compass\n  description: Send events\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-compass-events-api-openapi.yml\n  - openapi/atlassian-compass-metrics-api-openapi.yml\n- scope: write:metric:compass\n  description: Send metric values\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-compass-events-api-openapi.yml\n  - openapi/atlassian-compass-metrics-api-openapi.yml\ndocs: https://developer.atlassian.com/cloud/compass/rest/\nnote: 'The four Compass scopes are declared in Atlassian''s published OpenAPI oauth2 securityScheme. Atlassian\n  does not publish a separate Compass scopes reference page - the contract is the reference. Two further\n  scope namespaces reach Compass data from adjacent surfaces and are recorded below rather than merged\n\
  \  into the list, because they are not Compass scopes: the Atlassian Rovo MCP Server grants Compass access\n  through the read_compass and write_compass permission groups, and the Teamwork Graph scopes read:all:twg\n  / write:all:twg reach Compass components through the MCP graph tools.'\nadjacent_scopes:\n- surface: Atlassian Rovo MCP Server\n  permission_groups:\n  - read_compass\n  - write_compass\n  auth: OAuth 2.1 only; API-token authentication is not supported for Compass\n  source: https://github.com/atlassian/atlassian-mcp-server\n- surface: Atlassian Rovo MCP Server - Teamwork Graph\n  scopes:\n  - read:all:twg\n  - write:all:twg\n  note: Atlassian documents \"Compass - components\" as an entry point for the Teamwork Graph tools\n  source: https://support.atlassian.com/atlassian-rovo-mcp-server/docs/supported-tools/\n"
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
