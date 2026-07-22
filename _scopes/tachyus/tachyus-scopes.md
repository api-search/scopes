---
api_specs:
- filename: tachyus-tachapps-openapi.yml
  format: yaml
  label: Tachapps API
  slug: tachapps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tachyus/refs/heads/main/openapi/tachyus-tachapps-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.tachyus.com/api/authentication.html
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Tachyus Scopes
name_suffix: OAuth Scopes
note: Scopes are assigned to API tokens (Bearer personal-access-token model), not granted via OAuth2 authorization flows. Listed verbatim from the Tachapps authentication reference.
overview: 'Tachyus publishes 6 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Tachyus API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Tachyus
provider_slug: tachyus
schemes: []
scope_count: 6
scope_names:
- read:projects
- read:wells
- read:production
- write:projects
- write:wells
- admin
scopes:
- description: List and read projects
  flows: []
  scope: read:projects
- description: List and read wells
  flows: []
  scope: read:wells
- description: Read production data
  flows: []
  scope: read:production
- description: Create and update projects
  flows: []
  scope: write:projects
- description: Create and update wells
  flows: []
  scope: write:wells
- description: Full access
  flows: []
  scope: admin
slug: tachyus-scopes
source_filename: tachyus-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.tachyus.com/api/authentication.html\ndocs: https://docs.tachyus.com/api/authentication.html\nmodel: token-scopes\nnote: >-\n  Scopes are assigned to API tokens (Bearer personal-access-token model), not\n  granted via OAuth2 authorization flows. Listed verbatim from the Tachapps\n  authentication reference.\nscopes:\n  - scope: read:projects\n    description: List and read projects\n  - scope: read:wells\n    description: List and read wells\n  - scope: read:production\n    description: Read production data\n  - scope: write:projects\n    description: Create and update projects\n  - scope: write:wells\n    description: Create and update wells\n  - scope: admin\n    description: Full access\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tachyus/refs/heads/main/scopes/tachyus-scopes.yml
summary_line: 6 scopes
tags:
- Company
- Energy
- Oil and Gas
- Reservoir Management
- Production Optimization
- Emissions Management
- Machine Learning
- Analytics
token_urls: []
---
