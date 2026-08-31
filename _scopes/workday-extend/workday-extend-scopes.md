---
api_specs:
- filename: workday-extend-app-configurations-api-openapi.yml
  format: yaml
  label: Workday Extend App Configurations API
  slug: workday-extend-app-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-app-configurations-api-openapi.yml
- filename: workday-extend-app-deployments-api-openapi.yml
  format: yaml
  label: Workday Extend App Deployments API
  slug: workday-extend-app-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-app-deployments-api-openapi.yml
- filename: workday-extend-app-versions-api-openapi.yml
  format: yaml
  label: Workday Extend App Versions API
  slug: workday-extend-app-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-app-versions-api-openapi.yml
- filename: workday-extend-apps-api-openapi.yml
  format: yaml
  label: Workday Extend Apps API
  slug: workday-extend-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-apps-api-openapi.yml
- filename: workday-extend-custom-object-definitions-api-openapi.yml
  format: yaml
  label: Workday Extend Custom Object Definitions API
  slug: workday-extend-custom-object-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-custom-object-definitions-api-openapi.yml
- filename: workday-extend-custom-object-fields-api-openapi.yml
  format: yaml
  label: Workday Extend Custom Object Fields API
  slug: workday-extend-custom-object-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-custom-object-fields-api-openapi.yml
- filename: workday-extend-custom-object-instances-api-openapi.yml
  format: yaml
  label: Workday Extend Custom Object Instances API
  slug: workday-extend-custom-object-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-custom-object-instances-api-openapi.yml
- filename: workday-extend-graph-query-api-openapi.yml
  format: yaml
  label: Workday Extend Graph Query API
  slug: workday-extend-graph-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-graph-query-api-openapi.yml
- filename: workday-extend-orchestration-executions-api-openapi.yml
  format: yaml
  label: Workday Extend Orchestration Executions API
  slug: workday-extend-orchestration-executions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-orchestration-executions-api-openapi.yml
- filename: workday-extend-orchestration-steps-api-openapi.yml
  format: yaml
  label: Workday Extend Orchestration Steps API
  slug: workday-extend-orchestration-steps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-orchestration-steps-api-openapi.yml
- filename: workday-extend-orchestration-triggers-api-openapi.yml
  format: yaml
  label: Workday Extend Orchestration Triggers API
  slug: workday-extend-orchestration-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-orchestration-triggers-api-openapi.yml
- filename: workday-extend-orchestrations-api-openapi.yml
  format: yaml
  label: Workday Extend Orchestrations API
  slug: workday-extend-orchestrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-orchestrations-api-openapi.yml
- filename: workday-extend-schema-introspection-api-openapi.yml
  format: yaml
  label: Workday Extend Schema Introspection API
  slug: workday-extend-schema-introspection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-schema-introspection-api-openapi.yml
- filename: workday-extend-wql-query-api-openapi.yml
  format: yaml
  label: Workday Extend WQL Query API
  slug: workday-extend-wql-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-wql-query-api-openapi.yml
authorization_urls:
- https://{baseUrl}/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Workday Extend Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Workday Extend publishes 9 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Workday Extend API on a user''s behalf.


  Tokens are issued from https://{baseUrl}/oauth2/{tenant}/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Workday Extend
provider_slug: workday-extend
schemes:
- flows:
  - authorizationUrl: https://{baseUrl}/authorize
    flow: authorizationCode
    tokenUrl: https://{baseUrl}/oauth2/{tenant}/token
  name: OAuth2
  source: openapi/workday-extend-custom-objects-openapi.yml
- flows:
  - authorizationUrl: https://{baseUrl}/authorize
    flow: authorizationCode
    tokenUrl: https://{baseUrl}/oauth2/{tenant}/token
  name: OAuth2
  source: openapi/workday-extend-graph-api-openapi.yml
