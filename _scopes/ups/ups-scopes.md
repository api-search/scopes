---
api_specs:
- filename: ups-address-validation-api-openapi.yml
  format: yaml
  label: UPS Address Validation API
  slug: ups-address-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ups/refs/heads/main/openapi/ups-address-validation-api-openapi.yml
- filename: ups-paperless-documents-api-openapi.yml
  format: yaml
  label: UPS Paperless Documents API
  slug: ups-paperless-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ups/refs/heads/main/openapi/ups-paperless-documents-api-openapi.yml
- filename: ups-pickup-api-openapi.yml
  format: yaml
  label: UPS Pickup API
  slug: ups-pickup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ups/refs/heads/main/openapi/ups-pickup-api-openapi.yml
- filename: ups-rating-api-openapi.yml
  format: yaml
  label: UPS Rating API
  slug: ups-rating-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ups/refs/heads/main/openapi/ups-rating-api-openapi.yml
- filename: ups-shipping-api-openapi.yml
  format: yaml
  label: UPS Shipping API
  slug: ups-shipping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ups/refs/heads/main/openapi/ups-shipping-api-openapi.yml
- filename: ups-time-in-transit-api-openapi.yml
  format: yaml
  label: UPS Time In Transit API
  slug: ups-time-in-transit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ups/refs/heads/main/openapi/ups-time-in-transit-api-openapi.yml
- filename: ups-tracking-api-openapi.yml
  format: yaml
  label: UPS Tracking API
  slug: ups-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ups/refs/heads/main/openapi/ups-tracking-api-openapi.yml
- filename: ups-oauth-api-openapi.yml
  format: yaml
  label: UPS O Auth API
  slug: ups-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ups/refs/heads/main/openapi/ups-oauth-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Ups Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'UPS uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://onlinetools.ups.com/api/security/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: UPS
provider_slug: ups
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://onlinetools.ups.com/api/security/v1/oauth/token
  name: OAuth2
  source: openapi/ups-address-validation-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://onlinetools.ups.com/api/security/v1/oauth/token
  name: OAuth2
  source: openapi/ups-oauth-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://onlinetools.ups.com/api/security/v1/oauth/token
  name: OAuth2
  source: openapi/ups-paperless-documents-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://onlinetools.ups.com/api/security/v1/oauth/token
  name: OAuth2
  source: openapi/ups-pickup-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://onlinetools.ups.com/api/security/v1/oauth/token
  name: OAuth2
  source: openapi/ups-rating-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://onlinetools.ups.com/api/security/v1/oauth/token
  name: OAuth2
  source: openapi/ups-shipping-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://onlinetools.ups.com/api/security/v1/oauth/token
  name: OAuth2
  source: openapi/ups-time-in-transit-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://onlinetools.ups.com/api/security/v1/oauth/token
  name: OAuth2
  source: openapi/ups-tracking-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: ups-scopes
source_filename: ups-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/ups-address-validation-api-openapi.yml, openapi/ups-oauth-api-openapi.yml, openapi/ups-paperless-documents-api-openapi.yml,\n  openapi/ups-pickup-api-openapi.yml, openapi/ups-rating-api-openapi.yml, openapi/ups-shipping-api-openapi.yml,\n  openapi/ups-time-in-transit-api-openapi.yml, openapi/ups-tracking-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/ups-address-validation-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://onlinetools.ups.com/api/security/v1/oauth/token\n- name: OAuth2\n  source: openapi/ups-oauth-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://onlinetools.ups.com/api/security/v1/oauth/token\n- name: OAuth2\n  source: openapi/ups-paperless-documents-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://onlinetools.ups.com/api/security/v1/oauth/token\n- name: OAuth2\n  source: openapi/ups-pickup-api-openapi.yml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://onlinetools.ups.com/api/security/v1/oauth/token\n- name: OAuth2\n  source: openapi/ups-rating-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://onlinetools.ups.com/api/security/v1/oauth/token\n- name: OAuth2\n  source: openapi/ups-shipping-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://onlinetools.ups.com/api/security/v1/oauth/token\n- name: OAuth2\n  source: openapi/ups-time-in-transit-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://onlinetools.ups.com/api/security/v1/oauth/token\n- name: OAuth2\n  source: openapi/ups-tracking-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://onlinetools.ups.com/api/security/v1/oauth/token\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ups/refs/heads/main/scopes/ups-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Logistics
- Shipping
- Fortune 500
- Supply Chain
token_bound: false
token_urls:
- https://onlinetools.ups.com/api/security/v1/oauth/token
---
