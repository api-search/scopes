---
api_specs:
- filename: ubc-access-api-openapi.yml
  format: yaml
  label: UBC Library Abacus Dataverse API
  slug: abacus-dataverse
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubc/refs/heads/main/openapi/ubc-access-api-openapi.yml
- filename: ubc-collections-api-openapi.yml
  format: yaml
  label: University of British Columbia Collections API
  slug: ubc-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubc/refs/heads/main/openapi/ubc-collections-api-openapi.yml
authorization_urls: []
description: UBC operates no OAuth-scoped API surface. Open Collections authorizes by API key and rate tier, Abacus Dataverse by API token and repository role, and the enterprise gateway at api.ubc.ca by an out-of-band Data Access Framework request. The one authorization vocabulary UBC does publish is SAML attribute release from its Shibboleth IdP, which is not a scope model and is not enumerated in the public metadata.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: none
name: Ubc Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'University of British Columbia uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: University of British Columbia
provider_slug: ubc
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: ubc-scopes
source_filename: ubc-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "---\nspecification: API Commons Scopes\nspecificationVersion: '0.1'\nprovider: University of British Columbia\nproviderId: ubc\ngenerated: '2026-08-19'\nmethod: none\nsource: >-\n  No OAuth 2.0 authorization server, scope registry or consent screen was found on any\n  UBC-operated host on 2026-08-19.\ndescription: >-\n  UBC operates no OAuth-scoped API surface. Open Collections authorizes by API key and rate\n  tier, Abacus Dataverse by API token and repository role, and the enterprise gateway at\n  api.ubc.ca by an out-of-band Data Access Framework request. The one authorization vocabulary\n  UBC does publish is SAML attribute release from its Shibboleth IdP, which is not a scope\n  model and is not enumerated in the public metadata.\nx-operator: institution\nscopes: []\nauthorizationModels:\n- surface: ubc:abacus-dataverse\n  model: role-based\n  detail: >-\n    Dataverse assigns roles (admin, curator, contributor, file downloader) at dataverse and\n    dataset level; the\
  \ contract exposes /api/v1/roles and /api/v1/access operations that read\n    and assign them. Roles are the closest thing to a scope vocabulary UBC exposes, and they\n    are Dataverse's model, not UBC's design.\n- surface: ubc:iec-api-gateway\n  model: out-of-band\n  detail: >-\n    Entitlement is granted per-API by UBC's Data Access Framework via a ServiceNow request.\n    There is no programmatic representation of what a caller is entitled to.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ubc/refs/heads/main/scopes/ubc-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Education
- Higher Education
- University
- Public Research University
- Canada
- British Columbia
- U15
- Library
- Digital Collections
- Research Data
- Research Repository
- Open Data
- Identity Federation
- OAI-PMH
- IIIF
- Dataverse
token_urls: []
---
