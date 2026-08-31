---
api_specs:
- filename: ntu-search-api-openapi.yml
  format: yaml
  label: DR-NTU (Data) — Dataverse API
  slug: ntu-drntu-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntu/refs/heads/main/openapi/ntu-search-api-openapi.yml
- filename: ntu-discover-api-openapi.yml
  format: yaml
  label: Nanyang Technological University Discover API
  slug: ntu-discover-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntu/refs/heads/main/openapi/ntu-discover-api-openapi.yml
- filename: ntu-items-api-openapi.yml
  format: yaml
  label: Nanyang Technological University Items API
  slug: ntu-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntu/refs/heads/main/openapi/ntu-items-api-openapi.yml
- filename: ntu-oai-pmh-api-openapi.yml
  format: yaml
  label: Nanyang Technological University OAI PMH API
  slug: ntu-oai-pmh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntu/refs/heads/main/openapi/ntu-oai-pmh-api-openapi.yml
- filename: ntu-root-api-openapi.yml
  format: yaml
  label: Nanyang Technological University Root API
  slug: ntu-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntu/refs/heads/main/openapi/ntu-root-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Ntu Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Nanyang Technological University uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Nanyang Technological University
provider_slug: ntu
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: ntu-scopes
source_filename: ntu-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "# ntu — authorization scopes.\ngenerated: '2026-08-19'\nmethod: probed\nsource: live probes 2026-08-19 of every NTU surface in this repo\nprovider: ntu\nscopes: []\nfinding: none\ndetail: >-\n  No scope-based authorization exists on any surface attributed to Nanyang Technological\n  University. The institution-operated DR-NTU (Data) Dataverse API uses a single opaque\n  X-Dataverse-key token with no scope vocabulary. The tenant DSpace-CRIS API uses a JWT bearer\n  token whose authorization is DSpace group membership, not scopes. The SGAF/eduGAIN SAML IdP\n  releases attributes, not OAuth scopes, and its attribute release policy is federation-side and\n  not published by NTU. There is no OAuth 2.0 or OIDC authorization server on any ntu.edu.sg host:\n  https://api.ntu.edu.sg/.well-known/openid-configuration returns 404.\nevidence:\n  - url: https://api.ntu.edu.sg/.well-known/openid-configuration\n    status: 404\n  - url: https://dr.ntu.edu.sg/server/api\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ntu/refs/heads/main/scopes/ntu-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- Singapore
- Public Research University
- Research Data
- Research Repository
- Identity Federation
- Open Access
- Course Catalog
- Library
- OAI-PMH
token_urls: []
---
