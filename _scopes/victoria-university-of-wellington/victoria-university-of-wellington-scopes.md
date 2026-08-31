---
api_specs:
- filename: victoria-university-of-wellington-website-globalobject-openapi.yml
  format: yaml
  label: Website Global Object
  slug: website-global-object
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/victoria-university-of-wellington/refs/heads/main/openapi/victoria-university-of-wellington-website-globalobject-openapi.yml
- filename: victoria-university-of-wellington-identity-federation-openapi.yml
  format: yaml
  label: Shibboleth Identity Provider (Tuakiri / eduGAIN)
  slug: identity-federation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/victoria-university-of-wellington/refs/heads/main/openapi/victoria-university-of-wellington-identity-federation-openapi.yml
- filename: victoria-university-of-wellington-institutional-repository-openapi.yml
  format: yaml
  label: Institutional Repository (self-hosted DSpace)
  slug: institutional-repository
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/victoria-university-of-wellington/refs/heads/main/openapi/victoria-university-of-wellington-institutional-repository-openapi.yml
authorization_urls: []
description: 'Scope inventory for Te Herenga Waka—Victoria University of Wellington. The institution defines no OAuth scopes of its own: neither institution-operated surface is authenticated, so neither has scopes to define. The only scoping vocabulary the institution genuinely authors is its SAML attribute release, which is the identity-federation equivalent and is recorded here rather than left blank.'
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: derived
name: Victoria University Of Wellington Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Victoria University of Wellington uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Victoria University of Wellington
provider_slug: victoria-university-of-wellington
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: victoria-university-of-wellington-scopes
source_filename: victoria-university-of-wellington-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "specification: API Commons Scopes\nspecificationVersion: '0.1'\nprovider: Victoria University of Wellington\nproviderId: victoria-university-of-wellington\ngenerated: '2026-08-30'\nmethod: derived\nprobe_date: '2026-08-30'\nprobe_note: >-\n  Written by API Evangelist from live, unauthenticated probes. Every status code and payload\n  quoted below was observed on the date above; nothing here was published by the institution.\nsource: live probes, 2026-08-30\ndescription: >-\n  Scope inventory for Te Herenga Waka—Victoria University of Wellington. The institution defines no\n  OAuth scopes of its own: neither institution-operated surface is authenticated, so neither has\n  scopes to define. The only scoping vocabulary the institution genuinely authors is its SAML\n  attribute release, which is the identity-federation equivalent and is recorded here rather than\n  left blank.\noauth_scopes: []\nsaml_attribute_release:\n  operator: institution\n  entity_id: https://idp.vuw.ac.nz/idp/shibboleth\n\
  \  scope: vuw.ac.nz\n  entity_categories:\n  - http://refeds.org/category/research-and-scholarship\n  assurance:\n  - https://refeds.org/sirtfi\n  requested_attributes:\n  - friendly_name: mail\n    oid: urn:oid:0.9.2342.19200300.100.1.3\n  - friendly_name: schacHomeOrganization\n    oid: urn:oid:1.3.6.1.4.1.25178.1.2.9\n  - friendly_name: schacHomeOrganizationType\n    oid: urn:oid:1.3.6.1.4.1.25178.1.2.10\n  - friendly_name: auEduPersonSharedToken\n    oid: urn:oid:1.3.6.1.4.1.27856.1.2.5\n  evidence:\n    url: https://directory.tuakiri.ac.nz/metadata/tuakiri-metadata-signed.xml\n    status: 200\nnotes: >-\n  Tenant surfaces (Canvas, Symplectic Elements, Entra ID) carry their vendors' scope vocabularies,\n  not the university's, and are deliberately not restated here.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/victoria-university-of-wellington/refs/heads/main/scopes/victoria-university-of-wellington-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- New Zealand
- Public Research University
- Research
- Open Access
- Research Repository
- Institutional Repository
- OAI-PMH
- DSpace
- Library
- Course Catalog
- Identity Federation
- Research Computing
token_urls: []
---
