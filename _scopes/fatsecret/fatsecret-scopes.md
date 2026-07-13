---
api_specs:
- filename: fatsecret-platform-openapi.yml
  format: yaml
  label: FatSecret Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-platform-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Fatsecret Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'FatSecret publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the FatSecret API on a user''s behalf.


  Tokens are issued from https://oauth.fatsecret.com/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: FatSecret
provider_slug: fatsecret
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://oauth.fatsecret.com/connect/token
  name: oauth2
  source: openapi/fatsecret-platform-openapi.yml
scope_count: 2
scope_names:
- basic
- premier
scopes:
- description: Basic access to food and recipe data
  flows:
  - clientCredentials
  scope: basic
- description: Premier access including image recognition and NLP
  flows:
  - clientCredentials
  scope: premier
slug: fatsecret-scopes
source_filename: fatsecret-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fatsecret-platform-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/fatsecret-platform-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://oauth.fatsecret.com/connect/token\nscopes:\n- scope: basic\n  description: Basic access to food and recipe data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/fatsecret-platform-openapi.yml\n- scope: premier\n  description: Premier access including image recognition and NLP\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/fatsecret-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/scopes/fatsecret-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Barcode Scanning
- Calories
- Diets
- Exercise
- Fitness
- Food Diary
- Health
- Macronutrients
- Nutrition
- Recipes
- Weight Tracking
token_urls:
- https://oauth.fatsecret.com/connect/token
---
