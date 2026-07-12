---
authorization_urls:
- https://api.wellsfargo.com/oauth2/authorize
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Wells Fargo Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'wells-fargo publishes 4 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the wells-fargo API on a user''s behalf.


  Tokens are issued from https://api.wellsfargo.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: wells-fargo
provider_slug: wells-fargo
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.wellsfargo.com/oauth2/token
  name: oauth2
  source: openapi/wells-fargo-account-transactions-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.wellsfargo.com/oauth2/token
  name: oauth2
  source: openapi/wells-fargo-ach-payments-api-openapi.yml
- flows:
  - authorizationUrl: https://api.wellsfargo.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.wellsfargo.com/oauth2/token
  name: oauth2
  source: openapi/wells-fargo-gateway-api-openapi.yml
scope_count: 4
scope_names:
- accounts:read
- payments:read
- payments:write
- transactions:read
scopes:
- description: Read account information and balances
  flows:
  - authorizationCode
  - clientCredentials
  scope: accounts:read
- description: Read payment information and status
  flows:
  - clientCredentials
  scope: payments:read
- description: Initiate and cancel payments
  flows:
  - authorizationCode
  - clientCredentials
  scope: payments:write
- description: Read transaction history and details
  flows:
  - authorizationCode
  - clientCredentials
  scope: transactions:read
slug: wells-fargo-scopes
source_filename: wells-fargo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wells-fargo-account-transactions-api-openapi.yml, openapi/wells-fargo-ach-payments-api-openapi.yml,\n  openapi/wells-fargo-gateway-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/wells-fargo-account-transactions-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.wellsfargo.com/oauth2/token\n- name: oauth2\n  source: openapi/wells-fargo-ach-payments-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.wellsfargo.com/oauth2/token\n- name: oauth2\n  source: openapi/wells-fargo-gateway-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.wellsfargo.com/oauth2/authorize\n    tokenUrl: https://api.wellsfargo.com/oauth2/token\nscopes:\n- scope: accounts:read\n  description: Read account information and balances\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/wells-fargo-account-transactions-api-openapi.yml\n\
  \  - openapi/wells-fargo-gateway-api-openapi.yml\n- scope: payments:read\n  description: Read payment information and status\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/wells-fargo-ach-payments-api-openapi.yml\n- scope: payments:write\n  description: Initiate and cancel payments\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/wells-fargo-ach-payments-api-openapi.yml\n  - openapi/wells-fargo-gateway-api-openapi.yml\n- scope: transactions:read\n  description: Read transaction history and details\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/wells-fargo-account-transactions-api-openapi.yml\n  - openapi/wells-fargo-gateway-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wells-fargo/refs/heads/main/scopes/wells-fargo-scopes.yml
summary_line: 4 scopes · clientCredentials/authorizationCode
tags:
- Fortune 100
token_urls:
- https://api.wellsfargo.com/oauth2/token
---
