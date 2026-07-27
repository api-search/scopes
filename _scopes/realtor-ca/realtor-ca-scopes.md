---
api_specs:
- filename: realtor-ca-ddf-web-api-openapi.json
  format: json
  label: REALTOR.ca DDF Web API
  slug: realtor-ca-ddf-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/realtor-ca/refs/heads/main/openapi/realtor-ca-ddf-web-api-openapi.json
- filename: realtor-ca-ddf-web-api-openapi.json
  format: json
  label: REALTOR.ca DDF Lead API
  slug: realtor-ca-ddf-lead-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/realtor-ca/refs/heads/main/openapi/realtor-ca-ddf-web-api-openapi.json
authorization_urls:
- https://identity.crea.ca/connect/authorize
description: ''
docs: https://ddfapi-docs.realtor.ca/#section/Authorization
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Realtor Ca Scopes
name_suffix: OAuth Scopes
note: 'derive-oauth-scopes.py returned zero because neither harvested OpenAPI declares an oauth2 securityScheme. The scopes below are SEARCHED: CREA''s authorization server publishes them anonymously in its discovery document, and the documentation names exactly one — DDFApi_Read — as the scope a DDF data feed requests. The other three are advertised by the same authorization server for CREA products that have no public documentation and no resolvable host; they are recorded as observed-but-undocumented, and no endpoint was invented for them.'
overview: 'REALTOR.ca publishes 5 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the REALTOR.ca API on a user''s behalf.


  Tokens are issued from https://identity.crea.ca/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: REALTOR.ca
provider_slug: realtor-ca
schemes:
- flows:
  - authorizationUrl: https://identity.crea.ca/connect/authorize
    flow: clientCredentials
    tokenUrl: https://identity.crea.ca/connect/token
  name: DDFApiOAuth2
  source: https://identity.crea.ca/.well-known/openid-configuration
scope_count: 5
scope_names:
- DDFApi_Read
- openid
- offline_access
- OfferManagementApi.read.write
- BoardDataApi.read
scopes:
- description: Read access to the REALTOR.ca DDF Web API — the Property, Member, Office, OpenHouse and Destination OData resources and their Replication endpoints, restricted to the Destinations entitled to the calling data feed. This is the only scope CREA documents, and the only one a DDF integrator requests.
  flows:
  - clientCredentials
  scope: DDFApi_Read
- description: Standard OpenID Connect scope; returns an ID token for interactive flows.
  flows:
  - authorizationCode
  - implicit
  scope: openid
- description: Standard OAuth 2.0 scope requesting a refresh token. Not applicable to the documented client_credentials DDF flow.
  flows:
  - authorizationCode
  scope: offline_access
- description: Read/write access to a CREA offer-management API. Advertised by identity.crea.ca but CREA publishes no documentation, no host and no key-issuance path for it — offerapi.crea.ca and offermanagement-docs.realtor.ca do not resolve.
  flows:
  - clientCredentials
  scope: OfferManagementApi.read.write
- description: Read access to a CREA board-data API. Advertised by identity.crea.ca but undocumented — boarddataapi.crea.ca and boarddata-docs.realtor.ca do not resolve.
  flows:
  - clientCredentials
  scope: BoardDataApi.read
slug: realtor-ca-scopes
source_filename: realtor-ca-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: >-\n  https://identity.crea.ca/.well-known/openid-configuration (HTTP 200, anonymous) — the\n  `scopes_supported` array — cross-read against the \"API Access Tokens\" table in the DDF Web API\n  documentation\ndocs: https://ddfapi-docs.realtor.ca/#section/Authorization\nnote: >-\n  derive-oauth-scopes.py returned zero because neither harvested OpenAPI declares an oauth2\n  securityScheme. The scopes below are SEARCHED: CREA's authorization server publishes them\n  anonymously in its discovery document, and the documentation names exactly one — DDFApi_Read —\n  as the scope a DDF data feed requests. The other three are advertised by the same authorization\n  server for CREA products that have no public documentation and no resolvable host; they are\n  recorded as observed-but-undocumented, and no endpoint was invented for them.\nschemes:\n- name: DDFApiOAuth2\n  source: https://identity.crea.ca/.well-known/openid-configuration\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://identity.crea.ca/connect/token\n    authorizationUrl: https://identity.crea.ca/connect/authorize\nscopes:\n- scope: DDFApi_Read\n  description: >-\n    Read access to the REALTOR.ca DDF Web API — the Property, Member, Office, OpenHouse and\n    Destination OData resources and their Replication endpoints, restricted to the Destinations\n    entitled to the calling data feed. This is the only scope CREA documents, and the only one a\n    DDF integrator requests.\n  flows: [clientCredentials]\n  documented: true\n  sources: [https://ddfapi-docs.realtor.ca/#section/Authorization]\n- scope: openid\n  description: Standard OpenID Connect scope; returns an ID token for interactive flows.\n  flows: [authorizationCode, implicit]\n  documented: false\n  sources: [https://identity.crea.ca/.well-known/openid-configuration]\n- scope: offline_access\n  description: Standard OAuth 2.0 scope requesting a refresh token. Not applicable to the\
  \ documented client_credentials DDF flow.\n  flows: [authorizationCode]\n  documented: false\n  sources: [https://identity.crea.ca/.well-known/openid-configuration]\n- scope: OfferManagementApi.read.write\n  description: >-\n    Read/write access to a CREA offer-management API. Advertised by identity.crea.ca but CREA\n    publishes no documentation, no host and no key-issuance path for it — offerapi.crea.ca and\n    offermanagement-docs.realtor.ca do not resolve.\n  flows: [clientCredentials]\n  documented: false\n  undocumented_product: true\n  sources: [https://identity.crea.ca/.well-known/openid-configuration]\n- scope: BoardDataApi.read\n  description: >-\n    Read access to a CREA board-data API. Advertised by identity.crea.ca but undocumented —\n    boarddataapi.crea.ca and boarddata-docs.realtor.ca do not resolve.\n  flows: [clientCredentials]\n  documented: false\n  undocumented_product: true\n  sources: [https://identity.crea.ca/.well-known/openid-configuration]\nsummary:\n  total:\
  \ 5\n  documented: 1\n  granularity: >-\n    Coarse. One read scope covers the entire national listing pool; entitlement is enforced not by\n    scope but by the `destinationid` claim bound to the credential — a feed sees only the\n    Destinations a member or broker owner linked to it. There is no per-resource, per-board or\n    per-field scope.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/realtor-ca/refs/heads/main/scopes/realtor-ca-scopes.yml
summary_line: 5 scopes · clientCredentials
tags:
- Real Estate
- Canada
- Property Listings
- MLS
- RESO
- IDX
- Listing Syndication
- PropTech
- OData
- Rentals
token_urls:
- https://identity.crea.ca/connect/token
---
