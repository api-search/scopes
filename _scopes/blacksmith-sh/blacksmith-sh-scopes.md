---
api_specs:
- filename: blacksmith-sh-openapi.yml
  format: yaml
  label: Blacksmith GitHub Actions Runners
  slug: github-actions-runners
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blacksmith-sh/refs/heads/main/openapi/blacksmith-sh-openapi.yml
- filename: blacksmith-sh-openapi.yml
  format: yaml
  label: Blacksmith Docker Builds
  slug: docker-builds
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blacksmith-sh/refs/heads/main/openapi/blacksmith-sh-openapi.yml
- filename: blacksmith-sh-openapi.yml
  format: yaml
  label: Blacksmith Cache
  slug: cache
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blacksmith-sh/refs/heads/main/openapi/blacksmith-sh-openapi.yml
authorization_urls:
- https://github.com/apps/blacksmith
description: ''
docs: https://docs.blacksmith.sh/blacksmith-administration/permissions
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Blacksmith Sh Scopes
name_suffix: OAuth Scopes
note: Blacksmith publishes no OAuth scopes - login is exclusively GitHub SSO via the Blacksmith GitHub App, and dashboard access is role-based, inherited directly from GitHub organization/repository permissions rather than granted through scopes (https://docs.blacksmith.sh/blacksmith-administration/permissions).
overview: 'Blacksmith uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://github.com/login/oauth/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Blacksmith
provider_slug: blacksmith-sh
schemes:
- description: Access to Blacksmith is authorized through the Blacksmith GitHub App installed on a GitHub organization, not via a public API key or bearer token. There is no documented machine-to-machine API auth scheme.
  flows:
  - authorizationUrl: https://github.com/apps/blacksmith
    flow: authorizationCode
    tokenUrl: https://github.com/login/oauth/access_token
  name: githubApp
  source: openapi/blacksmith-sh-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: blacksmith-sh-scopes
source_filename: blacksmith-sh-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/blacksmith-sh-openapi.yml\ndocs: https://docs.blacksmith.sh/blacksmith-administration/permissions\nnote: Blacksmith publishes no OAuth scopes - login is exclusively GitHub SSO via\n  the Blacksmith GitHub App, and dashboard access is role-based, inherited directly\n  from GitHub organization/repository permissions rather than granted through scopes\n  (https://docs.blacksmith.sh/blacksmith-administration/permissions).\nschemes:\n- name: githubApp\n  source: openapi/blacksmith-sh-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://github.com/apps/blacksmith\n    tokenUrl: https://github.com/login/oauth/access_token\n  description: Access to Blacksmith is authorized through the Blacksmith GitHub App installed\n    on a GitHub organization, not via a public API key or bearer token. There is no documented\n    machine-to-machine API auth scheme.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blacksmith-sh/refs/heads/main/scopes/blacksmith-sh-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- CI/CD
- GitHub Actions
- Runners
- Caching
- Docker
token_urls:
- https://github.com/login/oauth/access_token
---
