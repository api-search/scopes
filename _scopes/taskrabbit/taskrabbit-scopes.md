---
authorization_urls: []
description: ''
docs: https://developer.taskrabbit.com/docs/getting-started
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Taskrabbit Scopes
name_suffix: OAuth Scopes
note: TaskRabbit's gated Partner API authenticates via Auth0 machine-to-machine OAuth2 client-credentials tokens issued during partner onboarding, and its documentation (https://developer.taskrabbit.com/docs/getting-started) publishes no OAuth scopes or scope-based permissions.
overview: 'TaskRabbit uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://taskrabbit.auth0.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: TaskRabbit
provider_slug: taskrabbit
schemes:
- description: Auth0 machine-to-machine (M2M) OAuth2 client-credentials grant. Credentials are issued during partner onboarding.
  flows:
  - flow: clientCredentials
    tokenUrl: https://taskrabbit.auth0.com/oauth/token
  name: oauth2
  source: openapi/taskrabbit-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: taskrabbit-scopes
source_filename: taskrabbit-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/taskrabbit-openapi.yml\ndocs: https://developer.taskrabbit.com/docs/getting-started\nnote: TaskRabbit's gated Partner API authenticates via Auth0 machine-to-machine OAuth2\n  client-credentials tokens issued during partner onboarding, and its documentation\n  (https://developer.taskrabbit.com/docs/getting-started) publishes no OAuth scopes\n  or scope-based permissions.\nschemes:\n- name: oauth2\n  source: openapi/taskrabbit-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://taskrabbit.auth0.com/oauth/token\n  description: Auth0 machine-to-machine (M2M) OAuth2 client-credentials grant. Credentials are\n    issued during partner onboarding.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taskrabbit/refs/heads/main/scopes/taskrabbit-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Gig Economy
- Handyman
- Home Services
- Marketplace
- Delivery
- Moving
- Partner API
- IKEA
token_urls:
- https://taskrabbit.auth0.com/oauth/token
---
