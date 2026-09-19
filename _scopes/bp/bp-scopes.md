---
api_specs:
- filename: bp-cards-api-openapi.yml
  format: yaml
  label: BP Cards API
  slug: bp-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bp/refs/heads/main/openapi/bp-cards-api-openapi.yml
- filename: bp-fueling-api-openapi.yml
  format: yaml
  label: BP Fueling API
  slug: bp-fueling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bp/refs/heads/main/openapi/bp-fueling-api-openapi.yml
- filename: bp-openapiinvoices-api-openapi.yml
  format: yaml
  label: BP Open API Invoices API
  slug: bp-openapiinvoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bp/refs/heads/main/openapi/bp-openapiinvoices-api-openapi.yml
- filename: bp-openapitransactions-api-openapi.yml
  format: yaml
  label: BP Open API Transactions API
  slug: bp-openapitransactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bp/refs/heads/main/openapi/bp-openapitransactions-api-openapi.yml
- filename: bp-sitediscovery-api-openapi.yml
  format: yaml
  label: BP Site Discovery API
  slug: bp-sitediscovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bp/refs/heads/main/openapi/bp-sitediscovery-api-openapi.yml
- filename: bp-token-api-openapi.yml
  format: yaml
  label: BP Token API
  slug: bp-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bp/refs/heads/main/openapi/bp-token-api-openapi.yml
- filename: bp-health-check-api-openapi.yml
  format: yaml
  label: BP Health Check API
  slug: bp-health-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bp/refs/heads/main/openapi/bp-health-check-api-openapi.yml
- filename: bp-payment-method-api-openapi.yml
  format: yaml
  label: BP Payment Method API
  slug: bp-payment-method-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bp/refs/heads/main/openapi/bp-payment-method-api-openapi.yml
authorization_urls: []
description: OAuth scopes advertised by BP's B2B identity host (b2bid.bp.com, ForgeRock AM), which is the authorization server behind the bp Open Fleet developer portal. These are the scopes the authorization server itself publishes as supported.
docs: https://developer.fleet.bp.com/DE/getting-started
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Bp Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'BP uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: BP
provider_slug: bp
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: bp-scopes
source_filename: bp-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: https://b2bid.bp.com/.well-known/openid-configuration (fetched, HTTP 200)\nprovider: BP\nproviderId: bp\ndocs: https://developer.fleet.bp.com/DE/getting-started\ndescription: >-\n  OAuth scopes advertised by BP's B2B identity host (b2bid.bp.com, ForgeRock AM), which is the\n  authorization server behind the bp Open Fleet developer portal. These are the scopes the\n  authorization server itself publishes as supported.\nauthorization_server: https://b2bid.bp.com/am/oauth2\nscopes:\n  - name: openid\n    description: Standard OpenID Connect scope; requests an ID token.\n    standard: true\n  - name: profile\n    description: Standard OIDC profile claims.\n    standard: true\n  - name: email\n    description: Standard OIDC email claims.\n    standard: true\n  - name: phone\n    description: Standard OIDC phone claims.\n    standard: true\n  - name: b2b-profile\n    description: BP-specific scope carrying the B2B business-account\
  \ profile.\n    standard: false\n  - name: b2b-consent\n    description: BP-specific scope covering B2B consent state for the authenticated business user.\n    standard: false\nclaims_supported:\n  - sub\n  - email\n  - email_verified\n  - phone\n  - phone_verified\n  - nickname\n  - locale\n  - appname\n  - subname\n  - external_id\n  - custom_username\n  - passwordless\nnotes:\n  - >-\n    The six bp Open Fleet resource OpenAPIs declare a bearer securityScheme with NO oauth2\n    scopes block, so no per-operation scope requirements are published. The scopes above govern\n    the portal sign-in flow, not fine-grained API authorization.\n  - >-\n    Authorization for the resource APIs is instead scoped by the credential's environment\n    (sandbox vs production) and by the AuthorityIds / ParentIds the caller may query.\nmaintainers:\n  - FN: Kin Lane\n    email: info@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bp/refs/heads/main/scopes/bp-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Energy
- Oil
- Gas
- Renewables
- Developer Platform
- Fleet
- Fuel Cards
- Mobility
- Retail Fuel
- EV Charging
token_urls: []
---
