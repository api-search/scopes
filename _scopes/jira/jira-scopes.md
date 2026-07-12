---
authorization_urls:
- https://auth.atlassian.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Jira Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Jira publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Jira API on a user''s behalf.


  Tokens are issued from https://auth.atlassian.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Jira
provider_slug: jira
schemes:
- description: OAuth 2.0 authorization code grant (3LO) for Jira Cloud apps.
  flows:
  - authorizationUrl: https://auth.atlassian.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.atlassian.com/oauth/token
  name: oauth2
  source: openapi/jira-cloud-platform-rest-api-openapi.yml
scope_count: 5
scope_names:
- manage:jira-configuration
- manage:jira-project
- read:jira-user
- read:jira-work
- write:jira-work
scopes:
- description: Manage Jira instance configuration.
  flows:
  - authorizationCode
  scope: manage:jira-configuration
- description: Manage Jira project settings.
  flows:
  - authorizationCode
  scope: manage:jira-project
- description: Read Jira user information.
  flows:
  - authorizationCode
  scope: read:jira-user
- description: Read Jira project and issue data.
  flows:
  - authorizationCode
  scope: read:jira-work
- description: Create and edit Jira issues and projects.
  flows:
  - authorizationCode
  scope: write:jira-work
slug: jira-scopes
source_filename: jira-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/jira-cloud-platform-rest-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/jira-cloud-platform-rest-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.atlassian.com/authorize\n    tokenUrl: https://auth.atlassian.com/oauth/token\n  description: OAuth 2.0 authorization code grant (3LO) for Jira Cloud apps.\nscopes:\n- scope: manage:jira-configuration\n  description: Manage Jira instance configuration.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jira-cloud-platform-rest-api-openapi.yml\n- scope: manage:jira-project\n  description: Manage Jira project settings.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jira-cloud-platform-rest-api-openapi.yml\n- scope: read:jira-user\n  description: Read Jira user information.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jira-cloud-platform-rest-api-openapi.yml\n- scope: read:jira-work\n  description:\
  \ Read Jira project and issue data.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jira-cloud-platform-rest-api-openapi.yml\n- scope: write:jira-work\n  description: Create and edit Jira issues and projects.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jira-cloud-platform-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/scopes/jira-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Agile
- Issue Tracking
- ITSM
- Project Management
- Service Management
token_urls:
- https://auth.atlassian.com/oauth/token
---
