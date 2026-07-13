---
api_specs:
- filename: interactive-brokers-web-api-openapi.yml
  format: yaml
  label: Interactive Brokers Web API
  slug: web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interactive-brokers/refs/heads/main/openapi/interactive-brokers-web-api-openapi.yml
authorization_urls:
- https://www.interactivebrokers.com/authorize
description: ''
docs: https://www.interactivebrokers.com/campus/ibkr-api-page/web-api-account-management/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Interactive Brokers Scopes
name_suffix: OAuth Scopes
note: Scopes apply to the OAuth 2.0 client_credentials token request (POST https://api.ibkr.com/oauth2/api/v1/token with private_key_jwt client assertion) documented on IBKR's Account Management Web API page; the trading Web API docs do not publish additional scope values.
overview: 'Interactive Brokers publishes 18 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Interactive Brokers API on a user''s behalf.


  Tokens are issued from https://www.interactivebrokers.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Interactive Brokers
provider_slug: interactive-brokers
schemes:
- flows:
  - authorizationUrl: https://www.interactivebrokers.com/authorize
    flow: authorizationCode
    tokenUrl: https://www.interactivebrokers.com/token
  name: oauth2
  source: openapi/interactive-brokers-web-api-openapi.yml
scope_count: 18
scope_names:
- accounts.read
- accounts.write
- bank-instructions.read
- bank-instructions.write
- clients.read
- clients.write
- echo.read
- echo.write
- fee-templates.read
- fee-templates.write
- instructions.read
- instructions.write
- statements.read
- transfers.read
- transfers.write
- sso-sessions.write
- sso-browser-sessions.write
- enumerations.read
scopes:
- description: View brokerage account information.
  flows: []
  scope: accounts.read
- description: Create a brokerage account.
  flows: []
  scope: accounts.write
- description: Listed in IBKR's documented token-request scope string; no individual description published.
  flows: []
  scope: bank-instructions.read
- description: Add banking instructions.
  flows: []
  scope: bank-instructions.write
- description: Listed in IBKR's documented token-request scope string; no individual description published.
  flows: []
  scope: clients.read
- description: Listed in IBKR's documented token-request scope string; no individual description published.
  flows: []
  scope: clients.write
- description: Listed in IBKR's documented token-request scope string; no individual description published.
  flows: []
  scope: echo.read
- description: Listed in IBKR's documented token-request scope string; no individual description published.
  flows: []
  scope: echo.write
- description: Listed in IBKR's documented token-request scope string; no individual description published.
  flows: []
  scope: fee-templates.read
- description: Listed in IBKR's documented token-request scope string; no individual description published.
  flows: []
  scope: fee-templates.write
- description: View fund transfer.
  flows: []
  scope: instructions.read
- description: Listed in IBKR's documented token-request scope string; no individual description published.
  flows: []
  scope: instructions.write
- description: View client statement.
  flows: []
  scope: statements.read
- description: Listed in IBKR's documented token-request scope string; no individual description published.
  flows: []
  scope: transfers.read
- description: Transfer funds.
  flows: []
  scope: transfers.write
- description: Create an SSO session used for placing trades (documented in prose as "sso.sessions.write").
  flows: []
  scope: sso-sessions.write
- description: Create an SSO session to the IBKR Portal.
  flows: []
  scope: sso-browser-sessions.write
- description: Listed in IBKR's documented token-request scope string; no individual description published.
  flows: []
  scope: enumerations.read
slug: interactive-brokers-scopes
source_filename: interactive-brokers-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/interactive-brokers-web-api-openapi.yml\ndocs: https://www.interactivebrokers.com/campus/ibkr-api-page/web-api-account-management/\nschemes:\n- name: oauth2\n  source: openapi/interactive-brokers-web-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.interactivebrokers.com/authorize\n    tokenUrl: https://www.interactivebrokers.com/token\nscopes:\n- scope: accounts.read\n  description: View brokerage account information.\n  sources:\n  - https://www.interactivebrokers.com/campus/ibkr-api-page/web-api-account-management/\n- scope: accounts.write\n  description: Create a brokerage account.\n  sources:\n  - https://www.interactivebrokers.com/campus/ibkr-api-page/web-api-account-management/\n- scope: bank-instructions.read\n  description: Listed in IBKR's documented token-request scope string; no individual\n    description published.\n  sources:\n  - https://www.interactivebrokers.com/campus/ibkr-api-page/web-api-account-management/\n\
  - scope: bank-instructions.write\n  description: Add banking instructions.\n  sources:\n  - https://www.interactivebrokers.com/campus/ibkr-api-page/web-api-account-management/\n- scope: clients.read\n  description: Listed in IBKR's documented token-request scope string; no individual\n    description published.\n  sources:\n  - https://www.interactivebrokers.com/campus/ibkr-api-page/web-api-account-management/\n- scope: clients.write\n  description: Listed in IBKR's documented token-request scope string; no individual\n    description published.\n  sources:\n  - https://www.interactivebrokers.com/campus/ibkr-api-page/web-api-account-management/\n- scope: echo.read\n  description: Listed in IBKR's documented token-request scope string; no individual\n    description published.\n  sources:\n  - https://www.interactivebrokers.com/campus/ibkr-api-page/web-api-account-management/\n- scope: echo.write\n  description: Listed in IBKR's documented token-request scope string; no individual\n   \
  \ description published.\n  sources:\n  - https://www.interactivebrokers.com/campus/ibkr-api-page/web-api-account-management/\n- scope: fee-templates.read\n  description: Listed in IBKR's documented token-request scope string; no individual\n    description published.\n  sources:\n  - https://www.interactivebrokers.com/campus/ibkr-api-page/web-api-account-management/\n- scope: fee-templates.write\n  description: Listed in IBKR's documented token-request scope string; no individual\n    description published.\n  sources:\n  - https://www.interactivebrokers.com/campus/ibkr-api-page/web-api-account-management/\n- scope: instructions.read\n  description: View fund transfer.\n  sources:\n  - https://www.interactivebrokers.com/campus/ibkr-api-page/web-api-account-management/\n- scope: instructions.write\n  description: Listed in IBKR's documented token-request scope string; no individual\n    description published.\n  sources:\n  - https://www.interactivebrokers.com/campus/ibkr-api-page/web-api-account-management/\n\
  - scope: statements.read\n  description: View client statement.\n  sources:\n  - https://www.interactivebrokers.com/campus/ibkr-api-page/web-api-account-management/\n- scope: transfers.read\n  description: Listed in IBKR's documented token-request scope string; no individual\n    description published.\n  sources:\n  - https://www.interactivebrokers.com/campus/ibkr-api-page/web-api-account-management/\n- scope: transfers.write\n  description: Transfer funds.\n  sources:\n  - https://www.interactivebrokers.com/campus/ibkr-api-page/web-api-account-management/\n- scope: sso-sessions.write\n  description: Create an SSO session used for placing trades (documented in prose\n    as \"sso.sessions.write\").\n  sources:\n  - https://www.interactivebrokers.com/campus/ibkr-api-page/web-api-account-management/\n- scope: sso-browser-sessions.write\n  description: Create an SSO session to the IBKR Portal.\n  sources:\n  - https://www.interactivebrokers.com/campus/ibkr-api-page/web-api-account-management/\n\
  - scope: enumerations.read\n  description: Listed in IBKR's documented token-request scope string; no individual\n    description published.\n  sources:\n  - https://www.interactivebrokers.com/campus/ibkr-api-page/web-api-account-management/\nnote: Scopes apply to the OAuth 2.0 client_credentials token request (POST https://api.ibkr.com/oauth2/api/v1/token\n  with private_key_jwt client assertion) documented on IBKR's Account Management Web\n  API page; the trading Web API docs do not publish additional scope values.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/interactive-brokers/refs/heads/main/scopes/interactive-brokers-scopes.yml
summary_line: 18 scopes · authorizationCode
tags:
- Brokerage
- Market Data
- Orders
- Portfolio
- Trading
token_urls:
- https://www.interactivebrokers.com/token
---
