---
api_specs:
- filename: hydro-quebec-open-data-explore-api-v2-1-openapi.json
  format: json
  label: Hydro-Québec Open Data Explore API v2.1
  slug: hydro-quebec-open-data-explore-api-v2-1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hydro-quebec/refs/heads/main/openapi/hydro-quebec-open-data-explore-api-v2-1-openapi.json
- filename: hydro-quebec-open-data-explore-api-v2-0-openapi.json
  format: json
  label: Hydro-Québec Open Data Explore API v2.0
  slug: hydro-quebec-open-data-explore-api-v2-0
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hydro-quebec/refs/heads/main/openapi/hydro-quebec-open-data-explore-api-v2-0-openapi.json
authorization_urls:
- https://donnees.hydroquebec.com/oauth2/authorize/
description: ''
docs: https://help.opendatasoft.com/apis/ods-explore-v2/explore_v2.1.html
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Hydro Quebec Scopes
name_suffix: OAuth Scopes
note: 'The harvested OpenAPI declares only an apiKey scheme, so the mechanical derive pass found no oauth2 flows. The Opendatasoft platform that serves donnees.hydroquebec.com does implement OAuth2, and both endpoints were verified live on the Hydro-Québec domain: /oauth2/authorize/ returned HTTP 302 and /oauth2/token/ returned HTTP 405 (POST only) on 2026-07-27. The scope surface is deliberately minimal — the platform documents exactly one scope. This is an authorization surface that exists but is undeclared in the machine-readable contract.'
overview: 'Hydro-Québec publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Hydro-Québec API on a user''s behalf.


  Tokens are issued from https://donnees.hydroquebec.com/oauth2/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hydro-Québec
provider_slug: hydro-quebec
schemes:
- flows:
  - authorizationUrl: https://donnees.hydroquebec.com/oauth2/authorize/
    authorization_code_length: 30
    authorization_code_ttl: 1 hour
    authorization_url_status: 302
    flow: authorizationCode
    parameters:
    - client_id
    - redirect_uri
    - response_type
    - scope
    - state
    refresh_supported: true
    response_type: code
    state_recommended: true
    tokenUrl: https://donnees.hydroquebec.com/oauth2/token/
    token_url_status: 405
    verified: '2026-07-27'
  name: oauth2
  rfc:
  - RFC 6749
  - RFC 6750
  source: https://help.opendatasoft.com/apis/ods-explore-v2/explore_v2.1.html
  token_type: Bearer
scope_count: 1
scope_names:
- all
scopes:
- description: Full access to the platform APIs on behalf of the authorizing user. The platform documentation states verbatim that "Currently, only all is supported" — there is no read/write or per-resource scope decomposition.
  flows:
  - authorizationCode
  scope: all
slug: hydro-quebec-scopes
source_filename: hydro-quebec-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: https://help.opendatasoft.com/apis/ods-explore-v2/explore_v2.1.html (Using OAuth2 authorization)\ndocs: https://help.opendatasoft.com/apis/ods-explore-v2/explore_v2.1.html\nnote: >-\n  The harvested OpenAPI declares only an apiKey scheme, so the mechanical derive pass found no\n  oauth2 flows. The Opendatasoft platform that serves donnees.hydroquebec.com does implement\n  OAuth2, and both endpoints were verified live on the Hydro-Québec domain: /oauth2/authorize/\n  returned HTTP 302 and /oauth2/token/ returned HTTP 405 (POST only) on 2026-07-27. The scope\n  surface is deliberately minimal — the platform documents exactly one scope. This is an\n  authorization surface that exists but is undeclared in the machine-readable contract.\nundeclared_in_spec: true\nschemes:\n- name: oauth2\n  source: https://help.opendatasoft.com/apis/ods-explore-v2/explore_v2.1.html\n  rfc: [RFC 6749, RFC 6750]\n  token_type: Bearer\n  flows:\n \
  \ - flow: authorizationCode\n    authorizationUrl: https://donnees.hydroquebec.com/oauth2/authorize/\n    tokenUrl: https://donnees.hydroquebec.com/oauth2/token/\n    verified: '2026-07-27'\n    authorization_url_status: 302\n    token_url_status: 405\n    parameters: [client_id, redirect_uri, response_type, scope, state]\n    response_type: code\n    authorization_code_length: 30\n    authorization_code_ttl: 1 hour\n    refresh_supported: true\n    state_recommended: true\nscopes:\n- scope: all\n  description: >-\n    Full access to the platform APIs on behalf of the authorizing user. The platform documentation\n    states verbatim that \"Currently, only all is supported\" — there is no read/write or\n    per-resource scope decomposition.\n  flows: [authorizationCode]\n  sources: [https://help.opendatasoft.com/apis/ods-explore-v2/explore_v2.1.html]\nclient_registration:\n  self_service: true\n  url: https://donnees.hydroquebec.com/account/\n  tab: My applications\n  client_types: [confidential,\
  \ public]\n  domain_bound: true\n  domain_bound_note: >-\n    Applications are registered against one specific domain and can only access data on that\n    domain, so a client registered elsewhere cannot read donnees.hydroquebec.com.\napi_keys:\n  self_service: true\n  url: https://donnees.hydroquebec.com/account/\n  tab: My API keys\n  permissions_note: >-\n    By default an API key authenticates as the user who created it and grants that user's rights,\n    so keys must not be shared. Key permissions can be narrowed through the platform's API key\n    Automation API.\napplicability:\n  note: >-\n    None of this is required to read Hydro-Québec's open data. All 26 datasets are public and\n    anonymously callable. OAuth2 and API keys matter only for authenticated identity, per-user\n    quota, or access to a private catalog — which Hydro-Québec does not operate.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hydro-quebec/refs/heads/main/scopes/hydro-quebec-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Energy
- Canada
- Utilities
- Electricity
- Grid
- Energy Markets
- Renewables
- Open Data
- Demand Response
- Carbon
token_urls:
- https://donnees.hydroquebec.com/oauth2/token/
---
