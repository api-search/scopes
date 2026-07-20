---
authorization_urls:
- https://cloudapi-oauth.suunto.com/oauth/authorize
description: ''
docs: https://apizone.suunto.com/how-to-start
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Liesheng Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Liesheng Group publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Liesheng Group API on a user''s behalf.


  Tokens are issued from https://cloudapi-oauth.suunto.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Liesheng Group
provider_slug: liesheng
schemes:
- flows:
  - authorizationUrl: https://cloudapi-oauth.suunto.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://cloudapi-oauth.suunto.com/oauth/token
  name: SuuntoOAuth2
  source: https://apizone.suunto.com/how-to-start
scope_count: 1
scope_names:
- workout
scopes:
- description: Access to the authorizing Suunto App user's workout data — FIT files with summary, sample and GPS-track content — and the ability to push workouts and routes back to the account.
  flows:
  - authorizationCode
  scope: workout
slug: liesheng-scopes
source_filename: liesheng-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://apizone.suunto.com/how-to-start\ndocs: https://apizone.suunto.com/how-to-start\nnotes: >-\n  Suunto does not publish a standalone scope reference page. The single scope\n  below is the one returned verbatim in the documented token response on the\n  quick-start page. Additional scopes may exist behind the partner-gated API\n  Zone; only the published value is recorded here.\nschemes:\n- name: SuuntoOAuth2\n  source: https://apizone.suunto.com/how-to-start\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://cloudapi-oauth.suunto.com/oauth/authorize\n    tokenUrl: https://cloudapi-oauth.suunto.com/oauth/token\nscopes:\n- scope: workout\n  description: >-\n    Access to the authorizing Suunto App user's workout data — FIT files with\n    summary, sample and GPS-track content — and the ability to push workouts and\n    routes back to the account.\n  flows:\n  - authorizationCode\n  sources:\n  - https://apizone.suunto.com/how-to-start\n\
  \  evidence: >-\n    Documented token response: {\"access_token\": \"<JWT_TOKEN>\", \"token_type\":\n    \"bearer\", \"refresh_token\": \"<JWT_REFRESH_TOKEN>\", \"expires_in\": 86400,\n    \"scope\": \"workout\"}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liesheng/refs/heads/main/scopes/liesheng-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Consumer Electronics
- Wearables
- Audio
- Sports
- Fitness
- Health
- Internet of Things
- ODM
- OEM
- China
token_urls:
- https://cloudapi-oauth.suunto.com/oauth/token
---
