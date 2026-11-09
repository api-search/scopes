---
api_specs:
- filename: zaptec-chargehistory-api-openapi.yml
  format: yaml
  label: Zaptec Charge History API
  slug: zaptec-chargehistory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zaptec/openapi/zaptec-chargehistory-api-openapi.yml
- filename: zaptec-charger-api-openapi.yml
  format: yaml
  label: Zaptec Charger API
  slug: zaptec-charger-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zaptec/openapi/zaptec-charger-api-openapi.yml
- filename: zaptec-chargerfirmware-api-openapi.yml
  format: yaml
  label: Zaptec Charger Firmware API
  slug: zaptec-chargerfirmware-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zaptec/openapi/zaptec-chargerfirmware-api-openapi.yml
- filename: zaptec-constants-api-openapi.yml
  format: yaml
  label: Zaptec Constants API
  slug: zaptec-constants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zaptec/openapi/zaptec-constants-api-openapi.yml
- filename: zaptec-installation-api-openapi.yml
  format: yaml
  label: Zaptec Installation API
  slug: zaptec-installation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zaptec/openapi/zaptec-installation-api-openapi.yml
- filename: zaptec-session-api-openapi.yml
  format: yaml
  label: Zaptec Session API
  slug: zaptec-session-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zaptec/openapi/zaptec-session-api-openapi.yml
- filename: zaptec-user-group-api-openapi.yml
  format: yaml
  label: Zaptec User Group API
  slug: zaptec-user-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zaptec/openapi/zaptec-user-group-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- password
kind: oauth-scopes
layout: scope
method: none
name: Zaptec Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Zaptec uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.zaptec.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Zaptec
provider_slug: zaptec
schemes:
- flows:
  - flow: password
    tokenUrl: https://api.zaptec.com/oauth/token
  name: ory_auth
  source: openapi/api_zaptec_swagger.json
scope_count: 0
scope_names: []
scopes: []
slug: zaptec-scopes
source_filename: zaptec-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: none\nsource: openapi/api_zaptec_swagger.json\nschemes:\n- name: ory_auth\n  source: openapi/api_zaptec_swagger.json\n  flows:\n  - flow: password\n    tokenUrl: https://api.zaptec.com/oauth/token\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://artifacts.apis.io/zaptec/scopes/zaptec-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- EV Charging
- Smart Charging
- Energy
- Sustainability
- Platform
token_bound: false
token_urls:
- https://api.zaptec.com/oauth/token
---
