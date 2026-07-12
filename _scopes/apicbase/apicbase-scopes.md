---
authorization_urls:
- https://app.apicbase.com/oauth/authorize/
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Apicbase Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Apicbase publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Apicbase API on a user''s behalf.


  Tokens are issued from https://api.apicbase.com/oauth/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Apicbase
provider_slug: apicbase
schemes:
- description: OAuth 2.0 authorization code flow. Access tokens are bearer tokens valid for 7 days; refresh tokens obtain new access tokens. Include the token in the Authorization header as "Bearer ACCESS_TOKEN".
  flows:
  - authorizationUrl: https://app.apicbase.com/oauth/authorize/
    flow: authorizationCode
    tokenUrl: https://api.apicbase.com/oauth/token/
  name: oauth2
  source: openapi/apicbase-openapi.yml
scope_count: 2
scope_names:
- accounts
- library
scopes:
- description: Access account and outlet data.
  flows:
  - authorizationCode
  scope: accounts
- description: Access library data (ingredients, recipes, stock).
  flows:
  - authorizationCode
  scope: library
slug: apicbase-scopes
source_filename: apicbase-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apicbase-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/apicbase-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.apicbase.com/oauth/authorize/\n    tokenUrl: https://api.apicbase.com/oauth/token/\n  description: OAuth 2.0 authorization code flow. Access tokens are bearer tokens valid for\n    7 days; refresh tokens obtain new access tokens. Include the token in the Authorization\n    header as \"Bearer ACCESS_TOKEN\".\nscopes:\n- scope: accounts\n  description: Access account and outlet data.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/apicbase-openapi.yml\n- scope: library\n  description: Access library data (ingredients, recipes, stock).\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/apicbase-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apicbase/refs/heads/main/scopes/apicbase-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Food and Beverage
- Restaurant
- Back of House
- Inventory
- Procurement
- Recipes
token_urls:
- https://api.apicbase.com/oauth/token/
---
