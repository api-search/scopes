---
api_specs:
- filename: sterling-check-authentication-api-openapi.yml
  format: yaml
  label: Sterling Authentication API
  slug: sterling-check-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sterling-check/refs/heads/main/openapi/sterling-check-authentication-api-openapi.yml
- filename: sterling-check-candidates-api-openapi.yml
  format: yaml
  label: Sterling Candidates API
  slug: sterling-check-candidates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sterling-check/refs/heads/main/openapi/sterling-check-candidates-api-openapi.yml
- filename: sterling-check-invites-api-openapi.yml
  format: yaml
  label: Sterling Invites API
  slug: sterling-check-invites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sterling-check/refs/heads/main/openapi/sterling-check-invites-api-openapi.yml
- filename: sterling-check-packages-api-openapi.yml
  format: yaml
  label: Sterling Packages API
  slug: sterling-check-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sterling-check/refs/heads/main/openapi/sterling-check-packages-api-openapi.yml
- filename: sterling-check-reports-api-openapi.yml
  format: yaml
  label: Sterling Reports API
  slug: sterling-check-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sterling-check/refs/heads/main/openapi/sterling-check-reports-api-openapi.yml
- filename: sterling-check-screenings-api-openapi.yml
  format: yaml
  label: Sterling Screenings API
  slug: sterling-check-screenings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sterling-check/refs/heads/main/openapi/sterling-check-screenings-api-openapi.yml
- filename: sterling-check-webhooks-api-openapi.yml
  format: yaml
  label: Sterling Webhooks API
  slug: sterling-check-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sterling-check/refs/heads/main/openapi/sterling-check-webhooks-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Sterling Check Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Sterling uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://auth.sterlingcheck.app/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Sterling
provider_slug: sterling-check
schemes:
- description: OAuth2 client credentials grant using your Client ID and Client Secret.
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.sterlingcheck.app/oauth/token
  name: oAuth2ClientCredentials
  source: openapi/sterling-check-authentication-api-openapi.yml
- description: OAuth2 client credentials grant using your Client ID and Client Secret.
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.sterlingcheck.app/oauth/token
  name: oAuth2ClientCredentials
  source: openapi/sterling-check-candidates-api-openapi.yml
- description: OAuth2 client credentials grant using your Client ID and Client Secret.
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.sterlingcheck.app/oauth/token
  name: oAuth2ClientCredentials
  source: openapi/sterling-check-invites-api-openapi.yml
- description: OAuth2 client credentials grant using your Client ID and Client Secret.
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.sterlingcheck.app/oauth/token
  name: oAuth2ClientCredentials
  source: openapi/sterling-check-packages-api-openapi.yml
- description: OAuth2 client credentials grant using your Client ID and Client Secret.
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.sterlingcheck.app/oauth/token
  name: oAuth2ClientCredentials
  source: openapi/sterling-check-reports-api-openapi.yml
- description: OAuth2 client credentials grant using your Client ID and Client Secret.
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.sterlingcheck.app/oauth/token
  name: oAuth2ClientCredentials
  source: openapi/sterling-check-screenings-api-openapi.yml
- description: OAuth2 client credentials grant using your Client ID and Client Secret.
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.sterlingcheck.app/oauth/token
  name: oAuth2ClientCredentials
  source: openapi/sterling-check-webhooks-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: sterling-check-scopes
source_filename: sterling-check-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/sterling-check-authentication-api-openapi.yml, openapi/sterling-check-candidates-api-openapi.yml,\n  openapi/sterling-check-invites-api-openapi.yml, openapi/sterling-check-packages-api-openapi.yml,\n  openapi/sterling-check-reports-api-openapi.yml, openapi/sterling-check-screenings-api-openapi.yml,\n  openapi/sterling-check-webhooks-api-openapi.yml\nschemes:\n- name: oAuth2ClientCredentials\n  source: openapi/sterling-check-authentication-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.sterlingcheck.app/oauth/token\n  description: OAuth2 client credentials grant using your Client ID and Client Secret.\n- name: oAuth2ClientCredentials\n  source: openapi/sterling-check-candidates-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.sterlingcheck.app/oauth/token\n  description: OAuth2 client credentials grant using your Client ID and Client Secret.\n- name: oAuth2ClientCredentials\n\
  \  source: openapi/sterling-check-invites-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.sterlingcheck.app/oauth/token\n  description: OAuth2 client credentials grant using your Client ID and Client Secret.\n- name: oAuth2ClientCredentials\n  source: openapi/sterling-check-packages-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.sterlingcheck.app/oauth/token\n  description: OAuth2 client credentials grant using your Client ID and Client Secret.\n- name: oAuth2ClientCredentials\n  source: openapi/sterling-check-reports-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.sterlingcheck.app/oauth/token\n  description: OAuth2 client credentials grant using your Client ID and Client Secret.\n- name: oAuth2ClientCredentials\n  source: openapi/sterling-check-screenings-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.sterlingcheck.app/oauth/token\n  description:\
  \ OAuth2 client credentials grant using your Client ID and Client Secret.\n- name: oAuth2ClientCredentials\n  source: openapi/sterling-check-webhooks-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.sterlingcheck.app/oauth/token\n  description: OAuth2 client credentials grant using your Client ID and Client Secret.\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sterling-check/refs/heads/main/scopes/sterling-check-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Background Screening
- Identity Verification
- Background Checks
- Human Resources
- Compliance
- Gated API
token_bound: false
token_urls:
- https://auth.sterlingcheck.app/oauth/token
---
