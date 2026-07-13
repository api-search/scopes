---
api_specs:
- filename: mediavalet-openapi.yml
  format: yaml
  label: MediaValet Assets API
  slug: mediavalet-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediavalet/refs/heads/main/openapi/mediavalet-openapi.yml
- filename: mediavalet-openapi.yml
  format: yaml
  label: MediaValet Categories API
  slug: mediavalet-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediavalet/refs/heads/main/openapi/mediavalet-openapi.yml
- filename: mediavalet-openapi.yml
  format: yaml
  label: MediaValet Attributes API
  slug: mediavalet-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediavalet/refs/heads/main/openapi/mediavalet-openapi.yml
- filename: mediavalet-openapi.yml
  format: yaml
  label: MediaValet Keywords API
  slug: mediavalet-keywords-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediavalet/refs/heads/main/openapi/mediavalet-openapi.yml
- filename: mediavalet-openapi.yml
  format: yaml
  label: MediaValet Uploads API
  slug: mediavalet-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediavalet/refs/heads/main/openapi/mediavalet-openapi.yml
- filename: mediavalet-openapi.yml
  format: yaml
  label: MediaValet Users API
  slug: mediavalet-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediavalet/refs/heads/main/openapi/mediavalet-openapi.yml
authorization_urls:
- https://login.mediavalet.com/connect/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Mediavalet Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'MediaValet publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the MediaValet API on a user''s behalf.


  Tokens are issued from https://login.mediavalet.com/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: MediaValet
provider_slug: mediavalet
schemes:
- description: OAuth 2.0 / OpenID Connect. Obtain an access token from https://login.mediavalet.com/connect/token using the authorization code flow (interactive apps) or password / client-credential grants, with scopes openid api offline_access. Send the token as a Bearer Authorization header.
  flows:
  - authorizationUrl: https://login.mediavalet.com/connect/authorize
    flow: authorizationCode
    tokenUrl: https://login.mediavalet.com/connect/token
  name: oauth2
  source: openapi/mediavalet-openapi.yml
scope_count: 3
scope_names:
- api
- offline_access
- openid
scopes:
- description: Access the MediaValet API
  flows:
  - authorizationCode
  scope: api
- description: Obtain a refresh token
  flows:
  - authorizationCode
  scope: offline_access
- description: OpenID Connect identity
  flows:
  - authorizationCode
  scope: openid
slug: mediavalet-scopes
source_filename: mediavalet-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mediavalet-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/mediavalet-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.mediavalet.com/connect/authorize\n    tokenUrl: https://login.mediavalet.com/connect/token\n  description: OAuth 2.0 / OpenID Connect. Obtain an access token from https://login.mediavalet.com/connect/token\n    using the authorization code flow (interactive apps) or password / client-credential grants,\n    with scopes openid api offline_access. Send the token as a Bearer Authorization header.\nscopes:\n- scope: api\n  description: Access the MediaValet API\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/mediavalet-openapi.yml\n- scope: offline_access\n  description: Obtain a refresh token\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/mediavalet-openapi.yml\n- scope: openid\n  description: OpenID Connect identity\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/mediavalet-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mediavalet/refs/heads/main/scopes/mediavalet-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Digital Asset Management
- DAM
- Media
- Assets
- Content
- Marketing
- Cloud Storage
token_urls:
- https://login.mediavalet.com/connect/token
---
