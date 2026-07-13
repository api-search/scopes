---
api_specs:
- filename: azure-devops-work-items-openapi.yml
  format: yaml
  label: Azure DevOps Work Item Tracking API
  slug: azure-devops-work-item-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-devops/refs/heads/main/openapi/azure-devops-work-items-openapi.yml
- filename: azure-devops-pipelines-openapi.yml
  format: yaml
  label: Azure DevOps Pipelines API
  slug: azure-devops-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-devops/refs/heads/main/openapi/azure-devops-pipelines-openapi.yml
authorization_urls:
- https://app.vssps.visualstudio.com/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Azure Devops Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Azure DevOps publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Azure DevOps API on a user''s behalf.


  Tokens are issued from https://app.vssps.visualstudio.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Azure DevOps
provider_slug: azure-devops
schemes:
- flows:
  - authorizationUrl: https://app.vssps.visualstudio.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://app.vssps.visualstudio.com/oauth2/token
  name: oauth2
  source: openapi/azure-devops-pipelines-openapi.yml
- flows:
  - authorizationUrl: https://app.vssps.visualstudio.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://app.vssps.visualstudio.com/oauth2/token
  name: oauth2
  source: openapi/azure-devops-work-items-openapi.yml
scope_count: 4
scope_names:
- vso.build
- vso.build_execute
- vso.work
- vso.work_write
scopes:
- description: Read build data
  flows:
  - authorizationCode
  scope: vso.build
- description: Queue and manage builds
  flows:
  - authorizationCode
  scope: vso.build_execute
- description: Read work items
  flows:
  - authorizationCode
  scope: vso.work
- description: Read and write work items
  flows:
  - authorizationCode
  scope: vso.work_write
slug: azure-devops-scopes
source_filename: azure-devops-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-devops-pipelines-openapi.yml, openapi/azure-devops-work-items-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/azure-devops-pipelines-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.vssps.visualstudio.com/oauth2/authorize\n    tokenUrl: https://app.vssps.visualstudio.com/oauth2/token\n- name: oauth2\n  source: openapi/azure-devops-work-items-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.vssps.visualstudio.com/oauth2/authorize\n    tokenUrl: https://app.vssps.visualstudio.com/oauth2/token\nscopes:\n- scope: vso.build\n  description: Read build data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/azure-devops-pipelines-openapi.yml\n- scope: vso.build_execute\n  description: Queue and manage builds\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/azure-devops-pipelines-openapi.yml\n- scope: vso.work\n  description:\
  \ Read work items\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/azure-devops-work-items-openapi.yml\n- scope: vso.work_write\n  description: Read and write work items\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/azure-devops-work-items-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-devops/refs/heads/main/scopes/azure-devops-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Azure
- CI/CD
- DevOps
- Pipelines
- Work Items
token_urls:
- https://app.vssps.visualstudio.com/oauth2/token
---
