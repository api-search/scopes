---
api_specs:
- filename: accurate-bg-adjudication-api-openapi.yml
  format: yaml
  label: Accurate Background Adjudication API
  slug: accurate-bg-adjudication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accurate-bg/refs/heads/main/openapi/accurate-bg-adjudication-api-openapi.yml
- filename: accurate-bg-candidates-api-openapi.yml
  format: yaml
  label: Accurate Background Candidates API
  slug: accurate-bg-candidates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accurate-bg/refs/heads/main/openapi/accurate-bg-candidates-api-openapi.yml
- filename: accurate-bg-documents-api-openapi.yml
  format: yaml
  label: Accurate Background Documents API
  slug: accurate-bg-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accurate-bg/refs/heads/main/openapi/accurate-bg-documents-api-openapi.yml
- filename: accurate-bg-notifications-api-openapi.yml
  format: yaml
  label: Accurate Background Notifications API
  slug: accurate-bg-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accurate-bg/refs/heads/main/openapi/accurate-bg-notifications-api-openapi.yml
- filename: accurate-bg-orders-api-openapi.yml
  format: yaml
  label: Accurate Background Orders API
  slug: accurate-bg-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accurate-bg/refs/heads/main/openapi/accurate-bg-orders-api-openapi.yml
- filename: accurate-bg-packages-api-openapi.yml
  format: yaml
  label: Accurate Background Packages API
  slug: accurate-bg-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accurate-bg/refs/heads/main/openapi/accurate-bg-packages-api-openapi.yml
- filename: accurate-bg-reports-api-openapi.yml
  format: yaml
  label: Accurate Background Reports API
  slug: accurate-bg-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accurate-bg/refs/heads/main/openapi/accurate-bg-reports-api-openapi.yml
- filename: accurate-bg-utility-api-openapi.yml
  format: yaml
  label: Accurate Background Utility API
  slug: accurate-bg-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accurate-bg/refs/heads/main/openapi/accurate-bg-utility-api-openapi.yml
- filename: accurate-bg-verifications-api-openapi.yml
  format: yaml
  label: Accurate Background Verifications API
  slug: accurate-bg-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accurate-bg/refs/heads/main/openapi/accurate-bg-verifications-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Accurate Bg Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Accurate Background uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.accuratebackground.com/v3/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Accurate Background
provider_slug: accurate-bg
schemes:
- description: Accurate API credentials are a ClientID / ClientSecret pair obtained from the Accurate developer portal. Credentials are exchanged (HTTP Basic) for an access token that authorizes subsequent requests.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.accuratebackground.com/v3/oauth/token
  name: oauth2ClientCredentials
  source: openapi/accurate-bg-adjudication-api-openapi.yml
- description: Accurate API credentials are a ClientID / ClientSecret pair obtained from the Accurate developer portal. Credentials are exchanged (HTTP Basic) for an access token that authorizes subsequent requests.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.accuratebackground.com/v3/oauth/token
  name: oauth2ClientCredentials
  source: openapi/accurate-bg-candidates-api-openapi.yml
- description: Accurate API credentials are a ClientID / ClientSecret pair obtained from the Accurate developer portal. Credentials are exchanged (HTTP Basic) for an access token that authorizes subsequent requests.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.accuratebackground.com/v3/oauth/token
  name: oauth2ClientCredentials
  source: openapi/accurate-bg-documents-api-openapi.yml
- description: Accurate API credentials are a ClientID / ClientSecret pair obtained from the Accurate developer portal. Credentials are exchanged (HTTP Basic) for an access token that authorizes subsequent requests.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.accuratebackground.com/v3/oauth/token
  name: oauth2ClientCredentials
  source: openapi/accurate-bg-notifications-api-openapi.yml
- description: Accurate API credentials are a ClientID / ClientSecret pair obtained from the Accurate developer portal. Credentials are exchanged (HTTP Basic) for an access token that authorizes subsequent requests.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.accuratebackground.com/v3/oauth/token
  name: oauth2ClientCredentials
  source: openapi/accurate-bg-orders-api-openapi.yml
- description: Accurate API credentials are a ClientID / ClientSecret pair obtained from the Accurate developer portal. Credentials are exchanged (HTTP Basic) for an access token that authorizes subsequent requests.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.accuratebackground.com/v3/oauth/token
  name: oauth2ClientCredentials
  source: openapi/accurate-bg-packages-api-openapi.yml
- description: Accurate API credentials are a ClientID / ClientSecret pair obtained from the Accurate developer portal. Credentials are exchanged (HTTP Basic) for an access token that authorizes subsequent requests.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.accuratebackground.com/v3/oauth/token
  name: oauth2ClientCredentials
  source: openapi/accurate-bg-reports-api-openapi.yml
