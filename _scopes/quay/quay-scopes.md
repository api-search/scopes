---
api_specs:
- filename: quay-openapi.yml
  format: yaml
  label: Quay
  slug: quay
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quay/refs/heads/main/openapi/quay-openapi.yml
authorization_urls:
- https://quay.io/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Quay Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Quay publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Quay API on a user''s behalf.


  Tokens are issued from https://quay.io/oauth/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Quay
provider_slug: quay
schemes:
- flows:
  - authorizationUrl: https://quay.io/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://quay.io/oauth/access_token
  name: OAuth2
  source: openapi/quay-openapi.yml
scope_count: 6
scope_names:
- org:admin
- repo:admin
- repo:read
- repo:write
- user:admin
- user:read
scopes:
- description: Administer organizations
  flows:
  - authorizationCode
  scope: org:admin
- description: Administer repositories
  flows:
  - authorizationCode
  scope: repo:admin
- description: Read repositories
  flows:
  - authorizationCode
  scope: repo:read
- description: Write repositories
  flows:
  - authorizationCode
  scope: repo:write
- description: Administer the user
  flows:
  - authorizationCode
  scope: user:admin
- description: Read user info
  flows:
  - authorizationCode
  scope: user:read
slug: quay-scopes
source_filename: quay-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/quay-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/quay-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://quay.io/oauth/authorize\n    tokenUrl: https://quay.io/oauth/access_token\nscopes:\n- scope: org:admin\n  description: Administer organizations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/quay-openapi.yml\n- scope: repo:admin\n  description: Administer repositories\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/quay-openapi.yml\n- scope: repo:read\n  description: Read repositories\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/quay-openapi.yml\n- scope: repo:write\n  description: Write repositories\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/quay-openapi.yml\n- scope: user:admin\n  description: Administer the user\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/quay-openapi.yml\n- scope: user:read\n  description:\
  \ Read user info\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/quay-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quay/refs/heads/main/scopes/quay-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Container Images
- Containers
- Red Hat
- Registry
- Security Scanning
token_urls:
- https://quay.io/oauth/access_token
---
