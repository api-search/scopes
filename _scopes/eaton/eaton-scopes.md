---
api_specs:
- filename: eaton-authorization-api-openapi.yml
  format: yaml
  label: Eaton Authorization API
  slug: eaton-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eaton/refs/heads/main/openapi/eaton-authorization-api-openapi.yml
- filename: eaton-device-commands-api-openapi.yml
  format: yaml
  label: Eaton Device Commands API
  slug: eaton-device-commands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eaton/refs/heads/main/openapi/eaton-device-commands-api-openapi.yml
- filename: eaton-devices-api-openapi.yml
  format: yaml
  label: Eaton Devices API
  slug: eaton-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eaton/refs/heads/main/openapi/eaton-devices-api-openapi.yml
- filename: eaton-energy-data-api-openapi.yml
  format: yaml
  label: Eaton Energy Data API
  slug: eaton-energy-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eaton/refs/heads/main/openapi/eaton-energy-data-api-openapi.yml
- filename: eaton-ev-only-api-openapi.yml
  format: yaml
  label: Eaton EV Only API
  slug: eaton-ev-only-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eaton/refs/heads/main/openapi/eaton-ev-only-api-openapi.yml
- filename: eaton-events-api-openapi.yml
  format: yaml
  label: Eaton Events API
  slug: eaton-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eaton/refs/heads/main/openapi/eaton-events-api-openapi.yml
- filename: eaton-locations-api-openapi.yml
  format: yaml
  label: Eaton Locations API
  slug: eaton-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eaton/refs/heads/main/openapi/eaton-locations-api-openapi.yml
- filename: eaton-organizations-api-openapi.yml
  format: yaml
  label: Eaton Organizations API
  slug: eaton-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eaton/refs/heads/main/openapi/eaton-organizations-api-openapi.yml
authorization_urls: []
description: ''
docs: https://api.em.eaton.com/docs
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Eaton Scopes
name_suffix: OAuth Scopes
note: Eaton's Smart Breaker API OAuth2 uses a scope-less client-credentials flow — tokens are issued from client ID + secret alongside an Em-Api-Subscription-Key header, with authorization governed by application/organization service accounts and user roles rather than documented OAuth scopes (https://api.em.eaton.com/docs).
overview: 'Eaton uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.em.eaton.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Eaton
provider_slug: eaton
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.em.eaton.com/oauth2/token
  name: OAuth2
  source: openapi/smart-breaker-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: eaton-scopes
source_filename: eaton-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/smart-breaker-openapi.yml\ndocs: https://api.em.eaton.com/docs\nnote: Eaton's Smart Breaker API OAuth2 uses a scope-less client-credentials flow — tokens are issued from client ID + secret alongside an Em-Api-Subscription-Key header, with authorization governed by application/organization service accounts and user roles rather than documented OAuth scopes (https://api.em.eaton.com/docs).\nschemes:\n- name: OAuth2\n  source: openapi/smart-breaker-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.em.eaton.com/oauth2/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eaton/refs/heads/main/scopes/eaton-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Power Management
- Electrical
- Smart Breaker
- EV Charging
- Demand Response
- Data Center
- DCIM
- PDU
- UPS
- Utility
- Industrial
- Building
- Mobility
- AI Factory
- Energy
- IoT
- Sustainability
token_urls:
- https://api.em.eaton.com/oauth2/token
---
