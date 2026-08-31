---
api_specs:
- filename: ucsf-documents-api-openapi.yml
  format: yaml
  label: University of California, San Francisco Documents API
  slug: ucsf-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsf/refs/heads/main/openapi/ucsf-documents-api-openapi.yml
- filename: ucsf-profiles-api-openapi.yml
  format: yaml
  label: University of California, San Francisco Profiles API
  slug: ucsf-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsf/refs/heads/main/openapi/ucsf-profiles-api-openapi.yml
authorization_urls: []
description: Authorization scopes across UCSF's institution-operated public surfaces.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Ucsf Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'University of California, San Francisco uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: University of California, San Francisco
provider_slug: ucsf
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: ucsf-scopes
source_filename: ucsf-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "name: UCSF API Scopes\ndescription: >-\n  Authorization scopes across UCSF's institution-operated public surfaces.\ngenerated: '2026-08-19'\nmethod: probed\nsource:\n  - https://profilesdeveloper.ucsf.edu/json-api\n  - https://solr.idl.ucsf.edu/solr/ltdl3/query?q=*:*&rows=0&wt=json\nscopes: []\nfinding: >-\n  No scope system exists on either institution-operated public API. Both the UCSF Profiles JSON\n  API and the UCSF Industry Documents Library Solr API are anonymous, read-only, and undifferentiated\n  — every caller sees exactly the same corpus, and there is no token, consent screen, or permission\n  boundary to describe. This is an accurate absence, not a gap in the research: a public archive\n  and a public directory of researchers have nothing to scope. Scoped authorization at UCSF lives\n  behind the SAML identity provider (urn:mace:incommon:ucsf.edu) and behind the gated\n  unified-api.ucsf.edu gateway, neither of which publishes a machine-readable scope inventory.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ucsf/refs/heads/main/scopes/ucsf-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- United States
- California
- UC System
- Public Research University
- Health Sciences
- Research
- Researcher Profiles
- Research Data
- Open Data
- Library
- Digital Archive
- Identity Federation
- Research Computing
token_urls: []
---
