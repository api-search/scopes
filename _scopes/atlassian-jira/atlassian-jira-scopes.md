---
api_specs:
- filename: swagger-v3.v3.json
  format: json
  label: Jira Cloud Platform REST API
  slug: jira-cloud-platform-rest-api
  spec_type: OpenAPI
  url: https://developer.atlassian.com/cloud/jira/platform/swagger-v3.v3.json
- filename: swagger.v3.json
  format: json
  label: Jira Software Cloud REST API
  slug: jira-software-cloud-rest-api
  spec_type: OpenAPI
  url: https://developer.atlassian.com/cloud/jira/software/swagger.v3.json
- filename: swagger.v3.json
  format: json
  label: Jira Service Management REST API
  slug: jira-service-management-rest-api
  spec_type: OpenAPI
  url: https://developer.atlassian.com/cloud/jira/service-desk/swagger.v3.json
authorization_urls:
- https://auth.atlassian.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Atlassian Jira Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Atlassian Jira publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Atlassian Jira API on a user''s behalf.


  Tokens are issued from https://auth.atlassian.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Atlassian Jira
provider_slug: atlassian-jira
schemes:
- description: Atlassian OAuth 2.0 (3LO) for Jira Cloud.
  flows:
  - authorizationUrl: https://auth.atlassian.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.atlassian.com/oauth/token
  name: OAuth2
  source: openapi/atlassian-jira-openapi.yml
scope_count: 4
scope_names:
- manage:jira-project
- read:jira-user
- read:jira-work
- write:jira-work
scopes:
- description: Manage Jira projects
  flows:
  - authorizationCode
  scope: manage:jira-project
- description: Read Jira user
  flows:
  - authorizationCode
  scope: read:jira-user
- description: Read Jira work
  flows:
  - authorizationCode
  scope: read:jira-work
- description: Write Jira work
  flows:
  - authorizationCode
  scope: write:jira-work
slug: atlassian-jira-scopes
source_filename: atlassian-jira-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/atlassian-jira-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/atlassian-jira-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.atlassian.com/authorize\n    tokenUrl: https://auth.atlassian.com/oauth/token\n  description: Atlassian OAuth 2.0 (3LO) for Jira Cloud.\nscopes:\n- scope: manage:jira-project\n  description: Manage Jira projects\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-openapi.yml\n- scope: read:jira-user\n  description: Read Jira user\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-openapi.yml\n- scope: read:jira-work\n  description: Read Jira work\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-openapi.yml\n- scope: write:jira-work\n  description: Write Jira work\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atlassian-jira/refs/heads/main/scopes/atlassian-jira-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Agile
- Atlassian
- Bug Tracking
- Issue Tracking
- ITSM
- Kanban
- Project Management
- Scrum
- Service Desk
token_urls:
- https://auth.atlassian.com/oauth/token
---
