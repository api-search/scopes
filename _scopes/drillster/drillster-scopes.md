---
authorization_urls:
- https://www.drillster.com/daas/oauth/authorize
description: ''
docs: https://www.drillster.com/info/developers/rest-apis/oauth/
flows:
- authorizationCode
- urn:ietf:params:oauth:grant-type:jwt-bearer
kind: oauth-scopes
layout: scope
method: searched
name: Drillster Scopes
name_suffix: OAuth Scopes
note: 'Drillster publishes no OpenAPI and no scope reference page. The only scope value the documentation ever shows in a real token response is ROLE_USER, which appears in both the authorization-code and JWT-bearer examples and in the decoded access-token payload. There is no documented scope parameter on the authorize or token requests: authorization is not carried by OAuth scopes at all but by the Drillster PERMISSION model attached to the account (and, for service accounts, by group access grants). Recorded honestly rather than padded — the permission surface below is documented, the scope surface is effectively one value.'
overview: 'Drillster publishes 1 OAuth 2.0 scope via the authorizationCode and urn:ietf:params:oauth:grant-type:jwt-bearer flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Drillster API on a user''s behalf.


  Tokens are issued from https://www.drillster.com/daas/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Drillster
provider_slug: drillster
schemes:
- flows:
  - authorizationUrl: https://www.drillster.com/daas/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://www.drillster.com/daas/oauth/token
  - flow: urn:ietf:params:oauth:grant-type:jwt-bearer
    tokenUrl: https://www.drillster.com/daas/oauth/token
  name: OAuth2
  source: https://www.drillster.com/.well-known/oauth-authorization-server
scope_count: 1
scope_names:
- ROLE_USER
scopes:
- description: The single scope observed in Drillster access tokens. Grants the token the authority of the Drillster account it was issued for; what that account may actually do is decided by the account's permissions and group access, not by the scope string.
  flows:
  - authorizationCode
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  scope: ROLE_USER
slug: drillster-scopes
source_filename: drillster-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: https://www.drillster.com/info/developers/rest-apis/oauth/authorization-code-grant/\ndocs: https://www.drillster.com/info/developers/rest-apis/oauth/\nnote: >-\n  Drillster publishes no OpenAPI and no scope reference page. The only scope value the\n  documentation ever shows in a real token response is ROLE_USER, which appears in both the\n  authorization-code and JWT-bearer examples and in the decoded access-token payload. There\n  is no documented scope parameter on the authorize or token requests: authorization is not\n  carried by OAuth scopes at all but by the Drillster PERMISSION model attached to the\n  account (and, for service accounts, by group access grants). Recorded honestly rather than\n  padded — the permission surface below is documented, the scope surface is effectively one value.\nschemes:\n  - name: OAuth2\n    source: https://www.drillster.com/.well-known/oauth-authorization-server\n    flows:\n      - flow:\
  \ authorizationCode\n        authorizationUrl: https://www.drillster.com/daas/oauth/authorize\n        tokenUrl: https://www.drillster.com/daas/oauth/token\n      - flow: 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n        tokenUrl: https://www.drillster.com/daas/oauth/token\nscopes:\n  - scope: ROLE_USER\n    description: >-\n      The single scope observed in Drillster access tokens. Grants the token the authority of\n      the Drillster account it was issued for; what that account may actually do is decided by\n      the account's permissions and group access, not by the scope string.\n    flows: [authorizationCode, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n    sources:\n      - https://www.drillster.com/info/developers/rest-apis/oauth/authorization-code-grant/\n      - https://www.drillster.com/info/developers/rest-apis/oauth/jwt-authorization-grant/\nauthorization_model:\n  kind: account permissions + group access (not OAuth scopes)\n  docs: https://www.drillster.com/info/developers/rest-apis/service-accounts/\n\
  \  documented_permissions:\n    - name: Manage service accounts\n      note: required to create service accounts for an organization\n    - name: PUBLISH_TO_CATALOG\n      note: surfaced as the not_authorized error on POST /catalogs\n    - name: Groups administrator\n      note: makes an account manager or viewer of every group in the organization\n  group_permission_filter_values: [VIEW, MANAGE]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drillster/refs/heads/main/scopes/drillster-scopes.yml
summary_line: 1 scope · authorizationCode/urn:ietf:params:oauth:grant-type:jwt-bearer
tags:
- Assessments
- Education
- Learning
- Quizzes
- Training
- LMS
- Adaptive Learning
- Compliance Training
- Webhooks
token_urls:
- https://www.drillster.com/daas/oauth/token
---