- flows:
  - authorizationUrl: https://{baseUrl}/authorize
    flow: authorizationCode
    tokenUrl: https://{baseUrl}/oauth2/{tenant}/token
  name: OAuth2
  source: openapi/workday-extend-orchestration-openapi.yml
- flows:
  - authorizationUrl: https://{baseUrl}/authorize
    flow: authorizationCode
    tokenUrl: https://{baseUrl}/oauth2/{tenant}/token
  name: OAuth2
  source: openapi/workday-extend-rest-api-openapi.yml
scope_count: 9
scope_names:
- customObjects:manage
- customObjects:read
- extend:apps
- extend:apps:read
- graph:read
- graph:schema
- orchestrate:executions
- orchestrate:orchestrations
- orchestrate:orchestrations:read
scopes:
- description: Manage custom object definitions and instances
  flows:
  - authorizationCode
  scope: customObjects:manage
- description: Read custom object data
  flows:
  - authorizationCode
  scope: customObjects:read
- description: Manage Extend applications
  flows:
  - authorizationCode
  scope: extend:apps
- description: Read Extend application data
  flows:
  - authorizationCode
  scope: extend:apps:read
- description: Query Workday data through the Graph API
  flows:
  - authorizationCode
  scope: graph:read
- description: Access schema introspection
  flows:
  - authorizationCode
  scope: graph:schema
- description: Execute orchestrations
  flows:
  - authorizationCode
  scope: orchestrate:executions
- description: Manage orchestrations
  flows:
  - authorizationCode
  scope: orchestrate:orchestrations
- description: Read orchestration data
  flows:
  - authorizationCode
  scope: orchestrate:orchestrations:read
slug: workday-extend-scopes
source_filename: workday-extend-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/workday-extend-custom-objects-openapi.yml, openapi/workday-extend-graph-api-openapi.yml,\n  openapi/workday-extend-orchestration-openapi.yml, openapi/workday-extend-rest-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/workday-extend-custom-objects-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{baseUrl}/authorize\n    tokenUrl: https://{baseUrl}/oauth2/{tenant}/token\n- name: OAuth2\n  source: openapi/workday-extend-graph-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{baseUrl}/authorize\n    tokenUrl: https://{baseUrl}/oauth2/{tenant}/token\n- name: OAuth2\n  source: openapi/workday-extend-orchestration-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{baseUrl}/authorize\n    tokenUrl: https://{baseUrl}/oauth2/{tenant}/token\n- name: OAuth2\n  source: openapi/workday-extend-rest-api-openapi.yml\n \
  \ flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{baseUrl}/authorize\n    tokenUrl: https://{baseUrl}/oauth2/{tenant}/token\nscopes:\n- scope: customObjects:manage\n  description: Manage custom object definitions and instances\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/workday-extend-custom-objects-openapi.yml\n- scope: customObjects:read\n  description: Read custom object data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/workday-extend-custom-objects-openapi.yml\n- scope: extend:apps\n  description: Manage Extend applications\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/workday-extend-rest-api-openapi.yml\n- scope: extend:apps:read\n  description: Read Extend application data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/workday-extend-rest-api-openapi.yml\n- scope: graph:read\n  description: Query Workday data through the Graph API\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/workday-extend-graph-api-openapi.yml\n\
  - scope: graph:schema\n  description: Access schema introspection\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/workday-extend-graph-api-openapi.yml\n- scope: orchestrate:executions\n  description: Execute orchestrations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/workday-extend-orchestration-openapi.yml\n- scope: orchestrate:orchestrations\n  description: Manage orchestrations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/workday-extend-orchestration-openapi.yml\n- scope: orchestrate:orchestrations:read\n  description: Read orchestration data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/workday-extend-orchestration-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/scopes/workday-extend-scopes.yml
summary_line: 9 scopes · authorizationCode
tags:
- Automation
- Custom Applications
- Enterprise
- Extensions
- HCM
- Integration
- Orchestration
- PaaS
token_urls:
- https://{baseUrl}/oauth2/{tenant}/token
---
