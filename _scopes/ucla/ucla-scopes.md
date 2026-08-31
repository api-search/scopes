---
api_specs:
- filename: ucla-class-sections-api-openapi.yml
  format: yaml
  label: University of California, Los Angeles Class Sections API
  slug: ucla-class-sections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucla/refs/heads/main/openapi/ucla-class-sections-api-openapi.yml
- filename: ucla-classes-api-openapi.yml
  format: yaml
  label: University of California, Los Angeles Classes API
  slug: ucla-classes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucla/refs/heads/main/openapi/ucla-classes-api-openapi.yml
- filename: ucla-courses-api-openapi.yml
  format: yaml
  label: University of California, Los Angeles Courses API
  slug: ucla-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucla/refs/heads/main/openapi/ucla-courses-api-openapi.yml
- filename: ucla-dictionary-api-openapi.yml
  format: yaml
  label: University of California, Los Angeles Dictionary API
  slug: ucla-dictionary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucla/refs/heads/main/openapi/ucla-dictionary-api-openapi.yml
- filename: ucla-ge-foundations-api-openapi.yml
  format: yaml
  label: University of California, Los Angeles GE Foundations API
  slug: ucla-ge-foundations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucla/refs/heads/main/openapi/ucla-ge-foundations-api-openapi.yml
- filename: ucla-infrastructure-api-openapi.yml
  format: yaml
  label: University of California, Los Angeles Infrastructure API
  slug: ucla-infrastructure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucla/refs/heads/main/openapi/ucla-infrastructure-api-openapi.yml
- filename: ucla-myucla-api-openapi.yml
  format: yaml
  label: University of California, Los Angeles My UCLA API
  slug: ucla-myucla-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucla/refs/heads/main/openapi/ucla-myucla-api-openapi.yml
- filename: ucla-production-calendar-jobs-api-openapi.yml
  format: yaml
  label: University of California, Los Angeles Production Calendar Jobs API
  slug: ucla-production-calendar-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucla/refs/heads/main/openapi/ucla-production-calendar-jobs-api-openapi.yml
- filename: ucla-weather-api-openapi.yml
  format: yaml
  label: University of California, Los Angeles Weather API
  slug: ucla-weather-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucla/refs/heads/main/openapi/ucla-weather-api-openapi.yml
authorization_urls: []
description: The complete authorization vocabulary UCLA's own API gateway advertises. It is two words. Every one of the six SIS contracts declares the same OAuth 2.0 application flow with the same two scopes, and no contract requests anything narrower than `read` on any operation. This is recorded exactly as found rather than elaborated - a two-scope model across a student information system is the finding.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Ucla Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'University of California, Los Angeles uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: University of California, Los Angeles
provider_slug: ucla
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: ucla-scopes
source_filename: ucla-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: >-\n  securityDefinitions.application.scopes read verbatim from the six Swagger 2.0 SIS contracts,\n  and components.securitySchemes.ApiKeyAuth from the OpenAPI 3.0.3 UCLA Weather contract, all\n  published at https://developer.api.ucla.edu/sites/default/files/apidoc_specs/ (HTTP 200,\n  fetched 2026-08-19)\nprovider: University of California, Los Angeles\nproviderId: ucla\nx-operator: institution\nauthorization_server: https://api.ucla.edu/oauth/client_credential/accesstoken\ndescription: >-\n  The complete authorization vocabulary UCLA's own API gateway advertises. It is two words.\n  Every one of the six SIS contracts declares the same OAuth 2.0 application flow with the same\n  two scopes, and no contract requests anything narrower than `read` on any operation. This is\n  recorded exactly as found rather than elaborated - a two-scope model across a student\n  information system is the finding.\nscopes:\n- name: read\n  standard:\
  \ false\n  x-operator: institution\n  description: >-\n    \"Read access to protected resources\", verbatim from the contract. Requested by every\n    operation in all six SIS contracts, including the entire 61-operation Registrar data\n    dictionary and every class, class-section and course-detail route.\n  declared_in:\n  - openapi/_original/ucla-sis-classes-openapi.yml\n  - openapi/_original/ucla-sis-courses-openapi.yml\n  - openapi/_original/ucla-sis-dictionary-openapi.yml\n  - openapi/_original/ucla-sis-production-calendar-jobs-openapi.yml\n  - openapi/_original/ucla-sis-verify-connectivity-openapi.yml\n  - openapi/_original/ucla-myucla-menu-data-openapi.yml\n- name: write\n  standard: false\n  x-operator: institution\n  description: >-\n    \"Write access to protected resources\", verbatim from the contract. Declared in all six SIS\n    contracts even though every operation in all six is an HTTP GET. Nothing published on the\n    portal exercises it, so it is either aspirational\
  \ or reserved for products that are only\n    visible after campus sign-in.\n  declared_in:\n  - openapi/_original/ucla-sis-classes-openapi.yml\n  - openapi/_original/ucla-sis-courses-openapi.yml\n  - openapi/_original/ucla-sis-dictionary-openapi.yml\n  - openapi/_original/ucla-sis-production-calendar-jobs-openapi.yml\n  - openapi/_original/ucla-sis-verify-connectivity-openapi.yml\n  - openapi/_original/ucla-myucla-menu-data-openapi.yml\nnon_scoped_credentials:\n- name: x-apikey\n  surface: UCLA Weather API\n  x-operator: institution\n  description: >-\n    The UCLA Weather contract uses a header API key with no scope model at all. Fourteen\n    read-only operations, one credential, no partition.\naccess_boundary: >-\n  The real authorization boundary at UCLA is not the token scope - it is the API Product an\n  application is subscribed to, approved per product by the owning campus unit through the\n  developer portal. The scope vocabulary is coarse on purpose because the product bundle\
  \ is\n  where the decision is made. That decision is not machine-readable anywhere public.\ngaps:\n- No per-resource or per-domain scope (nothing like sis.classes.read).\n- No scope documentation outside the contracts themselves.\n- No OpenID Connect discovery document on the gateway, so scopes_supported cannot be discovered.\n- write is declared on six read-only contracts.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ucla/refs/heads/main/scopes/ucla-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- United States
- California
- UC System
- Public Research University
- Course Catalog
- Student Information
- Identity Federation
- Research Repository
- Library
- IIIF
- Campus Life
token_urls: []
---
