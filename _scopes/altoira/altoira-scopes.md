---
api_specs:
- filename: altoira-handoffs-api-openapi.yml
  format: yaml
  label: AltoIRA Handoffs API
  slug: altoira-handoffs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altoira/refs/heads/main/openapi/altoira-handoffs-api-openapi.yml
- filename: altoira-investment-api-openapi.yml
  format: yaml
  label: AltoIRA Investment API
  slug: altoira-investment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altoira/refs/heads/main/openapi/altoira-investment-api-openapi.yml
- filename: altoira-offering-api-openapi.yml
  format: yaml
  label: AltoIRA Offering API
  slug: altoira-offering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altoira/refs/heads/main/openapi/altoira-offering-api-openapi.yml
- filename: altoira-user-api-openapi.yml
  format: yaml
  label: AltoIRA User API
  slug: altoira-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altoira/refs/heads/main/openapi/altoira-user-api-openapi.yml
- filename: altoira-oauth-api-openapi.yml
  format: yaml
  label: AltoIRA OAUTH API
  slug: altoira-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altoira/refs/heads/main/openapi/altoira-oauth-api-openapi.yml
authorization_urls:
- https://altoira.sandbox.altoira.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: none
name: Altoira Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'AltoIRA uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://altoira.sandbox.altoira.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AltoIRA
provider_slug: altoira
schemes:
- description: Redirect your users to /oauth/authorize to get started (see the OAuth section on this documentation)
  flows:
  - authorizationUrl: https://altoira.sandbox.altoira.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://altoira.sandbox.altoira.com/oauth/token
  name: UserOauth
  source: openapi/altoira-handoffs-api-openapi.yml
- description: Redirect your users to /oauth/authorize to get started (see the OAuth section on this documentation)
  flows:
  - authorizationUrl: https://altoira.sandbox.altoira.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://altoira.sandbox.altoira.com/oauth/token
  name: UserOauth
  source: openapi/altoira-investment-api-openapi.yml
- description: Redirect your users to /oauth/authorize to get started (see the OAuth section on this documentation)
  flows:
  - authorizationUrl: https://altoira.sandbox.altoira.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://altoira.sandbox.altoira.com/oauth/token
  name: UserOauth
  source: openapi/altoira-oauth-api-openapi.yml
- description: Redirect your users to /oauth/authorize to get started (see the OAuth section on this documentation)
  flows:
  - authorizationUrl: https://altoira.sandbox.altoira.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://altoira.sandbox.altoira.com/oauth/token
  name: UserOauth
  source: openapi/altoira-offering-api-openapi.yml
- description: Redirect your users to /oauth/authorize to get started (see the OAuth section on this documentation)
  flows:
  - authorizationUrl: https://altoira.sandbox.altoira.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://altoira.sandbox.altoira.com/oauth/token
  name: UserOauth
  source: openapi/altoira-user-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: altoira-scopes
source_filename: altoira-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/altoira-handoffs-api-openapi.yml, openapi/altoira-investment-api-openapi.yml,\n  openapi/altoira-oauth-api-openapi.yml, openapi/altoira-offering-api-openapi.yml, openapi/altoira-user-api-openapi.yml\nschemes:\n- name: UserOauth\n  source: openapi/altoira-handoffs-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://altoira.sandbox.altoira.com/oauth/authorize\n    tokenUrl: https://altoira.sandbox.altoira.com/oauth/token\n  description: Redirect your users to /oauth/authorize to get started (see the OAuth section\n    on this documentation)\n- name: UserOauth\n  source: openapi/altoira-investment-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://altoira.sandbox.altoira.com/oauth/authorize\n    tokenUrl: https://altoira.sandbox.altoira.com/oauth/token\n  description: Redirect your users to /oauth/authorize to get started (see the OAuth section\n    on this\
  \ documentation)\n- name: UserOauth\n  source: openapi/altoira-oauth-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://altoira.sandbox.altoira.com/oauth/authorize\n    tokenUrl: https://altoira.sandbox.altoira.com/oauth/token\n  description: Redirect your users to /oauth/authorize to get started (see the OAuth section\n    on this documentation)\n- name: UserOauth\n  source: openapi/altoira-offering-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://altoira.sandbox.altoira.com/oauth/authorize\n    tokenUrl: https://altoira.sandbox.altoira.com/oauth/token\n  description: Redirect your users to /oauth/authorize to get started (see the OAuth section\n    on this documentation)\n- name: UserOauth\n  source: openapi/altoira-user-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://altoira.sandbox.altoira.com/oauth/authorize\n    tokenUrl: https://altoira.sandbox.altoira.com/oauth/token\n\
  \  description: Redirect your users to /oauth/authorize to get started (see the OAuth section\n    on this documentation)\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/altoira/refs/heads/main/scopes/altoira-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Financial Services
- Retirement
- Self-Directed IRA
- Alternative Investments
- Private Markets
- Fintech
- Custody
- Cryptocurrency
- Wealth Management
- Investing
- Capital Raising
token_bound: false
token_urls:
- https://altoira.sandbox.altoira.com/oauth/token
---
