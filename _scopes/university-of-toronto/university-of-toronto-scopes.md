---
api_specs:
- filename: university-of-toronto-courses-api-openapi.yml
  format: yaml
  label: University of Toronto Courses API
  slug: university-of-toronto-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-toronto/refs/heads/main/openapi/university-of-toronto-courses-api-openapi.yml
- filename: university-of-toronto-reference-data-api-openapi.yml
  format: yaml
  label: University of Toronto Reference Data API
  slug: university-of-toronto-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-toronto/refs/heads/main/openapi/university-of-toronto-reference-data-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: University Of Toronto Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'University of Toronto uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: University of Toronto
provider_slug: university-of-toronto
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: university-of-toronto-scopes
source_filename: university-of-toronto-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "---\ngenerated: '2026-08-19'\nmethod: probed\nsource: >-\n  Live probing of every institution-operated surface on 2026-08-19. Nothing here was inferred from a\n  vendor's generic scope vocabulary.\nx-operator: institution\nsummary: >-\n  The University of Toronto publishes no OAuth scopes, because it publishes no OAuth authorization\n  server. This artifact records that absence explicitly rather than borrowing a vendor's scope list.\nscopes: []\nfindings:\n  - surface: university-of-toronto:ttb-course-timetable\n    x-operator: institution\n    authorization_model: none\n    detail: >-\n      Every operation is unauthenticated and returns the same data to every caller. There is no\n      per-caller partitioning to scope.\n  - surface: university-of-toronto:utorauth-shibboleth-idp\n    x-operator: institution\n    authorization_model: SAML attribute release\n    detail: >-\n      The nearest analogue to a scope on U of T's surface is the SAML attribute bundle released to a\n\
  \      service provider, governed by the REFEDS Research & Scholarship entity category asserted in\n      the IdP metadata. R&S implies release of person identifier, name, email and affiliation. This\n      is an attribute-release policy, not an OAuth scope, and it is not enumerated per-SP in public\n      metadata.\n  - surface: university-of-toronto:tspace-dspace-rest\n    x-operator: tenant\n    authorization_model: vendor-defined\n    detail: >-\n      DSpace 8 authorization is the Scholaris platform's. Any scope vocabulary belongs to DSpace and\n      is not attributable to the University of Toronto.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-toronto/refs/heads/main/scopes/university-of-toronto-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- Canada
- U15
- Research
- Course Catalog
- Identity Federation
- Research Data
- Institutional Repository
- Library
- Public Research University
token_urls: []
---
