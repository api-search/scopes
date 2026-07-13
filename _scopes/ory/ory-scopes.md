---
api_specs:
- filename: ory-hydra-openapi.json
  format: json
  label: Ory Hydra
  slug: hydra
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory/refs/heads/main/openapi/ory-hydra-openapi.json
- filename: ory-kratos-openapi.json
  format: json
  label: Ory Kratos
  slug: kratos
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory/refs/heads/main/openapi/ory-kratos-openapi.json
- filename: ory-keto-openapi.json
  format: json
  label: Ory Keto
  slug: keto
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory/refs/heads/main/openapi/ory-keto-openapi.json
- filename: ory-oathkeeper-openapi.json
  format: json
  label: Ory Oathkeeper
  slug: oathkeeper
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory/refs/heads/main/openapi/ory-oathkeeper-openapi.json
authorization_urls:
- https://hydra.demo.ory.sh/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Ory Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Ory publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Ory API on a user''s behalf.


  Tokens are issued from https://hydra.demo.ory.sh/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Ory
provider_slug: ory
schemes:
- flows:
  - authorizationUrl: https://hydra.demo.ory.sh/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://hydra.demo.ory.sh/oauth2/token
  name: oauth2
  source: openapi/ory-hydra-openapi.json
scope_count: 3
scope_names:
- offline
- offline_access
- openid
scopes:
- description: A scope required when requesting refresh tokens (alias for `offline_access`)
  flows:
  - authorizationCode
  scope: offline
- description: A scope required when requesting refresh tokens
  flows:
  - authorizationCode
  scope: offline_access
- description: Request an OpenID Connect ID Token
  flows:
  - authorizationCode
  scope: openid
slug: ory-scopes
source_filename: ory-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ory-hydra-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/ory-hydra-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://hydra.demo.ory.sh/oauth2/auth\n    tokenUrl: https://hydra.demo.ory.sh/oauth2/token\nscopes:\n- scope: offline\n  description: A scope required when requesting refresh tokens (alias for `offline_access`)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ory-hydra-openapi.json\n- scope: offline_access\n  description: A scope required when requesting refresh tokens\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ory-hydra-openapi.json\n- scope: openid\n  description: Request an OpenID Connect ID Token\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ory-hydra-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ory/refs/heads/main/scopes/ory-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Authentication
- Authorization
- Identity
- OAuth2
- OpenID Connect
- Open Source
token_urls:
- https://hydra.demo.ory.sh/oauth2/token
---
