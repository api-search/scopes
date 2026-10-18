---
api_specs:
- filename: coterie-applications-api-openapi.yml
  format: yaml
  label: Coterie Insurance Applications API
  slug: coterie-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coterie/refs/heads/main/openapi/coterie-applications-api-openapi.yml
- filename: coterie-documents-api-openapi.yml
  format: yaml
  label: Coterie Insurance Documents API
  slug: coterie-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coterie/refs/heads/main/openapi/coterie-documents-api-openapi.yml
- filename: coterie-industry-api-openapi.yml
  format: yaml
  label: Coterie Insurance Industry API
  slug: coterie-industry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coterie/refs/heads/main/openapi/coterie-industry-api-openapi.yml
- filename: coterie-policies-api-openapi.yml
  format: yaml
  label: Coterie Insurance Policies API
  slug: coterie-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coterie/refs/heads/main/openapi/coterie-policies-api-openapi.yml
- filename: coterie-quotes-api-openapi.yml
  format: yaml
  label: Coterie Insurance Quotes API
  slug: coterie-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coterie/refs/heads/main/openapi/coterie-quotes-api-openapi.yml
- filename: coterie-webhooks-api-openapi.yml
  format: yaml
  label: Coterie Insurance Webhooks API
  slug: coterie-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coterie/refs/heads/main/openapi/coterie-webhooks-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Coterie Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Coterie Insurance uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.coterieinsurance.com/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Coterie Insurance
provider_slug: coterie
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.coterieinsurance.com/v1/oauth/token
  name: oauth2
  source: openapi/coterie-applications-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.coterieinsurance.com/v1/oauth/token
  name: oauth2
  source: openapi/coterie-documents-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.coterieinsurance.com/v1/oauth/token
  name: oauth2
  source: openapi/coterie-industry-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.coterieinsurance.com/v1/oauth/token
  name: oauth2
  source: openapi/coterie-policies-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.coterieinsurance.com/v1/oauth/token
  name: oauth2
  source: openapi/coterie-quotes-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.coterieinsurance.com/v1/oauth/token
  name: oauth2
  source: openapi/coterie-webhooks-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: coterie-scopes
source_filename: coterie-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/coterie-applications-api-openapi.yml, openapi/coterie-documents-api-openapi.yml,\n  openapi/coterie-industry-api-openapi.yml, openapi/coterie-policies-api-openapi.yml, openapi/coterie-quotes-api-openapi.yml,\n  openapi/coterie-webhooks-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/coterie-applications-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.coterieinsurance.com/v1/oauth/token\n- name: oauth2\n  source: openapi/coterie-documents-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.coterieinsurance.com/v1/oauth/token\n- name: oauth2\n  source: openapi/coterie-industry-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.coterieinsurance.com/v1/oauth/token\n- name: oauth2\n  source: openapi/coterie-policies-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.coterieinsurance.com/v1/oauth/token\n\
  - name: oauth2\n  source: openapi/coterie-quotes-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.coterieinsurance.com/v1/oauth/token\n- name: oauth2\n  source: openapi/coterie-webhooks-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.coterieinsurance.com/v1/oauth/token\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coterie/refs/heads/main/scopes/coterie-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Insurance
- Commercial Insurance
- Small Business
- Embedded Insurance
- Insurtech
token_bound: false
token_urls:
- https://api.coterieinsurance.com/v1/oauth/token
---
