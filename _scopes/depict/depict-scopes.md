---
api_specs:
- filename: depict-storefront-openapi-original.json
  format: json
  label: Depict Storefront API
  slug: depict-storefront-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/depict/refs/heads/main/openapi/depict-storefront-openapi-original.json
- filename: depict-portal-openapi-original.json
  format: json
  label: Depict Portal API
  slug: depict-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/depict/refs/heads/main/openapi/depict-portal-openapi-original.json
- filename: depict-lite-openapi-original.json
  format: json
  label: Depict Lite API
  slug: depict-lite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/depict/refs/heads/main/openapi/depict-lite-openapi-original.json
authorization_urls:
- https://depict.eu.auth0.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Depict Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Depict publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Depict API on a user''s behalf.


  Tokens are issued from https://depict.eu.auth0.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Depict
provider_slug: depict
schemes:
- flows:
  - authorizationUrl: https://depict.eu.auth0.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://depict.eu.auth0.com/oauth/token
  name: Auth0
  source: openapi/depict-lite-openapi-original.json
- flows:
  - authorizationUrl: https://depict.eu.auth0.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://depict.eu.auth0.com/oauth/token
  name: Auth0
  source: openapi/depict-portal-openapi-original.json
scope_count: 3
scope_names:
- email
- openid
- profile
scopes:
- description: User email
  flows:
  - authorizationCode
  scope: email
- description: OpenID Connect
  flows:
  - authorizationCode
  scope: openid
- description: User profile
  flows:
  - authorizationCode
  scope: profile
slug: depict-scopes
source_filename: depict-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/depict-lite-openapi-original.json, openapi/depict-portal-openapi-original.json\nschemes:\n- name: Auth0\n  source: openapi/depict-lite-openapi-original.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://depict.eu.auth0.com/oauth/authorize\n    tokenUrl: https://depict.eu.auth0.com/oauth/token\n- name: Auth0\n  source: openapi/depict-portal-openapi-original.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://depict.eu.auth0.com/oauth/authorize\n    tokenUrl: https://depict.eu.auth0.com/oauth/token\nscopes:\n- scope: email\n  description: User email\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/depict-lite-openapi-original.json\n  - openapi/depict-portal-openapi-original.json\n- scope: openid\n  description: OpenID Connect\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/depict-lite-openapi-original.json\n  - openapi/depict-portal-openapi-original.json\n\
  - scope: profile\n  description: User profile\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/depict-lite-openapi-original.json\n  - openapi/depict-portal-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/depict/refs/heads/main/scopes/depict-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- E-commerce
- Merchandising
- Product Recommendations
- Search
- Personalization
- Artificial Intelligence
- Retail
- Fashion
- Shopify
token_urls:
- https://depict.eu.auth0.com/oauth/token
---
