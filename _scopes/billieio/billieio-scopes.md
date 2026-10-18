---
api_specs:
- filename: billieio-authentication-api-openapi.yml
  format: yaml
  label: Billieio Authentication API
  slug: billieio-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billieio/refs/heads/main/openapi/billieio-authentication-api-openapi.yml
- filename: billieio-back-end-order-creation-api-openapi.yml
  format: yaml
  label: Billieio Back-end Order Creation API
  slug: billieio-back-end-order-creation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billieio/refs/heads/main/openapi/billieio-back-end-order-creation-api-openapi.yml
- filename: billieio-captures-api-openapi.yml
  format: yaml
  label: Billieio Captures API
  slug: billieio-captures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billieio/refs/heads/main/openapi/billieio-captures-api-openapi.yml
- filename: billieio-front-end-order-creation-api-openapi.yml
  format: yaml
  label: Billieio Front-end Order Creation API
  slug: billieio-front-end-order-creation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billieio/refs/heads/main/openapi/billieio-front-end-order-creation-api-openapi.yml
- filename: billieio-order-management-api-openapi.yml
  format: yaml
  label: Billieio Order Management API
  slug: billieio-order-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billieio/refs/heads/main/openapi/billieio-order-management-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- password
kind: oauth-scopes
layout: scope
method: derived
name: Billieio Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Billieio publishes 1 OAuth 2.0 scope via the password flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Billieio API on a user''s behalf.


  Tokens are issued from /oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Billieio
provider_slug: billieio
schemes:
- description: 'This authentication mechanism is based on the OAuth 2.0 prototocol and requires a Client ID, a Client Secret Key and

    in some cases also a user and password.


    With these credentials, the client should request a token using the `POST /api/v1/oauth/token` endpoint,

    which should be used in the `Authorization` header together with the `Bearer` challenge to authenticate all the requests.


    > Example: `Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiIxMjM0NTY3ODkwIiwibmFtZSI6IkpvaG4gRG9lIiwiaWF0IjoxNTE2MjM5MDIyfQ.SflKxwRJSMeKKF2QT4fwpMeJf36POk6yJV_adQssw5c`.'
  flows:
  - flow: password
    tokenUrl: /oauth/token
  name: oauth2
  source: openapi/billieio-billie-direct-api-openapi.yml
scope_count: 1
scope_names:
- default
scopes:
- description: default
  flows:
  - password
  scope: default
slug: billieio-scopes
source_filename: billieio-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: derived\nsource: openapi/billieio-billie-direct-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/billieio-billie-direct-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: /oauth/token\n  description: |-\n    This authentication mechanism is based on the OAuth 2.0 prototocol and requires a Client ID, a Client Secret Key and\n    in some cases also a user and password.\n\n    With these credentials, the client should request a token using the `POST /api/v1/oauth/token` endpoint,\n    which should be used in the `Authorization` header together with the `Bearer` challenge to authenticate all the requests.\n\n    > Example: `Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiIxMjM0NTY3ODkwIiwibmFtZSI6IkpvaG4gRG9lIiwiaWF0IjoxNTE2MjM5MDIyfQ.SflKxwRJSMeKKF2QT4fwpMeJf36POk6yJV_adQssw5c`.\nscopes:\n- scope: default\n  description: default\n  flows:\n  - password\n  sources:\n  - openapi/billieio-billie-direct-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/billieio/refs/heads/main/scopes/billieio-scopes.yml
summary_line: 1 scope · password
tags:
- Fintech
- Payments
- B2B
- Europe
token_bound: false
token_urls:
- /oauth/token
---
