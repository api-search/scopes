---
api_specs:
- filename: newcastle-digitised-objects-api-openapi.yml
  format: yaml
  label: Digitised Objects Repository Search and Data API
  slug: digitised-objects
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle/refs/heads/main/openapi/newcastle-digitised-objects-api-openapi.yml
- filename: newcastle-entity-api-openapi.yml
  format: yaml
  label: Urban Observatory API (Urban Sciences Building) — Entity
  slug: urban-observatory-entity
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle/refs/heads/main/openapi/newcastle-entity-api-openapi.yml
- filename: newcastle-feed-api-openapi.yml
  format: yaml
  label: Urban Observatory API (Urban Sciences Building) — Feed
  slug: urban-observatory-feed
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle/refs/heads/main/openapi/newcastle-feed-api-openapi.yml
- filename: newcastle-summary-api-openapi.yml
  format: yaml
  label: Urban Observatory API (Urban Sciences Building) — Summary
  slug: urban-observatory-summary
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle/refs/heads/main/openapi/newcastle-summary-api-openapi.yml
- filename: newcastle-timeseries-api-openapi.yml
  format: yaml
  label: Urban Observatory API (Urban Sciences Building) — Timeseries
  slug: urban-observatory-timeseries
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle/refs/heads/main/openapi/newcastle-timeseries-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: derived
name: Newcastle Scopes
name_suffix: OAuth Scopes
note: No institution-operated Newcastle University API defines authorization scopes. The Digitised Objects Repository, the ECPPEC GraphQL API, the Urban Observatory API and the eTheses OAI-PMH endpoint are all open and unauthenticated, so there is nothing to scope. The one scoped authorization surface in the institution's footprint belongs to its Figshare tenant at data.ncl.ac.uk, and those scopes are Figshare's, defined in Figshare's contract — recording them here would credit Newcastle with a vendor's authorization design.
overview: 'Newcastle University uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Newcastle University
provider_slug: newcastle
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: newcastle-scopes
source_filename: newcastle-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "name: Newcastle University — authorization scopes\naid: newcastle\ngenerated: '2026-08-30'\nmethod: derived\nx-evidence-method: probed\nsource: live probes of Newcastle University operated hosts, 2026-08-30\nscopes: []\nnote: >-\n  No institution-operated Newcastle University API defines authorization scopes. The Digitised\n  Objects Repository, the ECPPEC GraphQL API, the Urban Observatory API and the eTheses OAI-PMH\n  endpoint are all open and unauthenticated, so there is nothing to scope. The one scoped\n  authorization surface in the institution's footprint belongs to its Figshare tenant at\n  data.ncl.ac.uk, and those scopes are Figshare's, defined in Figshare's contract — recording them\n  here would credit Newcastle with a vendor's authorization design.\nreleased_attributes:\n  note: >-\n    The nearest institution-operated analogue to a scope is SAML attribute release from the\n    Shibboleth IdP at gateway.ncl.ac.uk. Attribute release policy is not published in the\
  \ public\n    federation metadata, so no attribute list is asserted here.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newcastle/refs/heads/main/scopes/newcastle-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- United Kingdom
- Russell Group
- Research Data
- Open Data
- Digital Library
- Identity Federation
- Smart Cities
- Cultural Heritage
token_urls: []
---
