---
api_specs:
- filename: ordnance-survey-ngd-features-openapi.json
  format: json
  label: OS NGD API - Features
  slug: os-ngd-api-features
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/openapi/ordnance-survey-ngd-features-openapi.json
- filename: ordnance-survey-ngd-tiles-openapi.json
  format: json
  label: OS NGD API - Tiles
  slug: os-ngd-api-tiles
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/openapi/ordnance-survey-ngd-tiles-openapi.json
- filename: ordnance-survey-downloads-openapi.yaml
  format: yaml
  label: OS Downloads API
  slug: os-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/openapi/ordnance-survey-downloads-openapi.yaml
- filename: ordnance-survey-osnet-openapi.yaml
  format: yaml
  label: OS Net API
  slug: os-net-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/openapi/ordnance-survey-osnet-openapi.yaml
- filename: ordnance-survey-places-openapi.json
  format: json
  label: OS Places API
  slug: os-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/openapi/ordnance-survey-places-openapi.json
- filename: ordnance-survey-names-openapi.json
  format: json
  label: OS Names API
  slug: os-names-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/openapi/ordnance-survey-names-openapi.json
- filename: ordnance-survey-linked-identifiers-openapi.json
  format: json
  label: OS Linked Identifiers API
  slug: os-linked-identifiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/openapi/ordnance-survey-linked-identifiers-openapi.json
- filename: ordnance-survey-features-wfs-openapi.json
  format: json
  label: OS Features API
  slug: os-features-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/openapi/ordnance-survey-features-wfs-openapi.json
- filename: ordnance-survey-maps-openapi.json
  format: json
  label: OS Maps API
  slug: os-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/openapi/ordnance-survey-maps-openapi.json
- filename: ordnance-survey-vector-tile-openapi.json
  format: json
  label: OS Vector Tile API
  slug: os-vector-tile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/openapi/ordnance-survey-vector-tile-openapi.json
authorization_urls: []
description: 'Ordnance Survey runs OAuth 2.0 as a bare client-credentials token service and publishes NO named scopes. The OS OAuth 2 API documentation describes only grant_type=client_credentials against https://api.os.uk/oauth2/token/v1 with HTTP Basic (Project API Key : Project API Secret), returning access_token / expires_in / issued_at / token_type. Authorisation is carried by which APIs are attached to the OS Data Hub API Project, not by scope strings - so a token that is refused returns 403 (not entitled) rather than an insufficient_scope error. The single scope below is the literal "read" scope declared in the operation security requirements of the OS Linked Identifiers OpenAPI fragments; it is not documented anywhere in prose and no other OS spec declares it.'
docs: https://docs.os.uk/os-apis/core-concepts/authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Ordnance Survey Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Ordnance Survey publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Ordnance Survey API on a user''s behalf.


  Tokens are issued from https://api.os.uk/oauth2/token/v1.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Ordnance Survey
provider_slug: ordnance-survey
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.os.uk/oauth2/token/v1
  name: OAuth2
  source: openapi/ordnance-survey-downloads-openapi.yaml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.os.uk/oauth2/token/v1
  name: OAuth2
  source: openapi/ordnance-survey-linked-identifiers-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.os.uk/oauth2/token/v1
  name: oauth2
  source: openapi/ordnance-survey-ngd-features-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.os.uk/oauth2/token/v1
  name: oauth2
  source: openapi/ordnance-survey-ngd-tiles-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: OAUTH_TOKEN_URL
  name: OAuth2
  source: openapi/ordnance-survey-osnet-openapi.yaml
scope_count: 1
scope_names:
- read
scopes:
- description: Grants read access
  flows:
  - clientCredentials
  scope: read
slug: ordnance-survey-scopes
source_filename: ordnance-survey-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: openapi/ordnance-survey-downloads-openapi.yaml, openapi/ordnance-survey-linked-identifiers-openapi.json,\n  openapi/ordnance-survey-ngd-features-openapi.json, openapi/ordnance-survey-ngd-tiles-openapi.json,\n  openapi/ordnance-survey-osnet-openapi.yaml\ndocs: https://docs.os.uk/os-apis/core-concepts/authentication\noauth2_docs: https://docs.os.uk/os-apis/accessing-os-apis/oauth-2-api/technical-specification\ndescription: >-\n  Ordnance Survey runs OAuth 2.0 as a bare client-credentials token service and\n  publishes NO named scopes. The OS OAuth 2 API documentation describes only\n  grant_type=client_credentials against https://api.os.uk/oauth2/token/v1 with\n  HTTP Basic (Project API Key : Project API Secret), returning access_token /\n  expires_in / issued_at / token_type. Authorisation is carried by which APIs\n  are attached to the OS Data Hub API Project, not by scope strings - so a\n  token that is refused returns 403\
  \ (not entitled) rather than an\n  insufficient_scope error. The single scope below is the literal \"read\" scope\n  declared in the operation security requirements of the OS Linked Identifiers\n  OpenAPI fragments; it is not documented anywhere in prose and no other OS\n  spec declares it.\ntoken_endpoint: https://api.os.uk/oauth2/token/v1\ngrant_types: [client_credentials]\ntoken_lifetime_seconds: 299\ndiscovery_document: none published\nschemes:\n- name: OAuth2\n  source: openapi/ordnance-survey-downloads-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.os.uk/oauth2/token/v1\n- name: OAuth2\n  source: openapi/ordnance-survey-linked-identifiers-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.os.uk/oauth2/token/v1\n- name: oauth2\n  source: openapi/ordnance-survey-ngd-features-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.os.uk/oauth2/token/v1\n- name: oauth2\n  source: openapi/ordnance-survey-ngd-tiles-openapi.json\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.os.uk/oauth2/token/v1\n- name: OAuth2\n  source: openapi/ordnance-survey-osnet-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: OAUTH_TOKEN_URL\nscopes:\n- scope: read\n  description: Grants read access\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/ordnance-survey-linked-identifiers-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/scopes/ordnance-survey-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Real-Estate
- United Kingdom
- Land Registry
- Geospatial
- Addressing
- Open Data
- Property Data
- PropTech
- Government
- Mapping
- OGC
- UPRN
- National Mapping
- GNSS
- Vector Tiles
token_urls:
- https://api.os.uk/oauth2/token/v1
- OAUTH_TOKEN_URL
---
