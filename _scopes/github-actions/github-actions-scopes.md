---
api_specs:
- filename: github-actions-artifacts-api-openapi.yml
  format: yaml
  label: GitHub Actions Artifacts API
  slug: github-actions-artifacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/github-actions/openapi/github-actions-artifacts-api-openapi.yml
- filename: github-actions-cache-api-openapi.yml
  format: yaml
  label: GitHub Actions Cache API
  slug: github-actions-cache-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/github-actions/openapi/github-actions-cache-api-openapi.yml
- filename: github-actions-jobs-api-openapi.yml
  format: yaml
  label: GitHub Actions Jobs API
  slug: github-actions-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/github-actions/openapi/github-actions-jobs-api-openapi.yml
- filename: github-actions-oidc-api-openapi.yml
  format: yaml
  label: GitHub Actions OIDC API
  slug: github-actions-oidc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/github-actions/openapi/github-actions-oidc-api-openapi.yml
- filename: github-actions-permissions-api-openapi.yml
  format: yaml
  label: GitHub Actions Permissions API
  slug: github-actions-permissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/github-actions/openapi/github-actions-permissions-api-openapi.yml
- filename: github-actions-secrets-api-openapi.yml
  format: yaml
  label: GitHub Actions Secrets API
  slug: github-actions-secrets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/github-actions/openapi/github-actions-secrets-api-openapi.yml
- filename: github-actions-self-hosted-runner-groups-api-openapi.yml
  format: yaml
  label: GitHub Actions Self-Hosted Runner Groups API
  slug: github-actions-self-hosted-runner-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/github-actions/openapi/github-actions-self-hosted-runner-groups-api-openapi.yml
- filename: github-actions-self-hosted-runners-api-openapi.yml
  format: yaml
  label: GitHub Actions Self-Hosted Runners API
  slug: github-actions-self-hosted-runners-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/github-actions/openapi/github-actions-self-hosted-runners-api-openapi.yml
- filename: github-actions-variables-api-openapi.yml
  format: yaml
  label: GitHub Actions Variables API
  slug: github-actions-variables-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/github-actions/openapi/github-actions-variables-api-openapi.yml
- filename: github-actions-workflow-runs-api-openapi.yml
  format: yaml
  label: GitHub Actions Workflow Runs API
  slug: github-actions-workflow-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/github-actions/openapi/github-actions-workflow-runs-api-openapi.yml
- filename: github-actions-workflows-api-openapi.yml
  format: yaml
  label: GitHub Actions Workflows API
  slug: github-actions-workflows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/github-actions/openapi/github-actions-workflows-api-openapi.yml
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
overview: 'GitHub Actions publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the GitHub Actions API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: GitHub Actions
provider_slug: github-actions
schemes: []
scope_count: 4
scope_names:
- repo
- workflow
- admin:org
- read:org
scopes:
- description: Full control of private repositories
  flows: []
  scope: repo
- description: Grants the ability to add and update GitHub Actions workflow files. Required to push .github/workflows changes.
  flows: []
  scope: workflow
- description: Manage org-level Actions settings
  flows: []
  scope: admin:org
- description: Read org membership and org-level Actions configuration.
  flows: []
  scope: read:org
slug: github-actions-scopes
source_filename: github-actions-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: https://docs.github.com/en/apps/oauth-apps/building-oauth-apps/scopes-for-oauth-apps and https://docs.github.com/en/rest/authentication/permissions-required-for-fine-grained-personal-access-tokens\ndocs: https://docs.github.com/en/rest/authentication/permissions-required-for-fine-grained-personal-access-tokens\ndescription: 'The OpenAPI declares http-bearer auth without oauth2 flow objects, so scopes are captured\n  from the GitHub docs. GitHub exposes two parallel authorization models: classic OAuth scopes (coarse)\n  and fine-grained token / GitHub App permissions (per-resource read|write). Both relevant to the Actions\n  API are listed here.'\noauth_scopes:\n- scope: repo\n  description: Full control of private repositories\n  including workflow runs: null\n  artifacts: null\n  secrets and variables in private repos.: null\n- scope: workflow\n  description: Grants the ability to add and update GitHub Actions workflow files.\
  \ Required to push .github/workflows\n    changes.\n- scope: admin:org\n  description: Manage org-level Actions settings\n  org secrets/variables: null\n  runner groups and self-hosted runners.: null\n- scope: read:org\n  description: Read org membership and org-level Actions configuration.\nfine_grained_permissions:\n- permission: actions\n  access: read|write\n  description: Workflows, workflow runs, artifacts, caches, job logs and run reruns. Write manages run\n    state and artifacts.\n- permission: secrets\n  access: read|write\n  description: Repository-level Actions secrets (list metadata / create-update-delete).\n- permission: variables\n  access: read|write\n  description: Repository-level Actions variables.\n- permission: environments\n  access: read|write\n  description: Deployment environments\n  environment secrets and variables: null\n  protection rules.: null\n- permission: administration\n  access: read|write\n  description: Actions permissions/policy, cache limits, self-hosted\
  \ runner registration and OIDC subject-claim\n    customization.\n- permission: organization_secrets\n  access: read|write\n  description: Organization Actions secrets.\n- permission: organization_self_hosted_runners\n  access: read|write\n  description: Organization self-hosted runners and runner groups.\nnotes:\n- GITHUB_TOKEN (the automatic token inside a workflow run) is governed by the workflow's `permissions:`\n  block, which maps onto these fine-grained permissions.\nscopes:\n- name: repo\n  description: Full control of private repositories\n- name: workflow\n  description: Grants the ability to add and update GitHub Actions workflow files. Required to push .github/workflows\n    changes.\n- name: admin:org\n  description: Manage org-level Actions settings\n- name: read:org\n  description: Read org membership and org-level Actions configuration.\n"
source_yaml_url: https://artifacts.apis.io/github-actions/scopes/github-actions-scopes.yml
summary_line: 4 scopes
tags:
- CI/CD
- Continuous Integration
- Continuous Deployment
- DevOps
- Pipelines
- Workflows
- Automation
- Developer Tools
- Software Development
- Build Automation
- T1
- GitHub
token_bound: false
token_urls: []
---
