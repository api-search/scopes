---
api_specs:
- filename: zettle-finance-api-openapi.yaml
  format: yaml
  label: Zettle Finance API
  slug: zettle-finance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zettle/refs/heads/main/openapi/zettle-finance-api-openapi.yaml
authorization_urls:
- https://oauth.zettle.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Zettle Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Zettle publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Zettle API on a user''s behalf.


  Tokens are issued from https://oauth.zettle.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Zettle
provider_slug: zettle
schemes:
- description: For more information, see the [OAuth API documentation](https://developer.zettle.com/docs/api/oauth/overview).
  flows:
  - authorizationUrl: https://oauth.zettle.com/authorize
    flow: authorizationCode
    tokenUrl: https://oauth.zettle.com/token
  name: ZettleOauth
  source: openapi/zettle-finance-api-openapi.yaml
scope_count: 1
scope_names:
- READ:FINANCE
scopes:
- description: Access to read finance data
  flows:
  - authorizationCode
  scope: READ:FINANCE
slug: zettle-scopes
source_filename: zettle-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zettle-finance-api-openapi.yaml\nschemes:\n- name: ZettleOauth\n  source: openapi/zettle-finance-api-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth.zettle.com/authorize\n    tokenUrl: https://oauth.zettle.com/token\n  description: For more information, see the [OAuth API documentation](https://developer.zettle.com/docs/api/oauth/overview).\nscopes:\n- scope: READ:FINANCE\n  description: Access to read finance data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zettle-finance-api-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zettle/refs/heads/main/scopes/zettle-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Point of Sale
- POS
- Payments
- Inventory
- Finance
- PayPal
- Card Payments
- Merchant Services
token_urls:
- https://oauth.zettle.com/token
---
