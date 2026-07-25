---
api_specs:
- filename: microsoft-azure-repo-commits-api-openapi.yml
  format: yaml
  label: Azure Repos Commits API
  slug: microsoft-azure-repo-commits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-repo/refs/heads/main/openapi/microsoft-azure-repo-commits-api-openapi.yml
- filename: microsoft-azure-repo-items-api-openapi.yml
  format: yaml
  label: Azure Repos Items API
  slug: microsoft-azure-repo-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-repo/refs/heads/main/openapi/microsoft-azure-repo-items-api-openapi.yml
- filename: microsoft-azure-repo-pull-request-reviewers-api-openapi.yml
  format: yaml
  label: Azure Repos Pull Request Reviewers API
  slug: microsoft-azure-repo-pull-request-reviewers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-repo/refs/heads/main/openapi/microsoft-azure-repo-pull-request-reviewers-api-openapi.yml
- filename: microsoft-azure-repo-pull-request-threads-api-openapi.yml
  format: yaml
  label: Azure Repos Pull Request Threads API
  slug: microsoft-azure-repo-pull-request-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-repo/refs/heads/main/openapi/microsoft-azure-repo-pull-request-threads-api-openapi.yml
- filename: microsoft-azure-repo-pull-requests-api-openapi.yml
  format: yaml
  label: Azure Repos Pull Requests API
  slug: microsoft-azure-repo-pull-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-repo/refs/heads/main/openapi/microsoft-azure-repo-pull-requests-api-openapi.yml
- filename: microsoft-azure-repo-pushes-api-openapi.yml
  format: yaml
  label: Azure Repos Pushes API
  slug: microsoft-azure-repo-pushes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-repo/refs/heads/main/openapi/microsoft-azure-repo-pushes-api-openapi.yml
- filename: microsoft-azure-repo-refs-api-openapi.yml
  format: yaml
  label: Azure Repos Refs API
  slug: microsoft-azure-repo-refs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-repo/refs/heads/main/openapi/microsoft-azure-repo-refs-api-openapi.yml
- filename: microsoft-azure-repo-repositories-api-openapi.yml
  format: yaml
  label: Azure Repos Repositories API
  slug: microsoft-azure-repo-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-repo/refs/heads/main/openapi/microsoft-azure-repo-repositories-api-openapi.yml
- filename: microsoft-azure-repo-stats-api-openapi.yml
  format: yaml
  label: Azure Repos Stats API
  slug: microsoft-azure-repo-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-repo/refs/heads/main/openapi/microsoft-azure-repo-stats-api-openapi.yml
authorization_urls:
- https://app.vssps.visualstudio.com/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Microsoft Azure Repo Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Azure Repos publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Azure Repos API on a user''s behalf.


  Tokens are issued from https://app.vssps.visualstudio.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Azure Repos
provider_slug: microsoft-azure-repo
schemes:
- description: OAuth 2.0 authorization code flow for Azure DevOps Services. Requires the vso.code scope for read operations and vso.code_write for write operations.
  flows:
  - authorizationUrl: https://app.vssps.visualstudio.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://app.vssps.visualstudio.com/oauth2/token
  name: oauth2
  source: openapi/azure-repo-git-api-openapi.yml
scope_count: 3
scope_names:
- vso.code
- vso.code_manage
- vso.code_write
scopes:
- description: Read source code and metadata about commits, changesets, branches, and other version control artifacts
  flows:
  - authorizationCode
  scope: vso.code
- description: Read, create, manage, and delete repositories and branches
  flows:
  - authorizationCode
  scope: vso.code_manage
- description: Read, create, and manage pull requests and code
  flows:
  - authorizationCode
  scope: vso.code_write
slug: microsoft-azure-repo-scopes
source_filename: microsoft-azure-repo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-repo-git-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/azure-repo-git-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.vssps.visualstudio.com/oauth2/authorize\n    tokenUrl: https://app.vssps.visualstudio.com/oauth2/token\n  description: OAuth 2.0 authorization code flow for Azure DevOps Services. Requires the vso.code\n    scope for read operations and vso.code_write for write operations.\nscopes:\n- scope: vso.code\n  description: Read source code and metadata about commits, changesets, branches, and other\n    version control artifacts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/azure-repo-git-api-openapi.yml\n- scope: vso.code_manage\n  description: Read, create, manage, and delete repositories and branches\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/azure-repo-git-api-openapi.yml\n- scope: vso.code_write\n  description: Read,\
  \ create, and manage pull requests and code\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/azure-repo-git-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-repo/refs/heads/main/scopes/microsoft-azure-repo-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- DevOps
- Git
- Repositories
- Source Control
- TFVC
- Version Control
token_urls:
- https://app.vssps.visualstudio.com/oauth2/token
---
