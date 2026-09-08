---
api_specs:
- filename: university-of-minnesota-gems-exchange-soil-openapi.yml
  format: yaml
  label: GEMS Informatics Exchange APIs
  slug: gems-exchange-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-minnesota/refs/heads/main/openapi/university-of-minnesota-gems-exchange-soil-openapi.yml
- filename: university-of-minnesota-umedia-openapi.yml
  format: yaml
  label: UMedia Digital Collections JSON API
  slug: umedia-digital-collections
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-minnesota/refs/heads/main/openapi/university-of-minnesota-umedia-openapi.yml
authorization_urls: []
description: 'What authorization granularity the University''s programmable surfaces actually expose. Recorded including its absence: no University of Minnesota surface publishes an OAuth scope vocabulary, and pretending otherwise would credit the institution for a model it has not published.'
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: University Of Minnesota Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'University of Minnesota uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: University of Minnesota
provider_slug: university-of-minnesota
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: university-of-minnesota-scopes
source_filename: university-of-minnesota-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "---\nname: University of Minnesota — authorization scopes\ndescription: >-\n  What authorization granularity the University's programmable surfaces actually expose. Recorded\n  including its absence: no University of Minnesota surface publishes an OAuth scope vocabulary,\n  and pretending otherwise would credit the institution for a model it has not published.\ngenerated: '2026-09-01'\nmethod: probed\nsource: >-\n  Read from the nine live GEMS Exchange OpenAPI 3.1 documents in openapi/_original/ (none declare\n  components.securitySchemes or security[]), from the DSpace 10.0 HAL root at\n  conservancy.umn.edu/server/api, and from the Common Good API classification table published at\n  sites.google.com/umn.edu/integration-apis/common-good-apis.\noauth_scopes_published: false\nscopes: []\nauthorization_model:\n  - surface: GEMS Informatics Exchange APIs\n    model: opaque-api-key\n    granularity: per-key, per-API\n    detail: >-\n      Each of the ten Exchange APIs is a separate\
  \ deployment behind the same gateway and the key\n      is presented as an `apikey` header. No scope, role or claim vocabulary is published; the\n      contracts declare no security scheme at all.\n  - surface: Common Good APIs\n    model: data-classification-tiers\n    granularity: per-API, per-data-custodian\n    detail: >-\n      The University does not sell scopes here — it grades APIs by institutional data\n      classification and approves access per requester. The four published tiers are the closest\n      thing to a scope vocabulary the institution operates.\n    tiers:\n      - public\n      - private\n      - restricted\n      - highly restricted\n    evidence:\n      - url: https://sites.google.com/umn.edu/integration-apis/common-good-apis\n        status: 200\n  - surface: UMedia Digital Collections JSON API\n    model: anonymous-read\n    granularity: none\n    detail: Fully open read; there is nothing to scope.\n  - surface: UMN Digital Conservancy / DRUM\n    model: dspace-groups\n\
  \    granularity: collection and item level, via DSpace's own authorization model\n    detail: >-\n      Discovery is anonymous, item-level reads require authentication, and the group model is\n      DSpace's, not a University-authored one.\n  - surface: Institutional identity (Shibboleth IdP)\n    model: saml-attribute-release\n    granularity: per-service-provider attribute release, eduPerson attributes scoped to umn.edu\n    detail: >-\n      For the great majority of University systems this — not an OAuth scope — is the real\n      authorization surface, and it is the one the institution genuinely operates.\n    evidence:\n      - url: https://mdq.incommon.org/entities/urn%3Amace%3Aincommon%3Aumn.edu\n        status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-minnesota/refs/heads/main/scopes/university-of-minnesota-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- Research
- United States
- Minnesota
- Big Ten
- Land Grant
- Public Research University
- Research Data
- Research Repository
- Open Data
- Geospatial
- Agriculture
- Climate
- Digital Collections
- Identity Federation
- Research Computing
token_urls: []
---
