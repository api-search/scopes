---
api_specs:
- filename: quartzy-inventory-items-api-openapi.yml
  format: yaml
  label: Quartzy Inventory Items API
  slug: quartzy-inventory-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quartzy/refs/heads/main/openapi/quartzy-inventory-items-api-openapi.yml
- filename: quartzy-labs-api-openapi.yml
  format: yaml
  label: Quartzy Labs API
  slug: quartzy-labs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quartzy/refs/heads/main/openapi/quartzy-labs-api-openapi.yml
- filename: quartzy-order-requests-api-openapi.yml
  format: yaml
  label: Quartzy Order Requests API
  slug: quartzy-order-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quartzy/refs/heads/main/openapi/quartzy-order-requests-api-openapi.yml
- filename: quartzy-types-api-openapi.yml
  format: yaml
  label: Quartzy Types API
  slug: quartzy-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quartzy/refs/heads/main/openapi/quartzy-types-api-openapi.yml
- filename: quartzy-user-api-openapi.yml
  format: yaml
  label: Quartzy User API
  slug: quartzy-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quartzy/refs/heads/main/openapi/quartzy-user-api-openapi.yml
- filename: quartzy-webhooks-api-openapi.yml
  format: yaml
  label: Quartzy Webhooks API
  slug: quartzy-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quartzy/refs/heads/main/openapi/quartzy-webhooks-api-openapi.yml
authorization_urls:
- https://app.quartzy.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: none
name: Quartzy Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Quartzy uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.quartzy.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Quartzy
provider_slug: quartzy
schemes:
- description: OAuth2 authorization for Quartzy API access.
  flows:
  - authorizationUrl: https://app.quartzy.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.quartzy.com/oauth/token
  name: oauth2
  source: openapi/quartzy-inventory-items-api-openapi.yml
- description: OAuth2 authorization for Quartzy API access.
  flows:
  - authorizationUrl: https://app.quartzy.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.quartzy.com/oauth/token
  name: oauth2
  source: openapi/quartzy-labs-api-openapi.yml
- description: OAuth2 authorization for Quartzy API access.
  flows:
  - authorizationUrl: https://app.quartzy.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.quartzy.com/oauth/token
  name: oauth2
  source: openapi/quartzy-order-requests-api-openapi.yml
- description: OAuth2 authorization for Quartzy API access.
  flows:
  - authorizationUrl: https://app.quartzy.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.quartzy.com/oauth/token
  name: oauth2
  source: openapi/quartzy-types-api-openapi.yml
- description: OAuth2 authorization for Quartzy API access.
  flows:
  - authorizationUrl: https://app.quartzy.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.quartzy.com/oauth/token
  name: oauth2
  source: openapi/quartzy-user-api-openapi.yml
- description: OAuth2 authorization for Quartzy API access.
  flows:
  - authorizationUrl: https://app.quartzy.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.quartzy.com/oauth/token
  name: oauth2
  source: openapi/quartzy-webhooks-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: quartzy-scopes
source_filename: quartzy-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/quartzy-inventory-items-api-openapi.yml, openapi/quartzy-labs-api-openapi.yml,\n  openapi/quartzy-order-requests-api-openapi.yml, openapi/quartzy-types-api-openapi.yml, openapi/quartzy-user-api-openapi.yml,\n  openapi/quartzy-webhooks-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/quartzy-inventory-items-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.quartzy.com/oauth/authorize\n    tokenUrl: https://api.quartzy.com/oauth/token\n  description: OAuth2 authorization for Quartzy API access.\n- name: oauth2\n  source: openapi/quartzy-labs-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.quartzy.com/oauth/authorize\n    tokenUrl: https://api.quartzy.com/oauth/token\n  description: OAuth2 authorization for Quartzy API access.\n- name: oauth2\n  source: openapi/quartzy-order-requests-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n\
  \    authorizationUrl: https://app.quartzy.com/oauth/authorize\n    tokenUrl: https://api.quartzy.com/oauth/token\n  description: OAuth2 authorization for Quartzy API access.\n- name: oauth2\n  source: openapi/quartzy-types-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.quartzy.com/oauth/authorize\n    tokenUrl: https://api.quartzy.com/oauth/token\n  description: OAuth2 authorization for Quartzy API access.\n- name: oauth2\n  source: openapi/quartzy-user-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.quartzy.com/oauth/authorize\n    tokenUrl: https://api.quartzy.com/oauth/token\n  description: OAuth2 authorization for Quartzy API access.\n- name: oauth2\n  source: openapi/quartzy-webhooks-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.quartzy.com/oauth/authorize\n    tokenUrl: https://api.quartzy.com/oauth/token\n  description: OAuth2 authorization for Quartzy\
  \ API access.\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quartzy/refs/heads/main/scopes/quartzy-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Lab Management
- Inventory
- Life Sciences
- Procurement
- Ordering
- Laboratory
- Webhook
token_bound: false
token_urls:
- https://api.quartzy.com/oauth/token
---
