---
api_specs:
- filename: bloomberg-aim-broker-strategies-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Broker Strategies API
  slug: bloomberg-aim-broker-strategies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-broker-strategies-api-openapi.yml
- filename: bloomberg-aim-catalogs-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Catalogs API
  slug: bloomberg-aim-catalogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-catalogs-api-openapi.yml
- filename: bloomberg-aim-distributions-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Distributions API
  slug: bloomberg-aim-distributions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-distributions-api-openapi.yml
- filename: bloomberg-aim-field-lists-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Field Lists API
  slug: bloomberg-aim-field-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-field-lists-api-openapi.yml
- filename: bloomberg-aim-field-search-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Field Search API
  slug: bloomberg-aim-field-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-field-search-api-openapi.yml
- filename: bloomberg-aim-fills-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Fills API
  slug: bloomberg-aim-fills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-fills-api-openapi.yml
- filename: bloomberg-aim-historical-data-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Historical Data API
  slug: bloomberg-aim-historical-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-historical-data-api-openapi.yml
- filename: bloomberg-aim-instruments-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Instruments API
  slug: bloomberg-aim-instruments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-instruments-api-openapi.yml
- filename: bloomberg-aim-intraday-data-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Intraday Data API
  slug: bloomberg-aim-intraday-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-intraday-data-api-openapi.yml
- filename: bloomberg-aim-orders-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Orders API
  slug: bloomberg-aim-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-orders-api-openapi.yml
- filename: bloomberg-aim-reference-data-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Reference Data API
  slug: bloomberg-aim-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-reference-data-api-openapi.yml
- filename: bloomberg-aim-replies-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Replies API
  slug: bloomberg-aim-replies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-replies-api-openapi.yml
- filename: bloomberg-aim-requests-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Requests API
  slug: bloomberg-aim-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-requests-api-openapi.yml
- filename: bloomberg-aim-routes-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Routes API
  slug: bloomberg-aim-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-routes-api-openapi.yml
- filename: bloomberg-aim-teams-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Teams API
  slug: bloomberg-aim-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-teams-api-openapi.yml
- filename: bloomberg-aim-triggers-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Triggers API
  slug: bloomberg-aim-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-triggers-api-openapi.yml
- filename: bloomberg-aim-universes-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Universes API
  slug: bloomberg-aim-universes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-universes-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Bloomberg Aim Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Bloomberg AIM publishes 3 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Bloomberg AIM API on a user''s behalf.


  Tokens are issued from https://bsso.blpprofessional.com/ext/api/as/token.oauth2.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schemes:
- description: OAuth 2.0 client credentials flow
  flows:
  - flow: clientCredentials
    tokenUrl: https://bsso.blpprofessional.com/ext/api/as/token.oauth2
  name: oauth2
  source: openapi/bloomberg-data-license-api.yml
scope_count: 3
scope_names:
- eap
- eap.catalogs.read
- eap.catalogs.write
scopes:
- description: Access to Enterprise Access Point data
  flows:
  - clientCredentials
  scope: eap
- description: Read catalog data
  flows:
  - clientCredentials
  scope: eap.catalogs.read
- description: Write catalog data
  flows:
  - clientCredentials
  scope: eap.catalogs.write
slug: bloomberg-aim-scopes
source_filename: bloomberg-aim-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bloomberg-data-license-api.yml\nschemes:\n- name: oauth2\n  source: openapi/bloomberg-data-license-api.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://bsso.blpprofessional.com/ext/api/as/token.oauth2\n  description: OAuth 2.0 client credentials flow\nscopes:\n- scope: eap\n  description: Access to Enterprise Access Point data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bloomberg-data-license-api.yml\n- scope: eap.catalogs.read\n  description: Read catalog data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bloomberg-data-license-api.yml\n- scope: eap.catalogs.write\n  description: Write catalog data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bloomberg-data-license-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/scopes/bloomberg-aim-scopes.yml
summary_line: 3 scopes · clientCredentials
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio-Management
- Trading
token_urls:
- https://bsso.blpprofessional.com/ext/api/as/token.oauth2
---
