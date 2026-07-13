---
api_specs:
- filename: corelogic-trestle-reso-web-api-openapi.yml
  format: yaml
  label: Trestle RESO Web API
  slug: trestle-reso-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/corelogic/refs/heads/main/openapi/corelogic-trestle-reso-web-api-openapi.yml
- filename: corelogic-direct-webapi-crm-openapi.yml
  format: yaml
  label: Direct Web API — CRM
  slug: direct-webapi-crm
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/corelogic/refs/heads/main/openapi/corelogic-direct-webapi-crm-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Corelogic Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CoreLogic (Cotality) publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the CoreLogic (Cotality) API on a user''s behalf.


  Tokens are issued from https://api.cotality.com/trestle/oidc/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CoreLogic (Cotality)
provider_slug: corelogic
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.cotality.com/trestle/oidc/connect/token
  name: oauth2ClientCredentials
  source: openapi/corelogic-trestle-reso-web-api-openapi.yml
scope_count: 1
scope_names:
- api
scopes:
- description: Access to the Trestle RESO Web API
  flows:
  - clientCredentials
  scope: api
slug: corelogic-scopes
source_filename: corelogic-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/corelogic-trestle-reso-web-api-openapi.yml\nschemes:\n- name: oauth2ClientCredentials\n  source: openapi/corelogic-trestle-reso-web-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.cotality.com/trestle/oidc/connect/token\nscopes:\n- scope: api\n  description: Access to the Trestle RESO Web API\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/corelogic-trestle-reso-web-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corelogic/refs/heads/main/scopes/corelogic-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Climate Risk
- CoreLogic
- Cotality
- Direct Web API
- Hazard Data
- Insurance Data
- Listings
- Matrix MLS
- Mortgage Data
- MLS
- OData
- OneHome
- OpenID Connect
- Participant Reporting
- Property Data
- Real Estate
- RESO Data Dictionary
- RESO Web API
- RETS
- Tax Data
- Trestle
token_urls:
- https://api.cotality.com/trestle/oidc/connect/token
---
