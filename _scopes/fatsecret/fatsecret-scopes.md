---
api_specs:
- filename: fatsecret-exercise-diary-api-openapi.yml
  format: yaml
  label: FatSecret Exercise Diary API
  slug: fatsecret-exercise-diary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-exercise-diary-api-openapi.yml
- filename: fatsecret-food-diary-api-openapi.yml
  format: yaml
  label: FatSecret Food Diary API
  slug: fatsecret-food-diary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-food-diary-api-openapi.yml
- filename: fatsecret-foods-api-openapi.yml
  format: yaml
  label: FatSecret Foods API
  slug: fatsecret-foods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-foods-api-openapi.yml
- filename: fatsecret-profile-foods-api-openapi.yml
  format: yaml
  label: FatSecret Profile Foods API
  slug: fatsecret-profile-foods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-profile-foods-api-openapi.yml
- filename: fatsecret-profile-meals-api-openapi.yml
  format: yaml
  label: FatSecret Profile Meals API
  slug: fatsecret-profile-meals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-profile-meals-api-openapi.yml
- filename: fatsecret-recipes-api-openapi.yml
  format: yaml
  label: FatSecret Recipes API
  slug: fatsecret-recipes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-recipes-api-openapi.yml
- filename: fatsecret-reference-api-openapi.yml
  format: yaml
  label: FatSecret Reference API
  slug: fatsecret-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-reference-api-openapi.yml
- filename: fatsecret-weight-tracking-api-openapi.yml
  format: yaml
  label: FatSecret Weight Tracking API
  slug: fatsecret-weight-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-weight-tracking-api-openapi.yml
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
