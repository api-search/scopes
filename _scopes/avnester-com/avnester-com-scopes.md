---
api_specs:
- filename: avnester-com-public-api-openapi.yml
  format: yaml
  label: AVnester Public API
  slug: avnester-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/avnester-com/openapi/avnester-com-public-api-openapi.yml
authorization_urls:
- https://auth.avnester.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Avnester Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'AVnester publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the AVnester API on a user''s behalf.


  Tokens are issued from https://auth.avnester.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AVnester
provider_slug: avnester-com
schemes:
- flows:
  - authorizationUrl: https://auth.avnester.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://auth.avnester.com/oauth/token
  name: oauth2
  source: openapi/avnester-com-openapi.json
scope_count: 3
scope_names:
- calculators:use
- listings:read:public
- locality:read:public
scopes:
- description: Use deterministic real-estate calculators.
  flows:
  - authorizationCode
  scope: calculators:use
- description: Read public real-estate listing data.
  flows:
  - authorizationCode
  scope: listings:read:public
- description: Read public locality insights and comparisons.
  flows:
  - authorizationCode
  scope: locality:read:public
slug: avnester-com-scopes
source_filename: avnester-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: openapi/avnester-com-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/avnester-com-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.avnester.com/oauth/authorize\n    tokenUrl: https://auth.avnester.com/oauth/token\nscopes:\n- scope: calculators:use\n  description: Use deterministic real-estate calculators.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/avnester-com-openapi.json\n- scope: listings:read:public\n  description: Read public real-estate listing data.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/avnester-com-openapi.json\n- scope: locality:read:public\n  description: Read public locality insights and comparisons.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/avnester-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/avnester-com/scopes/avnester-com-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Real Estate
- Artificial Intelligence
- Property Listings
- India
- Marketplace
token_bound: false
token_urls:
- https://auth.avnester.com/oauth/token
---
