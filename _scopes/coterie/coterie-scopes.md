---
authorization_urls: []
description: ''
docs: https://docs.coterieinsurance.com/#authentication-guide
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Coterie Scopes
name_suffix: OAuth Scopes
note: Coterie does not document OAuth scopes; access is controlled by partner-issued Publishable and Secret API keys passed as a token in the Authorization header, with certain operations requiring the Secret key (https://docs.coterieinsurance.com/#authentication-guide).
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
  source: openapi/coterie-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: coterie-scopes
source_filename: coterie-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/coterie-openapi.yml\ndocs: https://docs.coterieinsurance.com/#authentication-guide\nnote: Coterie does not document OAuth scopes; access is controlled by partner-issued\n  Publishable and Secret API keys passed as a token in the Authorization header,\n  with certain operations requiring the Secret key\n  (https://docs.coterieinsurance.com/#authentication-guide).\nschemes:\n- name: oauth2\n  source: openapi/coterie-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.coterieinsurance.com/v1/oauth/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coterie/refs/heads/main/scopes/coterie-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Insurance
- Commercial Insurance
- Small Business
- Embedded Insurance
- Insurtech
token_urls:
- https://api.coterieinsurance.com/v1/oauth/token
---
