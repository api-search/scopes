---
api_specs:
- filename: depictai-storefront-openapi.json
  format: json
  label: Depict Storefront API
  slug: depict-storefront-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/depictai/refs/heads/main/openapi/depictai-storefront-openapi.json
- filename: depictai-portal-openapi.json
  format: json
  label: Depict Portal API
  slug: depict-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/depictai/refs/heads/main/openapi/depictai-portal-openapi.json
- filename: depictai-lite-openapi.json
  format: json
  label: Depict Lite API
  slug: depict-lite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/depictai/refs/heads/main/openapi/depictai-lite-openapi.json
authorization_urls:
- https://depict.eu.auth0.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Depictai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Depict.AI publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Depict.AI API on a user''s behalf.


  Tokens are issued from https://depict.eu.auth0.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Depict.AI
provider_slug: depictai
schemes:
- flows:
  - authorizationUrl: https://depict.eu.auth0.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://depict.eu.auth0.com/oauth/token
  name: Auth0
  source: openapi/depictai-lite-openapi.json
- flows:
  - authorizationUrl: https://depict.eu.auth0.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://depict.eu.auth0.com/oauth/token
  name: Auth0
  source: openapi/depictai-portal-openapi.json
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
slug: depictai-scopes
source_filename: depictai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/depictai-lite-openapi.json, openapi/depictai-portal-openapi.json\nschemes:\n- name: Auth0\n  source: openapi/depictai-lite-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://depict.eu.auth0.com/oauth/authorize\n    tokenUrl: https://depict.eu.auth0.com/oauth/token\n- name: Auth0\n  source: openapi/depictai-portal-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://depict.eu.auth0.com/oauth/authorize\n    tokenUrl: https://depict.eu.auth0.com/oauth/token\nscopes:\n- scope: email\n  description: User email\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/depictai-lite-openapi.json\n  - openapi/depictai-portal-openapi.json\n- scope: openid\n  description: OpenID Connect\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/depictai-lite-openapi.json\n  - openapi/depictai-portal-openapi.json\n- scope: profile\n  description: User profile\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - openapi/depictai-lite-openapi.json\n  - openapi/depictai-portal-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/depictai/refs/heads/main/scopes/depictai-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- E Commerce
- Search
- Recommendations
- Merchandising
- Personalization
- Product Discovery
- Retail
- Shopify
- Artificial Intelligence
token_urls:
- https://depict.eu.auth0.com/oauth/token
---