- description: Accurate API credentials are a ClientID / ClientSecret pair obtained from the Accurate developer portal. Credentials are exchanged (HTTP Basic) for an access token that authorizes subsequent requests.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.accuratebackground.com/v3/oauth/token
  name: oauth2ClientCredentials
  source: openapi/accurate-bg-utility-api-openapi.yml
- description: Accurate API credentials are a ClientID / ClientSecret pair obtained from the Accurate developer portal. Credentials are exchanged (HTTP Basic) for an access token that authorizes subsequent requests.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.accuratebackground.com/v3/oauth/token
  name: oauth2ClientCredentials
  source: openapi/accurate-bg-verifications-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: accurate-bg-scopes
source_filename: accurate-bg-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/accurate-bg-adjudication-api-openapi.yml, openapi/accurate-bg-candidates-api-openapi.yml,\n  openapi/accurate-bg-documents-api-openapi.yml, openapi/accurate-bg-notifications-api-openapi.yml,\n  openapi/accurate-bg-orders-api-openapi.yml, openapi/accurate-bg-packages-api-openapi.yml,\n  openapi/accurate-bg-reports-api-openapi.yml, openapi/accurate-bg-utility-api-openapi.yml,\n  openapi/accurate-bg-verifications-api-openapi.yml\nschemes:\n- name: oauth2ClientCredentials\n  source: openapi/accurate-bg-adjudication-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.accuratebackground.com/v3/oauth/token\n  description: Accurate API credentials are a ClientID / ClientSecret pair obtained from the\n    Accurate developer portal. Credentials are exchanged (HTTP Basic) for an access token that\n    authorizes subsequent requests.\n- name: oauth2ClientCredentials\n  source: openapi/accurate-bg-candidates-api-openapi.yml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.accuratebackground.com/v3/oauth/token\n  description: Accurate API credentials are a ClientID / ClientSecret pair obtained from the\n    Accurate developer portal. Credentials are exchanged (HTTP Basic) for an access token that\n    authorizes subsequent requests.\n- name: oauth2ClientCredentials\n  source: openapi/accurate-bg-documents-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.accuratebackground.com/v3/oauth/token\n  description: Accurate API credentials are a ClientID / ClientSecret pair obtained from the\n    Accurate developer portal. Credentials are exchanged (HTTP Basic) for an access token that\n    authorizes subsequent requests.\n- name: oauth2ClientCredentials\n  source: openapi/accurate-bg-notifications-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.accuratebackground.com/v3/oauth/token\n  description: Accurate API credentials are a ClientID\
  \ / ClientSecret pair obtained from the\n    Accurate developer portal. Credentials are exchanged (HTTP Basic) for an access token that\n    authorizes subsequent requests.\n- name: oauth2ClientCredentials\n  source: openapi/accurate-bg-orders-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.accuratebackground.com/v3/oauth/token\n  description: Accurate API credentials are a ClientID / ClientSecret pair obtained from the\n    Accurate developer portal. Credentials are exchanged (HTTP Basic) for an access token that\n    authorizes subsequent requests.\n- name: oauth2ClientCredentials\n  source: openapi/accurate-bg-packages-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.accuratebackground.com/v3/oauth/token\n  description: Accurate API credentials are a ClientID / ClientSecret pair obtained from the\n    Accurate developer portal. Credentials are exchanged (HTTP Basic) for an access token that\n    authorizes subsequent\
  \ requests.\n- name: oauth2ClientCredentials\n  source: openapi/accurate-bg-reports-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.accuratebackground.com/v3/oauth/token\n  description: Accurate API credentials are a ClientID / ClientSecret pair obtained from the\n    Accurate developer portal. Credentials are exchanged (HTTP Basic) for an access token that\n    authorizes subsequent requests.\n- name: oauth2ClientCredentials\n  source: openapi/accurate-bg-utility-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.accuratebackground.com/v3/oauth/token\n  description: Accurate API credentials are a ClientID / ClientSecret pair obtained from the\n    Accurate developer portal. Credentials are exchanged (HTTP Basic) for an access token that\n    authorizes subsequent requests.\n- name: oauth2ClientCredentials\n  source: openapi/accurate-bg-verifications-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.accuratebackground.com/v3/oauth/token\n\
  \  description: Accurate API credentials are a ClientID / ClientSecret pair obtained from the\n    Accurate developer portal. Credentials are exchanged (HTTP Basic) for an access token that\n    authorizes subsequent requests.\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accurate-bg/refs/heads/main/scopes/accurate-bg-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Background Checks
- Employment Screening
- Identity Verification
- Compliance
- Human Resources
- Screening
token_bound: false
token_urls:
- https://api.accuratebackground.com/v3/oauth/token
---
