---
api_specs:
- filename: princeton-art-museum-api-openapi.yml
  format: yaml
  label: Princeton University Art Museum API
  slug: art-museum-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/openapi/princeton-art-museum-api-openapi.yml
- filename: princeton-article-api-openapi.yml
  format: yaml
  label: Princeton University Article API
  slug: princeton-article-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/openapi/princeton-article-api-openapi.yml
- filename: princeton-banner-api-openapi.yml
  format: yaml
  label: Princeton University Banner API
  slug: princeton-banner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/openapi/princeton-banner-api-openapi.yml
- filename: princeton-best-bets-api-openapi.yml
  format: yaml
  label: Princeton University Best Bets API
  slug: princeton-best-bets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/openapi/princeton-best-bets-api-openapi.yml
- filename: princeton-catalog-api-openapi.yml
  format: yaml
  label: Princeton University Catalog API
  slug: princeton-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/openapi/princeton-catalog-api-openapi.yml
- filename: princeton-dpul-api-openapi.yml
  format: yaml
  label: Princeton University Dpul API
  slug: princeton-dpul-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/openapi/princeton-dpul-api-openapi.yml
- filename: princeton-findingaids-api-openapi.yml
  format: yaml
  label: Princeton University Findingaids API
  slug: princeton-findingaids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/openapi/princeton-findingaids-api-openapi.yml
- filename: princeton-journals-api-openapi.yml
  format: yaml
  label: Princeton University Journals API
  slug: princeton-journals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/openapi/princeton-journals-api-openapi.yml
- filename: princeton-libanswers-api-openapi.yml
  format: yaml
  label: Princeton University Libanswers API
  slug: princeton-libanswers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/openapi/princeton-libanswers-api-openapi.yml
- filename: princeton-libguides-api-openapi.yml
  format: yaml
  label: Princeton University Libguides API
  slug: princeton-libguides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/openapi/princeton-libguides-api-openapi.yml
- filename: princeton-library-databases-api-openapi.yml
  format: yaml
  label: Princeton University Library Databases API
  slug: princeton-library-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/openapi/princeton-library-databases-api-openapi.yml
- filename: princeton-library-staff-api-openapi.yml
  format: yaml
  label: Princeton University Library Staff API
  slug: princeton-library-staff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/openapi/princeton-library-staff-api-openapi.yml
- filename: princeton-library-website-api-openapi.yml
  format: yaml
  label: Princeton University Library Website API
  slug: princeton-library-website-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/openapi/princeton-library-website-api-openapi.yml
- filename: princeton-makers-api-openapi.yml
  format: yaml
  label: Princeton University Makers API
  slug: princeton-makers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/openapi/princeton-makers-api-openapi.yml
- filename: princeton-objects-api-openapi.yml
  format: yaml
  label: Princeton University Objects API
  slug: princeton-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/openapi/princeton-objects-api-openapi.yml
- filename: princeton-packages-api-openapi.yml
  format: yaml
  label: Princeton University Packages API
  slug: princeton-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/openapi/princeton-packages-api-openapi.yml
- filename: princeton-pulmap-api-openapi.yml
  format: yaml
  label: Princeton University Pulmap API
  slug: princeton-pulmap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/openapi/princeton-pulmap-api-openapi.yml
- filename: princeton-search-api-openapi.yml
  format: yaml
  label: Princeton University Search API
  slug: princeton-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/openapi/princeton-search-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Princeton Scopes
name_suffix: OAuth Scopes
note: Princeton publishes no OAuth scope catalog. This file records that as a measured absence rather than leaving the slot empty and unexplained.
overview: 'Princeton University uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Princeton University
provider_slug: princeton
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: princeton-scopes
source_filename: princeton-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: >-\n  https://allsearch-api.princeton.edu/api-docs/v1/swagger.yaml and probes against\n  api.princeton.edu, 2026-08-19\nx-operator: institution\nnote: >-\n  Princeton publishes no OAuth scope catalog. This file records that as a measured absence rather\n  than leaving the slot empty and unexplained.\nsummary:\n  scopes_published: false\n  oauth2_flows_documented: []\n  authorization_model: >-\n    Two-state, not scoped. The Library's public APIs require nothing; the OIT gateway requires a\n    NetID or service-account subscription per API. Access is granted at the API-subscription level\n    inside WSO2 API Manager, so entitlement is per-API rather than per-scope, and the subscription\n    catalog is not published outside the campus network.\nscopes: []\nevidence:\n- url: https://allsearch-api.princeton.edu/api-docs/v1/swagger.yaml\n  status: 200\n  note: OpenAPI 3.1.1 with no components and no securitySchemes — nothing to scope.\n\
  - url: https://api.princeton.edu/active-directory/1.0.6/users\n  status: 401\n  note: Gateway rejects anonymous calls with an empty body and no WWW-Authenticate scope hint.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/scopes/princeton-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- Ivy League
- United States
- New Jersey
- Research Library
- Research Data
- Open Data
- Digital Collections
- Identity Federation
- Museum
token_urls: []
---
