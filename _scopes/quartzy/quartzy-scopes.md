---
api_specs:
- filename: quartzy-openapi.yml
  format: yaml
  label: Quartzy Inventory Items API
  slug: quartzy-inventory-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quartzy/refs/heads/main/openapi/quartzy-openapi.yml
- filename: quartzy-openapi.yml
  format: yaml
  label: Quartzy Order Requests API
  slug: quartzy-order-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quartzy/refs/heads/main/openapi/quartzy-openapi.yml
- filename: quartzy-openapi.yml
  format: yaml
  label: Quartzy Types API
  slug: quartzy-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quartzy/refs/heads/main/openapi/quartzy-openapi.yml
- filename: quartzy-openapi.yml
  format: yaml
  label: Quartzy Labs API
  slug: quartzy-labs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quartzy/refs/heads/main/openapi/quartzy-openapi.yml
- filename: quartzy-openapi.yml
  format: yaml
  label: Quartzy Webhooks API
  slug: quartzy-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quartzy/refs/heads/main/openapi/quartzy-openapi.yml
authorization_urls:
- https://app.quartzy.com/oauth/authorize
description: ''
docs: https://docs.quartzy.com/api/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Quartzy Scopes
name_suffix: OAuth Scopes
note: Quartzy documents per-user AccessToken authentication (Access-Token header) and references OAuth2 in endpoint authorizations, but publishes no OAuth scopes or permission granularity (https://docs.quartzy.com/api/).
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
  source: openapi/quartzy-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: quartzy-scopes
source_filename: quartzy-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/quartzy-openapi.yml\ndocs: https://docs.quartzy.com/api/\nnote: Quartzy documents per-user AccessToken authentication (Access-Token header)\n  and references OAuth2 in endpoint authorizations, but publishes no OAuth scopes\n  or permission granularity (https://docs.quartzy.com/api/).\nschemes:\n- name: oauth2\n  source: openapi/quartzy-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.quartzy.com/oauth/authorize\n    tokenUrl: https://api.quartzy.com/oauth/token\n  description: OAuth2 authorization for Quartzy API access.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quartzy/refs/heads/main/scopes/quartzy-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Lab Management
- Inventory Management
- Life Sciences
- Procurement
- Ordering
- Laboratory
- Webhooks
token_urls:
- https://api.quartzy.com/oauth/token
---
