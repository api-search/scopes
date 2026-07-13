---
api_specs:
- filename: figma-api-openapi.yml
  format: yaml
  label: Figma API
  slug: figma-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-api-openapi.yml
- filename: figma-rest-api-openapi.yml
  format: yaml
  label: Figma REST API
  slug: figma-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-rest-api-openapi.yml
- filename: figma-files-api-openapi.yml
  format: yaml
  label: Figma Files API
  slug: figma-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-files-api-openapi.yml
- filename: figma-images-api-openapi.yml
  format: yaml
  label: Figma Images API
  slug: figma-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-images-api-openapi.yml
- filename: figma-teams-api-openapi.yml
  format: yaml
  label: Figma Teams API
  slug: figma-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-teams-api-openapi.yml
- filename: figma-projects-api-openapi.yml
  format: yaml
  label: Figma Projects API
  slug: figma-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-projects-api-openapi.yml
- filename: figma-me-api-openapi.yml
  format: yaml
  label: Figma Me API
  slug: figma-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-me-api-openapi.yml
- filename: figma-rest-api-openapi.yml
  format: yaml
  label: Figma Components API
  slug: figma-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-rest-api-openapi.yml
- filename: figma-component-sets-api-openapi.yml
  format: yaml
  label: Figma Component Sets API
  slug: figma-component-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-component-sets-api-openapi.yml
- filename: figma-styles-api-openapi.yml
  format: yaml
  label: Figma Styles API
  slug: figma-styles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-styles-api-openapi.yml
- filename: figma-activity-logs-api-openapi.yml
  format: yaml
  label: Figma Activity Logs API
  slug: figma-activity-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-activity-logs-api-openapi.yml
- filename: figma-payments-api-openapi.yml
  format: yaml
  label: Figma Payments API
  slug: figma-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-payments-api-openapi.yml
- filename: figma-dev-resources-api-openapi.yml
  format: yaml
  label: Figma Dev Resources API
  slug: figma-dev-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-dev-resources-api-openapi.yml
- filename: figma-analytics-api-openapi.yml
  format: yaml
  label: Figma Analytics API
  slug: figma-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-analytics-api-openapi.yml
- filename: figma-rest-api-openapi.yml
  format: yaml
  label: Figma Comments API
  slug: figma-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-rest-api-openapi.yml
- filename: figma-rest-api-openapi.yml
  format: yaml
  label: Figma Version History API
  slug: figma-version-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-rest-api-openapi.yml
- filename: figma-rest-api-openapi.yml
  format: yaml
  label: Figma Variables API
  slug: figma-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-rest-api-openapi.yml
- filename: figma-rest-api-openapi.yml
  format: yaml
  label: Figma Library Analytics API
  slug: figma-library-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-rest-api-openapi.yml
authorization_urls:
- https://www.figma.com/oauth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Figma Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Figma publishes 9 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Figma API on a user''s behalf.


  Tokens are issued from https://api.figma.com/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Figma
provider_slug: figma
schemes:
- flows:
  - authorizationUrl: https://www.figma.com/oauth
    flow: authorizationCode
    tokenUrl: https://api.figma.com/v1/oauth/token
  name: OrgOAuth2
  source: openapi/figma-activity-logs-api-openapi.yml
- flows:
  - authorizationUrl: https://www.figma.com/oauth
    flow: authorizationCode
    tokenUrl: https://api.figma.com/v1/oauth/token
  name: OAuth2
  source: openapi/figma-analytics-api-openapi.yml
- flows:
  - authorizationUrl: https://www.figma.com/oauth
    flow: authorizationCode
    tokenUrl: https://api.figma.com/v1/oauth/token
  name: OAuth2
  source: openapi/figma-api-openapi.yml
- flows:
  - authorizationUrl: https://www.figma.com/oauth
    flow: authorizationCode
    tokenUrl: https://api.figma.com/v1/oauth/token
  name: OAuth2
  source: openapi/figma-component-sets-api-openapi.yml
- flows:
  - authorizationUrl: https://www.figma.com/oauth
    flow: authorizationCode
    tokenUrl: https://api.figma.com/v1/oauth/token
  name: OAuth2
  source: openapi/figma-dev-resources-api-openapi.yml
- flows:
  - authorizationUrl: https://www.figma.com/oauth
    flow: authorizationCode
    tokenUrl: https://api.figma.com/v1/oauth/token
  name: OAuth2
  source: openapi/figma-files-api-openapi.yml
- flows:
  - authorizationUrl: https://www.figma.com/oauth
    flow: authorizationCode
    tokenUrl: https://www.figma.com/api/oauth/token
  name: OAuth2
  source: openapi/figma-images-api-openapi.yml
- flows:
  - authorizationUrl: https://www.figma.com/oauth
    flow: authorizationCode
    tokenUrl: https://www.figma.com/api/oauth/token
  name: OAuth2
  source: openapi/figma-me-api-openapi.yml
- flows:
  - authorizationUrl: https://www.figma.com/oauth
    flow: authorizationCode
    tokenUrl: https://www.figma.com/api/oauth/token
  name: OAuth2
  source: openapi/figma-projects-api-openapi.yml
- description: OAuth 2.0 authorization code flow for Figma. Applications must be registered on the Figma developer portal.
  flows:
  - authorizationUrl: https://www.figma.com/oauth
    flow: authorizationCode
    tokenUrl: https://api.figma.com/v1/oauth/token
  name: OAuth2
  source: openapi/figma-rest-api-openapi.yml
- flows:
  - authorizationUrl: https://www.figma.com/oauth
    flow: authorizationCode
    tokenUrl: https://www.figma.com/api/oauth/token
  name: OAuth2
  source: openapi/figma-styles-api-openapi.yml
