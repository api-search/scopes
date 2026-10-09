---
api_specs:
- filename: prove-auth-api-openapi.yml
  format: yaml
  label: Prove Auth API
  slug: prove-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prove/refs/heads/main/openapi/prove-auth-api-openapi.yml
- filename: prove-authentication-api-openapi.yml
  format: yaml
  label: Prove Authentication API
  slug: prove-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prove/refs/heads/main/openapi/prove-authentication-api-openapi.yml
- filename: prove-domain-api-openapi.yml
  format: yaml
  label: Prove Domain API
  slug: prove-domain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prove/refs/heads/main/openapi/prove-domain-api-openapi.yml
- filename: prove-identity-api-openapi.yml
  format: yaml
  label: Prove Identity API
  slug: prove-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prove/refs/heads/main/openapi/prove-identity-api-openapi.yml
- filename: prove-identity-verification-api-openapi.yml
  format: yaml
  label: Prove Identity Verification API
  slug: prove-identity-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prove/refs/heads/main/openapi/prove-identity-verification-api-openapi.yml
- filename: prove-pre-fill-api-openapi.yml
  format: yaml
  label: Prove Pre-Fill API
  slug: prove-pre-fill-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prove/refs/heads/main/openapi/prove-pre-fill-api-openapi.yml
- filename: prove-trust-score-api-openapi.yml
  format: yaml
  label: Prove Trust Score API
  slug: prove-trust-score-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prove/refs/heads/main/openapi/prove-trust-score-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Prove Scopes
name_suffix: OAuth Scopes
note: The contract declares an oauth2 clientCredentials flow with an empty scopes map and a bearerAuth scheme; no scopes or permissions reference is readable (developer.prove.com/tutorial/access-api-keys redirects to /login). Access is scoped per Portal project credential, not per OAuth scope.
overview: 'Prove uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.prove.com/v3/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Prove
provider_slug: prove
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.prove.com/v3/token
  name: oauth2
  source: openapi/prove-auth-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.prove.com/v3/token
  name: oauth2
  source: openapi/prove-authentication-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.prove.com/v3/token
  name: oauth2
  source: openapi/prove-domain-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.prove.com/v3/token
  name: oauth2
  source: openapi/prove-identity-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.prove.com/v3/token
  name: oauth2
  source: openapi/prove-identity-verification-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.prove.com/v3/token
  name: oauth2
  source: openapi/prove-pre-fill-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.prove.com/v3/token
  name: oauth2
  source: openapi/prove-trust-score-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: prove-scopes
source_filename: prove-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: none\nsource: openapi/prove-auth-api-openapi.yml, openapi/prove-authentication-api-openapi.yml, openapi/prove-domain-api-openapi.yml,\n  openapi/prove-identity-api-openapi.yml, openapi/prove-identity-verification-api-openapi.yml, openapi/prove-pre-fill-api-openapi.yml,\n  openapi/prove-trust-score-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/prove-auth-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.prove.com/v3/token\n- name: oauth2\n  source: openapi/prove-authentication-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.prove.com/v3/token\n- name: oauth2\n  source: openapi/prove-domain-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.prove.com/v3/token\n- name: oauth2\n  source: openapi/prove-identity-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.prove.com/v3/token\n- name: oauth2\n  source:\
  \ openapi/prove-identity-verification-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.prove.com/v3/token\n- name: oauth2\n  source: openapi/prove-pre-fill-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.prove.com/v3/token\n- name: oauth2\n  source: openapi/prove-trust-score-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.prove.com/v3/token\nscopes: []\nnote: The contract declares an oauth2 clientCredentials flow with an empty scopes map and a bearerAuth scheme; no\n  scopes or permissions reference is readable (developer.prove.com/tutorial/access-api-keys redirects to /login).\n  Access is scoped per Portal project credential, not per OAuth scope.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prove/refs/heads/main/scopes/prove-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Identity Verification
- Authentication
- Phone Intelligence
- KYC
- Fraud Prevention
token_bound: false
token_urls:
- https://api.prove.com/v3/token
---
