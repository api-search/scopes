---
api_specs:
- filename: drupal-rest-api-openapi.yml
  format: yaml
  label: Drupal REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drupal/refs/heads/main/openapi/drupal-rest-api-openapi.yml
- filename: drupal-jsonapi-openapi.yml
  format: yaml
  label: Drupal JSON:API
  slug: jsonapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drupal/refs/heads/main/openapi/drupal-jsonapi-openapi.yml
authorization_urls:
- https://example.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Drupal Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'drupal publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the drupal API on a user''s behalf.


  Tokens are issued from https://example.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: drupal
provider_slug: drupal
schemes:
- description: OAuth 2.0 via the Simple OAuth module.
  flows:
  - authorizationUrl: https://example.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://example.com/oauth/token
  name: oAuth2
  source: openapi/drupal-jsonapi-openapi.yml
- description: OAuth 2.0 authentication via the Simple OAuth module.
  flows:
  - authorizationUrl: https://example.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://example.com/oauth/token
  name: oAuth2
  source: openapi/drupal-rest-api-openapi.yml
scope_count: 2
scope_names:
- content
- user
scopes:
- description: Access and manage content entities
  flows:
  - authorizationCode
  scope: content
- description: Access and manage user entities
  flows:
  - authorizationCode
  scope: user
slug: drupal-scopes
source_filename: drupal-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/drupal-jsonapi-openapi.yml, openapi/drupal-rest-api-openapi.yml\nschemes:\n- name: oAuth2\n  source: openapi/drupal-jsonapi-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://example.com/oauth/authorize\n    tokenUrl: https://example.com/oauth/token\n  description: OAuth 2.0 via the Simple OAuth module.\n- name: oAuth2\n  source: openapi/drupal-rest-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://example.com/oauth/authorize\n    tokenUrl: https://example.com/oauth/token\n  description: OAuth 2.0 authentication via the Simple OAuth module.\nscopes:\n- scope: content\n  description: Access and manage content entities\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/drupal-jsonapi-openapi.yml\n  - openapi/drupal-rest-api-openapi.yml\n- scope: user\n  description: Access and manage user entities\n  flows:\n  - authorizationCode\n  sources:\n  -\
  \ openapi/drupal-jsonapi-openapi.yml\n  - openapi/drupal-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drupal/refs/heads/main/scopes/drupal-scopes.yml
summary_line: 2 scopes · authorizationCode
tags: []
token_urls:
- https://example.com/oauth/token
---
