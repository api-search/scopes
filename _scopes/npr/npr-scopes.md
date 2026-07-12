---
authorization_urls:
- https://authorization.api.npr.org/v2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Npr Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'NPR publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the NPR API on a user''s behalf.


  Tokens are issued from https://authorization.api.npr.org/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: NPR
provider_slug: npr
schemes:
- flows:
  - authorizationUrl: https://authorization.api.npr.org/v2/authorize
    flow: authorizationCode
    tokenUrl: https://authorization.api.npr.org/v2/token
  name: oauth2
  source: openapi/npr-authorization-openapi-original.yml
- flows:
  - authorizationUrl: https://authorization.api.npr.org/v2/authorize
    flow: authorizationCode
    tokenUrl: https://authorization.api.npr.org/v2/token
  name: oauth2
  source: openapi/npr-identity-openapi-original.yml
- flows:
  - authorizationUrl: https://authorization.api.npr.org/v2/authorize
    flow: authorizationCode
    tokenUrl: https://authorization.api.npr.org/v2/token
  name: oauth2
  source: openapi/npr-station-finder-openapi-original.yml
scope_count: 5
scope_names:
- identity.readonly
- identity.write
- listening.readonly
- listening.write
- localactivation
scopes:
- description: See your personal information, such as your first name, last name, and favorite station.
  flows:
  - authorizationCode
  scope: identity.readonly
- description: Update your personal information, such as your favorite station(s) or program(s) you follow, on your behalf.
  flows:
  - authorizationCode
  scope: identity.write
- description: See your NPR One listening history and get audio recommendations.
  flows:
  - authorizationCode
  scope: listening.readonly
- description: Record that you have heard, marked as interesting, and/or skipped NPR One stories in order to personalize future audio recommendations.
  flows:
  - authorizationCode
  scope: listening.write
- description: Connect you with your local NPR member station for communication purposes.
  flows:
  - authorizationCode
  scope: localactivation
slug: npr-scopes
source_filename: npr-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/npr-authorization-openapi-original.yml, openapi/npr-identity-openapi-original.yml,\n  openapi/npr-station-finder-openapi-original.yml\nschemes:\n- name: oauth2\n  source: openapi/npr-authorization-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authorization.api.npr.org/v2/authorize\n    tokenUrl: https://authorization.api.npr.org/v2/token\n- name: oauth2\n  source: openapi/npr-identity-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authorization.api.npr.org/v2/authorize\n    tokenUrl: https://authorization.api.npr.org/v2/token\n- name: oauth2\n  source: openapi/npr-station-finder-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authorization.api.npr.org/v2/authorize\n    tokenUrl: https://authorization.api.npr.org/v2/token\nscopes:\n- scope: identity.readonly\n  description: See your personal\
  \ information, such as your first name, last name, and favorite\n    station.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/npr-authorization-openapi-original.yml\n  - openapi/npr-identity-openapi-original.yml\n  - openapi/npr-station-finder-openapi-original.yml\n- scope: identity.write\n  description: Update your personal information, such as your favorite station(s) or program(s)\n    you follow, on your behalf.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/npr-authorization-openapi-original.yml\n  - openapi/npr-identity-openapi-original.yml\n  - openapi/npr-station-finder-openapi-original.yml\n- scope: listening.readonly\n  description: See your NPR One listening history and get audio recommendations.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/npr-authorization-openapi-original.yml\n  - openapi/npr-identity-openapi-original.yml\n  - openapi/npr-station-finder-openapi-original.yml\n- scope: listening.write\n  description: Record that you have heard,\
  \ marked as interesting, and/or skipped NPR One stories\n    in order to personalize future audio recommendations.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/npr-authorization-openapi-original.yml\n  - openapi/npr-identity-openapi-original.yml\n  - openapi/npr-station-finder-openapi-original.yml\n- scope: localactivation\n  description: Connect you with your local NPR member station for communication purposes.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/npr-authorization-openapi-original.yml\n  - openapi/npr-identity-openapi-original.yml\n  - openapi/npr-station-finder-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/npr/refs/heads/main/scopes/npr-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Media
- News
- Radio
token_urls:
- https://authorization.api.npr.org/v2/token
---
