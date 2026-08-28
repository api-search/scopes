---
api_specs:
- filename: wger-openapi.yml
  format: yaml
  label: Wger REST API v2
  slug: wger-rest-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wger/refs/heads/main/openapi/wger-openapi.yml
authorization_urls:
- https://wger.de/identity/o/authorize
description: ''
docs: https://wger.readthedocs.io/en/latest/administration/oauth2_provider.html
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Wger Scopes
name_suffix: OAuth Scopes
note: Baseline derived from the oidcAuth securityScheme in openapi/wger-openapi.yml, then upgraded from the live OIDC discovery document at https://wger.de/.well-known/openid-configuration (HTTP 200, probed 2026-08-27), which advertises three scopes the OpenAPI securityScheme does not list (openid, profile, email). wger acts as its own OAuth2/OIDC provider (django-oauth-toolkit); the provider is off by default on a self-hosted instance until configured.
overview: 'Wger publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Wger API on a user''s behalf.


  Tokens are issued from https://wger.de/identity/o/api/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Wger
provider_slug: wger
schemes:
- description: Access token issued by the OAuth2/OIDC provider
  flows:
  - authorizationUrl: https://wger.de/identity/o/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    tokenUrl: https://wger.de/identity/o/api/token
  issuer: https://wger.de
  name: oidcAuth
  source: openapi/wger-openapi.yml
scope_count: 5
scope_names:
- api:read
- api:write
- openid
- profile
- email
scopes:
- description: View your training, nutrition and body data
  flows:
  - authorizationCode
  scope: api:read
- description: Add and change your training, nutrition and body data
  flows:
  - authorizationCode
  scope: api:write
- description: Standard OIDC scope; requests an ID token for the signed-in wger user
  flows:
  - authorizationCode
  scope: openid
- description: Standard OIDC scope; basic profile claims at the userinfo endpoint
  flows:
  - authorizationCode
  scope: profile
- description: Standard OIDC scope; the account's email address
  flows:
  - authorizationCode
  scope: email
slug: wger-scopes
source_filename: wger-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: https://wger.de/.well-known/openid-configuration\ndocs: https://wger.readthedocs.io/en/latest/administration/oauth2_provider.html\nspec: openapi/wger-openapi.yml\nnote: >-\n  Baseline derived from the oidcAuth securityScheme in\n  openapi/wger-openapi.yml, then upgraded from the live OIDC discovery\n  document at https://wger.de/.well-known/openid-configuration (HTTP 200,\n  probed 2026-08-27), which advertises three scopes the OpenAPI securityScheme\n  does not list (openid, profile, email). wger acts as its own OAuth2/OIDC\n  provider (django-oauth-toolkit); the provider is off by default on a\n  self-hosted instance until configured.\nschemes:\n  - name: oidcAuth\n    source: openapi/wger-openapi.yml\n    issuer: https://wger.de\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://wger.de/identity/o/authorize\n        tokenUrl: https://wger.de/identity/o/api/token\n        code_challenge_methods:\
  \ [S256]\n    description: Access token issued by the OAuth2/OIDC provider\nscopes:\n  - scope: api:read\n    description: View your training, nutrition and body data\n    flows: [authorizationCode]\n    sources:\n      - openapi/wger-openapi.yml\n      - https://wger.de/.well-known/openid-configuration\n  - scope: api:write\n    description: Add and change your training, nutrition and body data\n    flows: [authorizationCode]\n    sources:\n      - openapi/wger-openapi.yml\n      - https://wger.de/.well-known/openid-configuration\n  - scope: openid\n    description: Standard OIDC scope; requests an ID token for the signed-in wger user\n    flows: [authorizationCode]\n    sources:\n      - https://wger.de/.well-known/openid-configuration\n  - scope: profile\n    description: Standard OIDC scope; basic profile claims at the userinfo endpoint\n    flows: [authorizationCode]\n    sources:\n      - https://wger.de/.well-known/openid-configuration\n  - scope: email\n    description: Standard\
  \ OIDC scope; the account's email address\n    flows: [authorizationCode]\n    sources:\n      - https://wger.de/.well-known/openid-configuration\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wger/refs/heads/main/scopes/wger-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Sports And Fitness
- Public APIs
- Fitness
- Nutrition
- Health
- Open Source
- Self Hosted
- Workout Tracking
- Django
- REST
token_urls:
- https://wger.de/identity/o/api/token
---
