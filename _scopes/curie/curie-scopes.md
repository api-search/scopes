---
api_specs:
- filename: curie-openapi.json
  format: json
  label: Curie 3D Product Commerce API
  slug: curie-3d-product-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curie/refs/heads/main/openapi/curie-openapi.json
authorization_urls:
- https://chat.curie.app/api/oauth/authorize
description: ''
docs: https://chat.curie.app/llms.txt
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Curie Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Curie publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Curie API on a user''s behalf.


  Tokens are issued from https://chat.curie.app/api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Curie
provider_slug: curie
schemes:
- description: OAuth 2.0 authorization code flow. Requires Curie Pro subscription.
  flows:
  - authorizationUrl: https://chat.curie.app/api/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://chat.curie.app/api/oauth/token
  name: oauth2
  source: openapi/curie-openapi.json
scope_count: 1
scope_names:
- read:products
scopes:
- description: Search and view products in the catalog
  flows:
  - authorizationCode
  scope: read:products
slug: curie-scopes
source_filename: curie-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/curie-openapi.json\ndocs: https://chat.curie.app/llms.txt\nschemes:\n- name: oauth2\n  source: openapi/curie-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://chat.curie.app/api/oauth/authorize\n    tokenUrl: https://chat.curie.app/api/oauth/token\n  description: OAuth 2.0 authorization code flow. Requires Curie Pro subscription.\nscopes:\n- scope: read:products\n  description: Search and view products in the catalog\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/curie-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curie/refs/heads/main/scopes/curie-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Commerce
- E-Commerce
- Shopify
- Artificial Intelligence
- Model Context Protocol
- Agentic Commerce
- Product Discovery
- 3D
token_urls:
- https://chat.curie.app/api/oauth/token
---
