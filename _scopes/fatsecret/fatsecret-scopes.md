---
api_specs:
- filename: fatsecret-exercise-diary-api-openapi.yml
  format: yaml
  label: fatsecret Exercise Diary API
  slug: fatsecret-exercise-diary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-exercise-diary-api-openapi.yml
- filename: fatsecret-food-diary-api-openapi.yml
  format: yaml
  label: fatsecret Food Diary API
  slug: fatsecret-food-diary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-food-diary-api-openapi.yml
- filename: fatsecret-foods-api-openapi.yml
  format: yaml
  label: fatsecret Foods API
  slug: fatsecret-foods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-foods-api-openapi.yml
- filename: fatsecret-image-recognition-api-openapi.yml
  format: yaml
  label: fatsecret Image Recognition API
  slug: fatsecret-image-recognition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-image-recognition-api-openapi.yml
- filename: fatsecret-natural-language-processing-api-openapi.yml
  format: yaml
  label: fatsecret Natural Language Processing API
  slug: fatsecret-natural-language-processing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-natural-language-processing-api-openapi.yml
- filename: fatsecret-profile-foods-api-openapi.yml
  format: yaml
  label: fatsecret Profile Foods API
  slug: fatsecret-profile-foods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-profile-foods-api-openapi.yml
- filename: fatsecret-profile-meals-api-openapi.yml
  format: yaml
  label: fatsecret Profile Meals API
  slug: fatsecret-profile-meals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-profile-meals-api-openapi.yml
- filename: fatsecret-recipes-api-openapi.yml
  format: yaml
  label: fatsecret Recipes API
  slug: fatsecret-recipes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-recipes-api-openapi.yml
- filename: fatsecret-reference-api-openapi.yml
  format: yaml
  label: fatsecret Reference API
  slug: fatsecret-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-reference-api-openapi.yml
- filename: fatsecret-weight-tracking-api-openapi.yml
  format: yaml
  label: fatsecret Weight Tracking API
  slug: fatsecret-weight-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-weight-tracking-api-openapi.yml
authorization_urls: []
description: ''
docs: https://platform.fatsecret.com/docs/guides/authentication/oauth2
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Fatsecret Scopes
name_suffix: OAuth Scopes
note: Upgraded from derived to searched on 2026-08-12. The OpenAPI declares only two scopes (basic, premier); the provider's OAuth 2.0 guide documents SEVEN. The five the spec omits — barcode, localization, nlp, image-recognition, feedback — gate exactly the capabilities fatsecret sells as add-ons, so a client built from the spec alone will hit error 14 ("Missing scope") on the barcode, image-recognition and NLP methods with no indication why.
overview: 'fatsecret publishes 7 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the fatsecret API on a user''s behalf.


  Tokens are issued from https://oauth.fatsecret.com/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: fatsecret
provider_slug: fatsecret
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://oauth.fatsecret.com/connect/token
  name: oauth2
  openid_configuration: https://oauth.fatsecret.com/.well-known/openid-configuration
  source: openapi/_original/fatsecret-platform-openapi.yml
- name: oauth1
  note: OAuth 1.0a 3-legged is used for member/profile data and carries no scope surface — the member authorization itself is the grant.
  source: openapi/_original/fatsecret-platform-openapi.yml
scope_count: 7
scope_names:
- basic
- premier
- barcode
- localization
- nlp
- image-recognition
- feedback
scopes:
- description: Basic access to food and recipe data
  flows:
  - clientCredentials
  scope: basic
- description: Premier access, including the enriched food data and global datasets sold on the Premier editions
  flows:
  - clientCredentials
  scope: premier
- description: UPC / GTIN-13 barcode lookup (food.find_id_for_barcode)
  flows:
  - clientCredentials
  scope: barcode
- description: Region and language filtering of results across 200+ regions and 25 languages
  flows:
  - clientCredentials
  scope: localization
- description: Natural Language Processing — parse a free-text description of what was eaten into foods
  flows:
  - clientCredentials
  scope: nlp
- description: Image Recognition — identify foods from an uploaded photo
  flows:
  - clientCredentials
  scope: image-recognition
- description: Feedback submission on API results
  flows:
  - clientCredentials
  scope: feedback
slug: fatsecret-scopes
source_filename: fatsecret-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://platform.fatsecret.com/docs/guides/authentication/oauth2\ndocs: https://platform.fatsecret.com/docs/guides/authentication/oauth2\nnote: >-\n  Upgraded from derived to searched on 2026-08-12. The OpenAPI declares only two scopes (basic,\n  premier); the provider's OAuth 2.0 guide documents SEVEN. The five the spec omits — barcode,\n  localization, nlp, image-recognition, feedback — gate exactly the capabilities fatsecret sells as\n  add-ons, so a client built from the spec alone will hit error 14 (\"Missing scope\") on the\n  barcode, image-recognition and NLP methods with no indication why.\nschemes:\n  - name: oauth2\n    source: openapi/_original/fatsecret-platform-openapi.yml\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://oauth.fatsecret.com/connect/token\n    openid_configuration: https://oauth.fatsecret.com/.well-known/openid-configuration\n  - name: oauth1\n    source: openapi/_original/fatsecret-platform-openapi.yml\n\
  \    note: >-\n      OAuth 1.0a 3-legged is used for member/profile data and carries no scope surface — the member\n      authorization itself is the grant.\nscopes:\n  - scope: basic\n    description: Basic access to food and recipe data\n    flows: [clientCredentials]\n    sources: [openapi/_original/fatsecret-platform-openapi.yml, https://platform.fatsecret.com/docs/guides/authentication/oauth2]\n  - scope: premier\n    description: Premier access, including the enriched food data and global datasets sold on the Premier editions\n    flows: [clientCredentials]\n    sources: [openapi/_original/fatsecret-platform-openapi.yml, https://platform.fatsecret.com/docs/guides/authentication/oauth2]\n  - scope: barcode\n    description: UPC / GTIN-13 barcode lookup (food.find_id_for_barcode)\n    flows: [clientCredentials]\n    sources: [https://platform.fatsecret.com/docs/guides/authentication/oauth2]\n  - scope: localization\n    description: Region and language filtering of results across 200+\
  \ regions and 25 languages\n    flows: [clientCredentials]\n    sources: [https://platform.fatsecret.com/docs/guides/authentication/oauth2]\n  - scope: nlp\n    description: Natural Language Processing — parse a free-text description of what was eaten into foods\n    flows: [clientCredentials]\n    sources: [https://platform.fatsecret.com/docs/guides/authentication/oauth2]\n  - scope: image-recognition\n    description: Image Recognition — identify foods from an uploaded photo\n    flows: [clientCredentials]\n    sources: [https://platform.fatsecret.com/docs/guides/authentication/oauth2]\n  - scope: feedback\n    description: Feedback submission on API results\n    flows: [clientCredentials]\n    sources: [https://platform.fatsecret.com/docs/guides/authentication/oauth2]\nscope_count: 7\nmissing_from_spec: [barcode, localization, nlp, image-recognition, feedback]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/scopes/fatsecret-scopes.yml
summary_line: 7 scopes · clientCredentials
tags:
- Artificial Intelligence
- Barcode Scanning
- Calories
- Diets
- Image Recognition
- Natural Language Processing
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
