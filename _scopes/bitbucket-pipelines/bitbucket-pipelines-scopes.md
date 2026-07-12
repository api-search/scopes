---
authorization_urls:
- https://bitbucket.org/site/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Bitbucket Pipelines Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Bitbucket Pipelines publishes 26 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Bitbucket Pipelines API on a user''s behalf.


  Tokens are issued from https://bitbucket.org/site/oauth2/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bitbucket Pipelines
provider_slug: bitbucket-pipelines
schemes:
- description: OAuth 2 as per [RFC-6749](https://tools.ietf.org/html/rfc6749).
  flows:
  - authorizationUrl: https://bitbucket.org/site/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://bitbucket.org/site/oauth2/access_token
  name: oauth2
  source: openapi/bitbucket-pipelines-openapi.json
scope_count: 26
scope_names:
- account
- account:write
- email
- issue
- issue:write
- pipeline
- pipeline:variable
- pipeline:write
- project
- project:admin
- pullrequest
- pullrequest:write
- repository
- repository:admin
- repository:delete
- repository:write
- runner
- runner:write
- snippet
- snippet:write
- team
- team:write
- test
- test:write
- webhook
- wiki
scopes:
- description: Read your account information
  flows:
  - authorizationCode
  scope: account
- description: Read and modify your account information
  flows:
  - authorizationCode
  scope: account:write
- description: Read your account's primary email address
  flows:
  - authorizationCode
  scope: email
- description: Read your repositories' issues
  flows:
  - authorizationCode
  scope: issue
- description: Read and modify your repositories' issues
  flows:
  - authorizationCode
  scope: issue:write
- description: Access your repositories' build pipelines
  flows:
  - authorizationCode
  scope: pipeline
- description: Access your repositories' build pipelines and configure their variables
  flows:
  - authorizationCode
  scope: pipeline:variable
- description: Access and rerun your repositories' build pipelines
  flows:
  - authorizationCode
  scope: pipeline:write
- description: Read your workspace's project settings and read repositories contained within your workspace's projects
  flows:
  - authorizationCode
  scope: project
- description: Read and modify settings for projects in your workspace
  flows:
  - authorizationCode
  scope: project:admin
- description: Read your repositories and their pull requests
  flows:
  - authorizationCode
  scope: pullrequest
- description: Read and modify your repositories and their pull requests
  flows:
  - authorizationCode
  scope: pullrequest:write
- description: Read your repositories
  flows:
  - authorizationCode
  scope: repository
- description: Administer your repositories
  flows:
  - authorizationCode
  scope: repository:admin
- description: Delete your repositories
  flows:
  - authorizationCode
  scope: repository:delete
- description: Read and modify your repositories
  flows:
  - authorizationCode
  scope: repository:write
- description: Access your workspaces/repositories' runners
  flows:
  - authorizationCode
  scope: runner
- description: Access and edit your workspaces/repositories' runners
  flows:
  - authorizationCode
  scope: runner:write
- description: Read your snippets
  flows:
  - authorizationCode
  scope: snippet
- description: Read and modify your snippets
  flows:
  - authorizationCode
  scope: snippet:write
- description: Read your team membership information
  flows:
  - authorizationCode
  scope: team
- description: Read and modify your team membership information
  flows:
  - authorizationCode
  scope: team:write
- description: Access your workspaces/repositories' test
  flows:
  - authorizationCode
  scope: test
- description: Access and edit your workspaces/repositories' test
  flows:
  - authorizationCode
  scope: test:write
- description: Read and modify your repositories' webhooks
  flows:
  - authorizationCode
  scope: webhook
- description: Read and modify your repositories' wikis
  flows:
  - authorizationCode
  scope: wiki
slug: bitbucket-pipelines-scopes
source_filename: bitbucket-pipelines-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bitbucket-pipelines-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/bitbucket-pipelines-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://bitbucket.org/site/oauth2/authorize\n    tokenUrl: https://bitbucket.org/site/oauth2/access_token\n  description: OAuth 2 as per [RFC-6749](https://tools.ietf.org/html/rfc6749).\nscopes:\n- scope: account\n  description: Read your account information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitbucket-pipelines-openapi.json\n- scope: account:write\n  description: Read and modify your account information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitbucket-pipelines-openapi.json\n- scope: email\n  description: Read your account's primary email address\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitbucket-pipelines-openapi.json\n- scope: issue\n  description: Read your repositories' issues\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - openapi/bitbucket-pipelines-openapi.json\n- scope: issue:write\n  description: Read and modify your repositories' issues\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitbucket-pipelines-openapi.json\n- scope: pipeline\n  description: Access your repositories' build pipelines\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitbucket-pipelines-openapi.json\n- scope: pipeline:variable\n  description: Access your repositories' build pipelines and configure their variables\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitbucket-pipelines-openapi.json\n- scope: pipeline:write\n  description: Access and rerun your repositories' build pipelines\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitbucket-pipelines-openapi.json\n- scope: project\n  description: Read your workspace's project settings and read repositories contained within\n    your workspace's projects\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/bitbucket-pipelines-openapi.json\n- scope: project:admin\n  description: Read and modify settings for projects in your workspace\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitbucket-pipelines-openapi.json\n- scope: pullrequest\n  description: Read your repositories and their pull requests\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitbucket-pipelines-openapi.json\n- scope: pullrequest:write\n  description: Read and modify your repositories and their pull requests\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitbucket-pipelines-openapi.json\n- scope: repository\n  description: Read your repositories\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitbucket-pipelines-openapi.json\n- scope: repository:admin\n  description: Administer your repositories\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitbucket-pipelines-openapi.json\n- scope: repository:delete\n  description: Delete your repositories\n  flows:\n  -\
  \ authorizationCode\n  sources:\n  - openapi/bitbucket-pipelines-openapi.json\n- scope: repository:write\n  description: Read and modify your repositories\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitbucket-pipelines-openapi.json\n- scope: runner\n  description: Access your workspaces/repositories' runners\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitbucket-pipelines-openapi.json\n- scope: runner:write\n  description: Access and edit your workspaces/repositories' runners\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitbucket-pipelines-openapi.json\n- scope: snippet\n  description: Read your snippets\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitbucket-pipelines-openapi.json\n- scope: snippet:write\n  description: Read and modify your snippets\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitbucket-pipelines-openapi.json\n- scope: team\n  description: Read your team membership information\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/bitbucket-pipelines-openapi.json\n- scope: team:write\n  description: Read and modify your team membership information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitbucket-pipelines-openapi.json\n- scope: test\n  description: Access your workspaces/repositories' test\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitbucket-pipelines-openapi.json\n- scope: test:write\n  description: Access and edit your workspaces/repositories' test\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitbucket-pipelines-openapi.json\n- scope: webhook\n  description: Read and modify your repositories' webhooks\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitbucket-pipelines-openapi.json\n- scope: wiki\n  description: Read and modify your repositories' wikis\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitbucket-pipelines-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitbucket-pipelines/refs/heads/main/scopes/bitbucket-pipelines-scopes.yml
summary_line: 26 scopes · authorizationCode
tags:
- DevOps
- CI/CD
- Pipelines
- Atlassian
- Bitbucket
- Hosted
- Self-Hosted Runners
token_urls:
- https://bitbucket.org/site/oauth2/access_token
---
