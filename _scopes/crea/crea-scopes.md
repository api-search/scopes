---
api_specs:
- filename: crea-realtor-ca-ddf-web-api-openapi.json
  format: json
  label: REALTOR.ca DDF Web API
  slug: realtor-ca-ddf-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crea/refs/heads/main/openapi/crea-realtor-ca-ddf-web-api-openapi.json
- filename: crea-realtor-ca-ddf-web-api-openapi.json
  format: json
  label: REALTOR.ca DDF Lead API
  slug: realtor-ca-ddf-lead-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crea/refs/heads/main/openapi/crea-realtor-ca-ddf-web-api-openapi.json
- filename: crea-realtor-ca-board-api-openapi.json
  format: json
  label: REALTOR.ca Board API
  slug: realtor-ca-board-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crea/refs/heads/main/openapi/crea-realtor-ca-board-api-openapi.json
authorization_urls:
- https://identity.crea.ca/connect/authorize
description: CREA publishes no scopes reference page, but the OpenID Connect discovery document at identity.crea.ca is served anonymously and enumerates every scope the shared authorization server will issue. Two of the five are documented in the API docs (DDFApi_Read and BoardDataApi.read); the other three are advertised by discovery only. Neither OpenAPI document declares an oauth2 securityScheme, so nothing here could be derived from the specs - this file is entirely searched.
docs: https://ddfapi-docs.realtor.ca/#section/Authorization/API-Access-Tokens
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Crea Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CREA (REALTOR.ca) publishes 5 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the CREA (REALTOR.ca) API on a user''s behalf.


  Tokens are issued from https://identity.crea.ca/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CREA (REALTOR.ca)
provider_slug: crea
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://identity.crea.ca/connect/token
  - authorizationUrl: https://identity.crea.ca/connect/authorize
    flow: authorizationCode
    note: Advertised by discovery; not documented for the public DDF or Board APIs.
    tokenUrl: https://identity.crea.ca/connect/token
  name: CREA IdentityServer
  source: https://identity.crea.ca/.well-known/openid-configuration
scope_count: 5
scope_names:
- DDFApi_Read
- BoardDataApi.read
- OfferManagementApi.read.write
- openid
- offline_access
scopes:
- description: Read access to the REALTOR.ca DDF Web API (OData v4 Property, Member, Office, OpenHouse, Destination and the three Replication collections) and to the DDF Lead API endpoint. This is the only scope documented for DDF; despite the _Read suffix it also covers the single write operation, POST /v1/Lead/CreateLead.
  flows:
  - clientCredentials
  scope: DDFApi_Read
- description: Read access to the REALTOR.ca Board API roster endpoints (GET /Member, GET /Office and their single-record forms) for a member board or association.
  flows:
  - clientCredentials
  scope: BoardDataApi.read
- description: Read and write access to a CREA Offer Management API. No public documentation, OpenAPI or developer surface for this API could be found on 2026-07-26 - it is known only from this discovery document, and corresponds to the offer-management product CREA has been rolling out on REALTOR.ca. Recorded here because it is genuinely advertised, not because it is consumable.
  flows:
  - clientCredentials
  scope: OfferManagementApi.read.write
- description: Standard OpenID Connect scope; returns an id_token and the sub claim.
  flows:
  - authorizationCode
  scope: openid
- description: Standard OAuth 2.0 scope requesting a refresh token. Not applicable to the documented client-credentials flows.
  flows:
  - authorizationCode
  scope: offline_access
slug: crea-scopes
source_filename: crea-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: https://identity.crea.ca/.well-known/openid-configuration\ndocs: https://ddfapi-docs.realtor.ca/#section/Authorization/API-Access-Tokens\ndescription: >-\n  CREA publishes no scopes reference page, but the OpenID Connect discovery document at\n  identity.crea.ca is served anonymously and enumerates every scope the shared authorization\n  server will issue. Two of the five are documented in the API docs (DDFApi_Read and\n  BoardDataApi.read); the other three are advertised by discovery only. Neither OpenAPI\n  document declares an oauth2 securityScheme, so nothing here could be derived from the specs -\n  this file is entirely searched.\nissuer: https://identity.crea.ca\nschemes:\n- name: CREA IdentityServer\n  source: https://identity.crea.ca/.well-known/openid-configuration\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://identity.crea.ca/connect/token\n  - flow: authorizationCode\n    authorizationUrl: https://identity.crea.ca/connect/authorize\n\
  \    tokenUrl: https://identity.crea.ca/connect/token\n    note: Advertised by discovery; not documented for the public DDF or Board APIs.\nscopes:\n- scope: DDFApi_Read\n  description: >-\n    Read access to the REALTOR.ca DDF Web API (OData v4 Property, Member, Office, OpenHouse,\n    Destination and the three Replication collections) and to the DDF Lead API endpoint. This\n    is the only scope documented for DDF; despite the _Read suffix it also covers the single\n    write operation, POST /v1/Lead/CreateLead.\n  flows: [clientCredentials]\n  documented: true\n  sources: [https://identity.crea.ca/.well-known/openid-configuration, 'https://ddfapi-docs.realtor.ca/']\n- scope: BoardDataApi.read\n  description: >-\n    Read access to the REALTOR.ca Board API roster endpoints (GET /Member, GET /Office and\n    their single-record forms) for a member board or association.\n  flows: [clientCredentials]\n  documented: true\n  sources: [https://identity.crea.ca/.well-known/openid-configuration,\
  \ 'https://boardapi-docs.realtor.ca/']\n- scope: OfferManagementApi.read.write\n  description: >-\n    Read and write access to a CREA Offer Management API. No public documentation, OpenAPI or\n    developer surface for this API could be found on 2026-07-26 - it is known only from this\n    discovery document, and corresponds to the offer-management product CREA has been rolling\n    out on REALTOR.ca. Recorded here because it is genuinely advertised, not because it is\n    consumable.\n  flows: [clientCredentials]\n  documented: false\n  sources: [https://identity.crea.ca/.well-known/openid-configuration]\n- scope: openid\n  description: Standard OpenID Connect scope; returns an id_token and the sub claim.\n  flows: [authorizationCode]\n  documented: false\n  sources: [https://identity.crea.ca/.well-known/openid-configuration]\n- scope: offline_access\n  description: Standard OAuth 2.0 scope requesting a refresh token. Not applicable to the documented client-credentials flows.\n  flows:\
  \ [authorizationCode]\n  documented: false\n  sources: [https://identity.crea.ca/.well-known/openid-configuration]\nclaims_supported: [sub, destinationid]\nclaims_note: >-\n  destinationid is the tenancy claim - it binds an issued DDF token to a specific Destination\n  (data feed), which is how CREA scopes a Technology Provider's merged feed.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crea/refs/heads/main/scopes/crea-scopes.yml
summary_line: 5 scopes · clientCredentials/authorizationCode
tags:
- Real-Estate
- Canada
- Property Listings
- MLS
- IDX
- RESO
- OData
- Industry Body
- PropTech
- Data Syndication
token_urls:
- https://identity.crea.ca/connect/token
---
