---
api_specs:
- filename: github-actions-artifacts-api-openapi.yml
  format: yaml
  label: GitHub Actions Artifacts API
  slug: github-actions-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/openapi/github-actions-artifacts-api-openapi.yml
- filename: github-actions-cache-api-openapi.yml
  format: yaml
  label: GitHub Actions Cache API
  slug: github-actions-cache-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/openapi/github-actions-cache-api-openapi.yml
- filename: github-actions-jobs-api-openapi.yml
  format: yaml
  label: GitHub Actions Jobs API
  slug: github-actions-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/openapi/github-actions-jobs-api-openapi.yml
- filename: github-actions-oidc-api-openapi.yml
  format: yaml
  label: GitHub Actions OIDC API
  slug: github-actions-oidc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/openapi/github-actions-oidc-api-openapi.yml
- filename: github-actions-permissions-api-openapi.yml
  format: yaml
  label: GitHub Actions Permissions API
  slug: github-actions-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/openapi/github-actions-permissions-api-openapi.yml
- filename: github-actions-secrets-api-openapi.yml
  format: yaml
  label: GitHub Actions Secrets API
  slug: github-actions-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/openapi/github-actions-secrets-api-openapi.yml
- filename: github-actions-self-hosted-runner-groups-api-openapi.yml
  format: yaml
  label: GitHub Actions Self-Hosted Runner Groups API
  slug: github-actions-self-hosted-runner-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/openapi/github-actions-self-hosted-runner-groups-api-openapi.yml
- filename: github-actions-self-hosted-runners-api-openapi.yml
  format: yaml
  label: GitHub Actions Self-Hosted Runners API
  slug: github-actions-self-hosted-runners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/openapi/github-actions-self-hosted-runners-api-openapi.yml
- filename: github-actions-variables-api-openapi.yml
  format: yaml
  label: GitHub Actions Variables API
  slug: github-actions-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/openapi/github-actions-variables-api-openapi.yml
- filename: github-actions-workflow-runs-api-openapi.yml
  format: yaml
  label: GitHub Actions Workflow Runs API
  slug: github-actions-workflow-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/openapi/github-actions-workflow-runs-api-openapi.yml
- filename: github-actions-workflows-api-openapi.yml
  format: yaml
  label: GitHub Actions Workflows API
  slug: github-actions-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/openapi/github-actions-workflows-api-openapi.yml
authorization_urls: []
description: 'The OpenAPI declares http-bearer auth without oauth2 flow objects, so scopes are captured from the GitHub docs. GitHub exposes two parallel authorization models: classic OAuth scopes (coarse) and fine-grained token / GitHub App permissions (per-resource read|write). Both relevant to the Actions API are listed here.'
docs: https://docs.github.com/en/rest/authentication/permissions-required-for-fine-grained-personal-access-tokens
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Github Actions Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'GitHub Actions uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: GitHub Actions
provider_slug: github-actions
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: github-actions-scopes
source_filename: github-actions-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: >-\n  https://docs.github.com/en/apps/oauth-apps/building-oauth-apps/scopes-for-oauth-apps\n  and https://docs.github.com/en/rest/authentication/permissions-required-for-fine-grained-personal-access-tokens\ndocs: https://docs.github.com/en/rest/authentication/permissions-required-for-fine-grained-personal-access-tokens\ndescription: >-\n  The OpenAPI declares http-bearer auth without oauth2 flow objects, so scopes\n  are captured from the GitHub docs. GitHub exposes two parallel authorization\n  models: classic OAuth scopes (coarse) and fine-grained token / GitHub App\n  permissions (per-resource read|write). Both relevant to the Actions API are\n  listed here.\noauth_scopes:\n  - {scope: repo, description: Full control of private repositories, including workflow runs, artifacts, secrets and variables in private repos.}\n  - {scope: workflow, description: Grants the ability to add and update GitHub Actions workflow files. Required\
  \ to push .github/workflows changes.}\n  - {scope: 'admin:org', description: Manage org-level Actions settings, org secrets/variables, runner groups and self-hosted runners.}\n  - {scope: 'read:org', description: Read org membership and org-level Actions configuration.}\nfine_grained_permissions:\n  - {permission: actions, access: 'read|write', description: 'Workflows, workflow runs, artifacts, caches, job logs and run reruns. Write manages run state and artifacts.'}\n  - {permission: secrets, access: 'read|write', description: Repository-level Actions secrets (list metadata / create-update-delete).}\n  - {permission: variables, access: 'read|write', description: Repository-level Actions variables.}\n  - {permission: environments, access: 'read|write', description: Deployment environments, environment secrets and variables, protection rules.}\n  - {permission: administration, access: 'read|write', description: 'Actions permissions/policy, cache limits, self-hosted runner registration and\
  \ OIDC subject-claim customization.'}\n  - {permission: organization_secrets, access: 'read|write', description: Organization Actions secrets.}\n  - {permission: organization_self_hosted_runners, access: 'read|write', description: Organization self-hosted runners and runner groups.}\nnotes:\n  - GITHUB_TOKEN (the automatic token inside a workflow run) is governed by the workflow's `permissions:` block, which maps onto these fine-grained permissions.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/scopes/github-actions-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags: []
token_urls: []
---
