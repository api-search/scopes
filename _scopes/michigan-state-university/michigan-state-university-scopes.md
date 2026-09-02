---
api_specs:
- filename: michigan-state-university-record-api-openapi.yml
  format: yaml
  label: MSU Libraries Catalog Record API
  slug: michigan-state-university-record-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/michigan-state-university/refs/heads/main/openapi/michigan-state-university-record-api-openapi.yml
- filename: michigan-state-university-search-api-openapi.yml
  format: yaml
  label: MSU Libraries Catalog Search API
  slug: michigan-state-university-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/michigan-state-university/refs/heads/main/openapi/michigan-state-university-search-api-openapi.yml
authorization_urls: []
description: Michigan State University publishes NO authorization scopes. This artifact records that absence explicitly rather than leaving the reader to infer it, and describes the read surface each public operation actually exposes so an agent can reason about consequence without a scope vocabulary to lean on.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: derived
name: Michigan State University Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Michigan State University uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Michigan State University
provider_slug: michigan-state-university
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: michigan-state-university-scopes
source_filename: michigan-state-university-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "---\nspecification: API Commons Scopes\nspecificationVersion: '0.1'\nprovider: Michigan State University\nproviderId: michigan-state-university\ngenerated: '2026-08-30'\nmethod: derived\nsource: openapi/_original/michigan-state-university-catalog-rest.yaml\ndescription: >-\n  Michigan State University publishes NO authorization scopes. This artifact records that\n  absence explicitly rather than leaving the reader to infer it, and describes the read\n  surface each public operation actually exposes so an agent can reason about consequence\n  without a scope vocabulary to lean on.\ndeclared_scopes: []\ndeclared_scopes_note: >-\n  The published Library Catalog OpenAPI (v11.0.4) declares no components.securitySchemes,\n  therefore no oauth2 flows and no scopes. The Shibboleth IdP issues SAML attributes, not\n  OAuth scopes; attribute release is negotiated per service provider through InCommon and\n  is not published as a machine-readable scope list.\nimplied_read_surface:\n- name:\
  \ catalog.record.read\n  operations:\n  - GET /record\n  - GET /index2/record\n  - GET /web/record\n  consequence: read\n  data: Public bibliographic and web-page records from the library discovery index.\n  authorization: none — open to anonymous callers\n- name: catalog.search.read\n  operations:\n  - GET /search\n  - GET /index2/search\n  - GET /web/search\n  consequence: read\n  data: Public search results and facets over the library discovery index.\n  authorization: none — open to anonymous callers\n- name: metadata.harvest.read\n  operations:\n  - GET /OAI/Server?verb=*\n  - GET /oai?verb=*\n  consequence: read\n  data: Dublin Core, MARC21/MARCXML and MODS metadata records for harvesting.\n  authorization: none — open to anonymous harvesters\nwarning: >-\n  These names are OUR descriptive labels for reasoning about consequence. They are NOT\n  published by Michigan State University and must never be sent as scope values.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/michigan-state-university/refs/heads/main/scopes/michigan-state-university-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Education
- Higher Education
- University
- Public Research University
- Land-Grant University
- Big Ten
- United States
- Michigan
- Library
- Library Catalog
- Digital Repository
- Metadata
- OAI-PMH
- Identity Federation
- Shibboleth
- Research Computing
token_urls: []
---
