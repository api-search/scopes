---
api_specs:
- filename: sterling-check-openapi.yml
  format: yaml
  label: Sterling Screenings API
  slug: sterling-check-screenings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sterling-check/refs/heads/main/openapi/sterling-check-openapi.yml
- filename: sterling-check-openapi.yml
  format: yaml
  label: Sterling Candidates API
  slug: sterling-check-candidates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sterling-check/refs/heads/main/openapi/sterling-check-openapi.yml
- filename: sterling-check-openapi.yml
  format: yaml
  label: Sterling Packages API
  slug: sterling-check-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sterling-check/refs/heads/main/openapi/sterling-check-openapi.yml
- filename: sterling-check-openapi.yml
  format: yaml
  label: Sterling Reports API
  slug: sterling-check-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sterling-check/refs/heads/main/openapi/sterling-check-openapi.yml
- filename: sterling-check-openapi.yml
  format: yaml
  label: Sterling Invites API
  slug: sterling-check-invites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sterling-check/refs/heads/main/openapi/sterling-check-openapi.yml
- filename: sterling-check-openapi.yml
  format: yaml
  label: Sterling Webhooks API
  slug: sterling-check-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sterling-check/refs/heads/main/openapi/sterling-check-openapi.yml
authorization_urls: []
description: ''
docs: https://sterling.readme.io/reference/authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Sterling Check Scopes
name_suffix: OAuth Scopes
note: Sterling's API uses OAuth2 client_credentials only (Base64 client_id:client_secret sent to the oauth token endpoint) and documents no scope parameter or scope list; access is governed by the Client ID/Client Secret issued per account and screening region (https://sterling.readme.io/reference/authentication).
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
  source: openapi/sterling-check-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: sterling-check-scopes
source_filename: sterling-check-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sterling-check-openapi.yml\ndocs: https://sterling.readme.io/reference/authentication\nnote: Sterling's API uses OAuth2 client_credentials only (Base64 client_id:client_secret\n  sent to the oauth token endpoint) and documents no scope parameter or scope list;\n  access is governed by the Client ID/Client Secret issued per account and screening\n  region (https://sterling.readme.io/reference/authentication).\nschemes:\n- name: oAuth2ClientCredentials\n  source: openapi/sterling-check-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.sterlingcheck.app/oauth/token\n  description: OAuth2 client credentials grant using your Client ID and Client Secret.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sterling-check/refs/heads/main/scopes/sterling-check-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Background Screening
- Identity Verification
- Background Check
- HR Tech
- Compliance
- Gated API
token_urls:
- https://auth.sterlingcheck.app/oauth/token
---
