---
api_specs:
- filename: university-of-leeds-facets-api-openapi.yml
  format: yaml
  label: University of Leeds Facets API
  slug: university-of-leeds-facets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-leeds/refs/heads/main/openapi/university-of-leeds-facets-api-openapi.yml
- filename: university-of-leeds-iiif-image-api-openapi.yml
  format: yaml
  label: University of Leeds IIIF Image API
  slug: university-of-leeds-iiif-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-leeds/refs/heads/main/openapi/university-of-leeds-iiif-image-api-openapi.yml
- filename: university-of-leeds-oai-pmh-api-openapi.yml
  format: yaml
  label: University of Leeds OAI PMH API
  slug: university-of-leeds-oai-pmh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-leeds/refs/heads/main/openapi/university-of-leeds-oai-pmh-api-openapi.yml
- filename: university-of-leeds-spaces-api-openapi.yml
  format: yaml
  label: University of Leeds Spaces API
  slug: university-of-leeds-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-leeds/refs/heads/main/openapi/university-of-leeds-spaces-api-openapi.yml
- filename: university-of-leeds-open-search-api-openapi.yml
  format: yaml
  label: University of Leeds Open Search API
  slug: university-of-leeds-open-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-leeds/refs/heads/main/openapi/university-of-leeds-open-search-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: derived
name: University Of Leeds Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'University of Leeds uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: University of Leeds
provider_slug: university-of-leeds
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: university-of-leeds-scopes
source_filename: university-of-leeds-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "scopes_version: '0.1'\nprovider: university-of-leeds\ngenerated: '2026-08-30'\nmethod: derived\nevidence_method: probed\nprobed: '2026-08-30'\nx-operator: institution\nsource: >-\n  Determined by probing every institution-operated surface unauthenticated on 2026-08-30 and finding\n  no authorization layer to scope.\nscopes: []\ndetail: >-\n  NONE, and this is a finding rather than a gap. All four institution-operated surfaces are anonymous\n  read-only (see authentication/). With no credential there is no authorization boundary and\n  therefore no scope vocabulary to publish. Scopes would only become meaningful if Leeds put a key\n  or an OAuth flow in front of these endpoints. The one surface that DOES carry scopes — Ex Libris\n  Alma/Primo — is vendor-operated under a tenancy, and its scope model belongs in the Ex Libris\n  profile, not this one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-leeds/refs/heads/main/scopes/university-of-leeds-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- United Kingdom
- Russell Group
- Research Data
- Research Repository
- Library
- Open Data
- OAI-PMH
- IIIF
- Research Computing
- Digital Collections
token_urls: []
---
