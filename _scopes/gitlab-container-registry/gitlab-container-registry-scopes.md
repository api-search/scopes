---
authorization_urls:
- https://gitlab.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Gitlab Container Registry Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'GitLab Container Registry publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the GitLab Container Registry API on a user''s behalf.


  Tokens are issued from https://gitlab.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: GitLab Container Registry
provider_slug: gitlab-container-registry
schemes:
- flows:
  - authorizationUrl: https://gitlab.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://gitlab.com/oauth/token
  name: OAuth2
  source: openapi/gitlab-container-registry-openapi.yml
scope_count: 1
scope_names:
- api
scopes:
- description: Full API access
  flows:
  - authorizationCode
  scope: api
slug: gitlab-container-registry-scopes
source_filename: gitlab-container-registry-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gitlab-container-registry-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/gitlab-container-registry-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://gitlab.com/oauth/authorize\n    tokenUrl: https://gitlab.com/oauth/token\nscopes:\n- scope: api\n  description: Full API access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gitlab-container-registry-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gitlab-container-registry/refs/heads/main/scopes/gitlab-container-registry-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Container Images
- Containers
- GitLab
- Registry
token_urls:
- https://gitlab.com/oauth/token
---
