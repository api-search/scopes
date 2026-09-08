---
api_specs:
- filename: beacon-roofing-supply-v2-openapi.yml
  format: yaml
  label: Beacon PRO+ API (V2, OAuth)
  slug: beacon-pro-plus
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beacon-roofing-supply/refs/heads/main/openapi/beacon-roofing-supply-v2-openapi.yml
- filename: beacon-roofing-supply-all-api-openapi.yml
  format: yaml
  label: Beacon External Rest Service (all_api)
  slug: beacon-rest-all-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beacon-roofing-supply/refs/heads/main/openapi/beacon-roofing-supply-all-api-openapi.yml
- filename: beacon-roofing-supply-v3-openapi.yml
  format: yaml
  label: Beacon Rest Services V3 (Public / Integrations)
  slug: beacon-rest-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beacon-roofing-supply/refs/heads/main/openapi/beacon-roofing-supply-v3-openapi.yml
- filename: beacon-roofing-supply-v1-openapi.yml
  format: yaml
  label: Beacon Rest Services V1 (session)
  slug: beacon-rest-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beacon-roofing-supply/refs/heads/main/openapi/beacon-roofing-supply-v1-openapi.yml
- filename: beacon-roofing-supply-oauth2-openapi.yml
  format: yaml
  label: Beacon OAuth Rest Service
  slug: beacon-oauth
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beacon-roofing-supply/refs/heads/main/openapi/beacon-roofing-supply-oauth2-openapi.yml
- filename: beacon-roofing-supply-public-openapi.yml
  format: yaml
  label: Beacon Rest Services Public
  slug: beacon-rest-public
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beacon-roofing-supply/refs/heads/main/openapi/beacon-roofing-supply-public-openapi.yml
- filename: beacon-roofing-supply-internal-openapi.yml
  format: yaml
  label: Beacon Internal Rest Service
  slug: beacon-rest-internal
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beacon-roofing-supply/refs/heads/main/openapi/beacon-roofing-supply-internal-openapi.yml
authorization_urls: []
description: 'Beacon''s OAuth surface carries a `scopes` field, but it is NOT a permission scope in the RFC 6749 sense. It is a refresh-behaviour selector on the token endpoint: it tells the server which of the two tokens to re-mint. No document in the Beacon Rest Services set declares an oauth2 securityScheme with a `scopes` map, and no operation is gated on a named scope. Authorization is carried instead by the profile/permission-template model inside the API (see permission_model).'
docs: https://beaconproplus.com/swagger/oauth2/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Beacon Roofing Supply Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Beacon Roofing Supply uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Beacon Roofing Supply
provider_slug: beacon-roofing-supply
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: beacon-roofing-supply-scopes
source_filename: beacon-roofing-supply-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: >-\n  https://beaconproplus.com/swagger/oauth2/ and its backing document\n  openapi/beacon-roofing-supply-oauth2-openapi.yml (components.schemas.tokenReqObj.scopes and\n  tokenResp.scope)\nspecification: API Commons OAuth Scopes\nspecificationVersion: '0.1'\nprovider: Beacon Roofing Supply\nproviderId: beacon-roofing-supply\ndocs: https://beaconproplus.com/swagger/oauth2/\ndescription: >-\n  Beacon's OAuth surface carries a `scopes` field, but it is NOT a permission scope in the RFC 6749\n  sense. It is a refresh-behaviour selector on the token endpoint: it tells the server which of the\n  two tokens to re-mint. No document in the Beacon Rest Services set declares an oauth2\n  securityScheme with a `scopes` map, and no operation is gated on a named scope. Authorization is\n  carried instead by the profile/permission-template model inside the API (see permission_model).\nscope_semantics: refresh-selector\nscope_count: 3\nscopes:\n\
  \  - name: '(empty)'\n    description: 'Only refresh access_token. The refresh_token is left as-is.'\n    source: components.schemas.tokenReqObj.scopes description\n  - name: all\n    description: 'Refresh access_token AND refresh_token.'\n    source: components.schemas.tokenReqObj.scopes description\n  - name: refresh_token\n    description: >-\n      Also refresh access_token and refresh_token. Multiple values are separated by whitespace, per\n      the field description.\n    source: components.schemas.tokenReqObj.scopes description\ntoken_endpoint:\n  method: POST\n  url: https://beaconproplus.com/rest/model/REST/oauth/token\n  templated_server: 'https://{server}/rest/model/REST/oauth/ where server ∈ {beacon-uat.becn.com, beaconproplus.com}'\n  grant_type: refresh_token\n  request_fields: [grant_type, refresh_token, client_id, scopes]\n  response_fields: [access_token, token_type, expires_in, refresh_expires_in, refresh_token, scope, success, messages]\n  client_secret_required: false\n\
  \  note: >-\n    The published request takes client_id with no client_secret. The initial grant that issues the\n    first refresh_token is not published anywhere — it is arranged through partner onboarding at\n    https://go.qxo.com/qxoapi.\npermission_model:\n  style: profile + permission template (server-side, not scope-based)\n  operations:\n    - GET /getCurrentUserPermission\n    - GET /permissionTemplateList\n    - GET /getPermissionTemplateDetail\n    - POST /createPermissionTemplate\n    - POST /updatePermissionTemplate\n    - POST /deletePermissionTemplate\n  roles_referenced: [master admin user, admin user]\n  evidence: >-\n    102 operations declare a 403 whose description is \"Forbidden, user do not has permission to\n    access this API\"; eleven of those narrow it to \"only master admin user or admin user\". Message\n    code 2006 is \"Current profile is permission denied\".\n  agent_note: >-\n    An agent cannot determine from the contract which operations its token may\
  \ call. There is no\n    scope string to inspect and no capability discovery endpoint — the only way to learn the\n    permission surface is to call GET /getCurrentUserPermission at runtime, or to fail with 403.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beacon-roofing-supply/refs/heads/main/scopes/beacon-roofing-supply-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Construction
- Distribution
- Roofing
- Building Materials
- E-Commerce
- Fortune 1000
- Supply Chain
- Order
- Catalog
- Delivery
token_urls: []
---
