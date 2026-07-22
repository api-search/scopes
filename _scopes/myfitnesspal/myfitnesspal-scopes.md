---
api_specs:
- filename: myfitnesspal-notifications-asyncapi.yml
  format: yaml
  label: MyFitnessPal API v2
  slug: myfitnesspal-api-v2
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/myfitnesspal/refs/heads/main/asyncapi/myfitnesspal-notifications-asyncapi.yml
authorization_urls:
- https://api.myfitnesspal.com/v2/oauth2/auth
description: ''
docs: https://myfitnesspalapi.com/docs/user-authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Myfitnesspal Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'MyFitnessPal publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the MyFitnessPal API on a user''s behalf.


  Tokens are issued from https://api.myfitnesspal.com/v2/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: MyFitnessPal
provider_slug: myfitnesspal
schemes:
- flows:
  - authorizationUrl: https://api.myfitnesspal.com/v2/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://api.myfitnesspal.com/v2/oauth2/token
  name: OAuth2
scope_count: 4
scope_names:
- diary
- measurements
- private-exercises
- subscriptions
scopes:
- description: Read and write the user's food and exercise diary (meals and cardio/exercise entries).
  flows:
  - authorizationCode
  scope: diary
- description: Read and write the user's body measurements (weight and other measured values).
  flows:
  - authorizationCode
  scope: measurements
- description: Access the user's private/custom exercise definitions.
  flows:
  - authorizationCode
  scope: private-exercises
- description: Create, read, and delete webhook subscriptions for user data-change notifications.
  flows:
  - authorizationCode
  scope: subscriptions
slug: myfitnesspal-scopes
source_filename: myfitnesspal-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://myfitnesspalapi.com/docs/auth-example-2\ndocs: https://myfitnesspalapi.com/docs/user-authentication\nschemes:\n- name: OAuth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.myfitnesspal.com/v2/oauth2/auth\n    tokenUrl: https://api.myfitnesspal.com/v2/oauth2/token\nscopes:\n- scope: diary\n  description: Read and write the user's food and exercise diary (meals and cardio/exercise entries).\n  flows: [authorizationCode]\n- scope: measurements\n  description: Read and write the user's body measurements (weight and other measured values).\n  flows: [authorizationCode]\n- scope: private-exercises\n  description: Access the user's private/custom exercise definitions.\n  flows: [authorizationCode]\n- scope: subscriptions\n  description: Create, read, and delete webhook subscriptions for user data-change notifications.\n  flows: [authorizationCode]\nnotes:\n- Scope values confirmed verbatim from\
  \ the documented authorization request example (scope=diary+measurements+private-exercises+subscriptions).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/myfitnesspal/refs/heads/main/scopes/myfitnesspal-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Consumer
- Health and Fitness
- Nutrition
- Fitness Tracking
- Food Diary
- Wellness
- Webhooks
- OAuth
token_urls:
- https://api.myfitnesspal.com/v2/oauth2/token
---