- flows:
  - authorizationUrl: https://www.figma.com/oauth
    flow: authorizationCode
    tokenUrl: https://www.figma.com/api/oauth/token
  name: OAuth2
  source: openapi/figma-teams-api-openapi.yml
scope_count: 9
scope_names:
- file_comments:write
- file_dev_resources:read
- file_dev_resources:write
- file_variables:read
- file_variables:write
- files:read
- library_analytics:read
- org:activity_log_read
- webhooks:write
scopes:
- description: Post and delete comments on files
  flows:
  - authorizationCode
  scope: file_comments:write
- description: Read dev resources on files
  flows:
  - authorizationCode
  scope: file_dev_resources:read
- description: Write dev resources to files
  flows:
  - authorizationCode
  scope: file_dev_resources:write
- description: Read access to variables in files
  flows:
  - authorizationCode
  scope: file_variables:read
- description: Write access to variables in files
  flows:
  - authorizationCode
  scope: file_variables:write
- description: Read files
  flows:
  - authorizationCode
  scope: files:read
- description: Read library analytics
  flows:
  - authorizationCode
  scope: library_analytics:read
- description: Read organization activity logs
  flows:
  - authorizationCode
  scope: org:activity_log_read
- description: Create and manage webhooks
  flows:
  - authorizationCode
  scope: webhooks:write
slug: figma-scopes
source_filename: figma-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/figma-activity-logs-api-openapi.yml, openapi/figma-analytics-api-openapi.yml,\n  openapi/figma-api-openapi.yml, openapi/figma-component-sets-api-openapi.yml, openapi/figma-dev-resources-api-openapi.yml,\n  openapi/figma-files-api-openapi.yml, openapi/figma-images-api-openapi.yml, openapi/figma-me-api-openapi.yml,\n  openapi/figma-projects-api-openapi.yml, openapi/figma-rest-api-openapi.yml, openapi/figma-styles-api-openapi.yml,\n  openapi/figma-teams-api-openapi.yml\nschemes:\n- name: OrgOAuth2\n  source: openapi/figma-activity-logs-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.figma.com/oauth\n    tokenUrl: https://api.figma.com/v1/oauth/token\n- name: OAuth2\n  source: openapi/figma-analytics-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.figma.com/oauth\n    tokenUrl: https://api.figma.com/v1/oauth/token\n- name: OAuth2\n  source:\
  \ openapi/figma-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.figma.com/oauth\n    tokenUrl: https://api.figma.com/v1/oauth/token\n- name: OAuth2\n  source: openapi/figma-component-sets-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.figma.com/oauth\n    tokenUrl: https://api.figma.com/v1/oauth/token\n- name: OAuth2\n  source: openapi/figma-dev-resources-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.figma.com/oauth\n    tokenUrl: https://api.figma.com/v1/oauth/token\n- name: OAuth2\n  source: openapi/figma-files-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.figma.com/oauth\n    tokenUrl: https://api.figma.com/v1/oauth/token\n- name: OAuth2\n  source: openapi/figma-images-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.figma.com/oauth\n    tokenUrl: https://www.figma.com/api/oauth/token\n\
  - name: OAuth2\n  source: openapi/figma-me-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.figma.com/oauth\n    tokenUrl: https://www.figma.com/api/oauth/token\n- name: OAuth2\n  source: openapi/figma-projects-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.figma.com/oauth\n    tokenUrl: https://www.figma.com/api/oauth/token\n- name: OAuth2\n  source: openapi/figma-rest-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.figma.com/oauth\n    tokenUrl: https://api.figma.com/v1/oauth/token\n  description: OAuth 2.0 authorization code flow for Figma. Applications must be registered\n    on the Figma developer portal.\n- name: OAuth2\n  source: openapi/figma-styles-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.figma.com/oauth\n    tokenUrl: https://www.figma.com/api/oauth/token\n- name: OAuth2\n  source: openapi/figma-teams-api-openapi.yml\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.figma.com/oauth\n    tokenUrl: https://www.figma.com/api/oauth/token\nscopes:\n- scope: file_comments:write\n  description: Post and delete comments on files\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/figma-rest-api-openapi.yml\n- scope: file_dev_resources:read\n  description: Read dev resources on files\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/figma-rest-api-openapi.yml\n- scope: file_dev_resources:write\n  description: Write dev resources to files\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/figma-dev-resources-api-openapi.yml\n  - openapi/figma-files-api-openapi.yml\n  - openapi/figma-rest-api-openapi.yml\n- scope: file_variables:read\n  description: Read access to variables in files\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/figma-rest-api-openapi.yml\n- scope: file_variables:write\n  description: Write access to variables in files\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/figma-rest-api-openapi.yml\n- scope: files:read\n  description: Read files\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/figma-api-openapi.yml\n  - openapi/figma-component-sets-api-openapi.yml\n  - openapi/figma-files-api-openapi.yml\n  - openapi/figma-images-api-openapi.yml\n  - openapi/figma-me-api-openapi.yml\n  - openapi/figma-projects-api-openapi.yml\n  - openapi/figma-rest-api-openapi.yml\n  - openapi/figma-styles-api-openapi.yml\n  - openapi/figma-teams-api-openapi.yml\n- scope: library_analytics:read\n  description: Read library analytics\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/figma-analytics-api-openapi.yml\n- scope: org:activity_log_read\n  description: Read organization activity logs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/figma-activity-logs-api-openapi.yml\n- scope: webhooks:write\n  description: Create and manage webhooks\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/figma-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/scopes/figma-scopes.yml
summary_line: 9 scopes · authorizationCode
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
token_urls:
- https://api.figma.com/v1/oauth/token
- https://www.figma.com/api/oauth/token
---
