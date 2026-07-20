---
api_specs:
- filename: delivery-hero-on-demand-rider-openapi.json
  format: json
  label: Delivery Hero On Demand Rider API
  slug: delivery-hero-on-demand-rider
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delivery-hero/refs/heads/main/openapi/delivery-hero-on-demand-rider-openapi.json
authorization_urls: []
description: ''
docs: https://on-demand-rider-docs.deliveryhero.io/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Delivery Hero Scopes
name_suffix: OAuth Scopes
note: ODR OpenAPI declares only an apiKey Bearer scheme; OAuth2 client_credentials + scopes are documented in the auth guide, not the spec. Scopes are provisioned per client by ODR representatives.
overview: 'Delivery Hero publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the Delivery Hero API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Delivery Hero
provider_slug: delivery-hero
schemes:
- assertion: urn:ietf:params:oauth:client-assertion-type:jwt-bearer
  flow: clientCredentials
  name: OAuth2
  tokenUrl: https://sts.deliveryhero.io/oauth2/token
scope_count: 1
scope_names:
- pandago.api.sg.*
scopes:
- description: 'Documented example: full ODR API access for the Pandago brand in Singapore'
  flows:
  - clientCredentials
  scope: pandago.api.sg.*
slug: delivery-hero-scopes
source_filename: delivery-hero-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/delivery-hero-on-demand-rider-openapi.json\ndocs: https://on-demand-rider-docs.deliveryhero.io/\nnote: ODR OpenAPI declares only an apiKey Bearer scheme; OAuth2 client_credentials\n  + scopes are documented in the auth guide, not the spec. Scopes are provisioned\n  per client by ODR representatives.\nschemes:\n- name: OAuth2\n  flow: clientCredentials\n  tokenUrl: https://sts.deliveryhero.io/oauth2/token\n  assertion: urn:ietf:params:oauth:client-assertion-type:jwt-bearer\nscope_pattern: '{brand}.api.{country_code}.*'\nscopes:\n- scope: pandago.api.sg.*\n  description: 'Documented example: full ODR API access for the Pandago brand in Singapore'\n  flows:\n  - clientCredentials\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/delivery-hero/refs/heads/main/scopes/delivery-hero-scopes.yml
summary_line: 1 scope
tags:
- Company
- Technology
- Food Delivery
- Logistics
- Quick Commerce
- Last Mile Delivery
- On Demand
- Orders
token_urls: []
---
