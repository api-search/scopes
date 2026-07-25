---
api_specs:
- filename: ory-api-api-openapi.yml
  format: yaml
  label: Ory api API
  slug: ory-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory/refs/heads/main/openapi/ory-api-api-openapi.yml
- filename: ory-courier-api-openapi.yml
  format: yaml
  label: Ory courier API
  slug: ory-courier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory/refs/heads/main/openapi/ory-courier-api-openapi.yml
- filename: ory-frontend-api-openapi.yml
  format: yaml
  label: Ory frontend API
  slug: ory-frontend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory/refs/heads/main/openapi/ory-frontend-api-openapi.yml
- filename: ory-identity-api-openapi.yml
  format: yaml
  label: Ory identity API
  slug: ory-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory/refs/heads/main/openapi/ory-identity-api-openapi.yml
- filename: ory-jwk-api-openapi.yml
  format: yaml
  label: Ory jwk API
  slug: ory-jwk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory/refs/heads/main/openapi/ory-jwk-api-openapi.yml
- filename: ory-metadata-api-openapi.yml
  format: yaml
  label: Ory metadata API
  slug: ory-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory/refs/heads/main/openapi/ory-metadata-api-openapi.yml
- filename: ory-oauth2-api-openapi.yml
  format: yaml
  label: Ory oAuth2 API
  slug: ory-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory/refs/heads/main/openapi/ory-oauth2-api-openapi.yml
- filename: ory-oidc-api-openapi.yml
  format: yaml
  label: Ory oidc API
  slug: ory-oidc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory/refs/heads/main/openapi/ory-oidc-api-openapi.yml
- filename: ory-permission-api-openapi.yml
  format: yaml
  label: Ory permission API
  slug: ory-permission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory/refs/heads/main/openapi/ory-permission-api-openapi.yml
- filename: ory-relationship-api-openapi.yml
  format: yaml
  label: Ory relationship API
  slug: ory-relationship-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory/refs/heads/main/openapi/ory-relationship-api-openapi.yml
- filename: ory-wellknown-api-openapi.yml
  format: yaml
  label: Ory wellknown API
  slug: ory-wellknown-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory/refs/heads/main/openapi/ory-wellknown-api-openapi.yml
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
