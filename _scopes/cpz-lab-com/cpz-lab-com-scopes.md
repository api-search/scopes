---
api_specs:
- filename: cpz-lab-com-accounts-api-openapi.yml
  format: yaml
  label: CPZ Lab Accounts API
  slug: cpz-lab-com-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-accounts-api-openapi.yml
- filename: cpz-lab-com-actions-api-openapi.yml
  format: yaml
  label: CPZ Lab Actions API
  slug: cpz-lab-com-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-actions-api-openapi.yml
- filename: cpz-lab-com-backtests-api-openapi.yml
  format: yaml
  label: CPZ Lab Backtests API
  slug: cpz-lab-com-backtests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-backtests-api-openapi.yml
- filename: cpz-lab-com-cash-api-openapi.yml
  format: yaml
  label: CPZ Lab Cash API
  slug: cpz-lab-com-cash-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-cash-api-openapi.yml
- filename: cpz-lab-com-data-files-api-openapi.yml
  format: yaml
  label: CPZ Lab Data Files API
  slug: cpz-lab-com-data-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-data-files-api-openapi.yml
- filename: cpz-lab-com-me-api-openapi.yml
  format: yaml
  label: CPZ Lab Me API
  slug: cpz-lab-com-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-me-api-openapi.yml
- filename: cpz-lab-com-order-approvals-api-openapi.yml
  format: yaml
  label: CPZ Lab Order Approvals API
  slug: cpz-lab-com-order-approvals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-order-approvals-api-openapi.yml
- filename: cpz-lab-com-orders-api-openapi.yml
  format: yaml
  label: CPZ Lab Orders API
  slug: cpz-lab-com-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-orders-api-openapi.yml
- filename: cpz-lab-com-positions-api-openapi.yml
  format: yaml
  label: CPZ Lab Positions API
  slug: cpz-lab-com-positions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-positions-api-openapi.yml
- filename: cpz-lab-com-risk-snapshots-api-openapi.yml
  format: yaml
  label: CPZ Lab Risk Snapshots API
  slug: cpz-lab-com-risk-snapshots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-risk-snapshots-api-openapi.yml
- filename: cpz-lab-com-strategies-api-openapi.yml
  format: yaml
  label: CPZ Lab Strategies API
  slug: cpz-lab-com-strategies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-strategies-api-openapi.yml
- filename: cpz-lab-com-transactions-api-openapi.yml
  format: yaml
  label: CPZ Lab Transactions API
  slug: cpz-lab-com-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-transactions-api-openapi.yml
- filename: cpz-lab-com-watchlist-api-openapi.yml
  format: yaml
  label: CPZ Lab Watchlist API
  slug: cpz-lab-com-watchlist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-watchlist-api-openapi.yml
- filename: cpz-lab-com-webhooks-api-openapi.yml
  format: yaml
  label: CPZ Lab Webhooks API
  slug: cpz-lab-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-webhooks-api-openapi.yml
authorization_urls:
- https://api.cpz-lab.com/oauth/authorize
description: ''
docs: https://ai.cpz-lab.com/docs/api/introduction
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: CPZ Lab Scopes
name_suffix: OAuth Scopes
note: API keys are scoped in Settings > API Keys using the documented scope table (docs write "trading credentials" and "data connections" with spaces). Execute Order requires both orders AND trading credentials scopes.
overview: 'CPZ Lab publishes 13 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the CPZ Lab API on a user''s behalf.


  Tokens are issued from https://api.cpz-lab.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CPZ Lab
provider_slug: cpz-lab-com
schemes:
- description: OAuth 2.0 + PKCE issued by the CPZAI authorization server.
  flows:
  - authorizationUrl: https://api.cpz-lab.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.cpz-lab.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://api.cpz-lab.com/oauth/token
  name: OAuth2
  source: openapi/cpz-lab-com-openapi.yml
scope_count: 13
scope_names:
- confirm_orders
- data
- data_connections
- email
- offline_access
- openid
- orders
- orders_paper
- profile
- storage
- strategies
- trading_credentials
- simons
scopes:
- description: confirm_orders
  flows:
  - authorizationCode
  - clientCredentials
  scope: confirm_orders
- description: Fetch market data, economic data, news
  flows:
  - authorizationCode
  - clientCredentials
  scope: data
- description: Manage data provider connections
  flows:
  - authorizationCode
  - clientCredentials
  scope: data_connections
- description: email
  flows:
  - authorizationCode
  scope: email
- description: offline_access
  flows:
  - authorizationCode
  scope: offline_access
- description: openid
  flows:
  - authorizationCode
  scope: openid
- description: Submit, cancel, replace orders
  flows:
  - authorizationCode
  - clientCredentials
  scope: orders
- description: orders_paper
  flows:
  - authorizationCode
  - clientCredentials
  scope: orders_paper
- description: profile
  flows:
  - authorizationCode
  scope: profile
- description: Upload, download, manage files
  flows:
  - authorizationCode
  - clientCredentials
  scope: storage
- description: Create, read, update, delete strategies
  flows:
  - authorizationCode
  - clientCredentials
  scope: strategies
- description: Access broker connections
  flows:
  - authorizationCode
  - clientCredentials
  scope: trading_credentials
- description: Chat with Simons AI
  flows: []
  scope: simons
slug: cpz-lab-com-scopes
source_filename: cpz-lab-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource:\n- https://ai.cpz-lab.com/docs/api/introduction\n- openapi/cpz-lab-com-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/cpz-lab-com-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.cpz-lab.com/oauth/authorize\n    tokenUrl: https://api.cpz-lab.com/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://api.cpz-lab.com/oauth/token\n  description: OAuth 2.0 + PKCE issued by the CPZAI authorization server.\nscopes:\n- scope: confirm_orders\n  description: confirm_orders\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/cpz-lab-com-openapi.yml\n- scope: data\n  description: Fetch market data, economic data, news\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/cpz-lab-com-openapi.yml\n  - https://ai.cpz-lab.com/docs/api/introduction\n- scope: data_connections\n  description: Manage data provider connections\n  flows:\n\
  \  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/cpz-lab-com-openapi.yml\n  - https://ai.cpz-lab.com/docs/api/introduction\n- scope: email\n  description: email\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cpz-lab-com-openapi.yml\n- scope: offline_access\n  description: offline_access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cpz-lab-com-openapi.yml\n- scope: openid\n  description: openid\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cpz-lab-com-openapi.yml\n- scope: orders\n  description: Submit, cancel, replace orders\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/cpz-lab-com-openapi.yml\n  - https://ai.cpz-lab.com/docs/api/introduction\n- scope: orders_paper\n  description: orders_paper\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/cpz-lab-com-openapi.yml\n- scope: profile\n  description: profile\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cpz-lab-com-openapi.yml\n\
  - scope: storage\n  description: Upload, download, manage files\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/cpz-lab-com-openapi.yml\n  - https://ai.cpz-lab.com/docs/api/introduction\n- scope: strategies\n  description: Create, read, update, delete strategies\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/cpz-lab-com-openapi.yml\n  - https://ai.cpz-lab.com/docs/api/introduction\n- scope: trading_credentials\n  description: Access broker connections\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/cpz-lab-com-openapi.yml\n  - https://ai.cpz-lab.com/docs/api/introduction\n- scope: simons\n  description: Chat with Simons AI\n  api_key_scope: true\n  sources:\n  - https://ai.cpz-lab.com/docs/api/introduction\n  note: Documented as an API key scope; not declared in the OpenAPI oauth2 flows.\ndocs: https://ai.cpz-lab.com/docs/api/introduction\nnote: API keys are scoped in Settings > API Keys\
  \ using the documented scope table (docs write \"trading credentials\" and \"data connections\" with spaces). Execute Order requires both orders AND trading credentials\n  scopes.\n"
source_yaml_url: https://artifacts.apis.io/cpz-lab-com/scopes/cpz-lab-com-scopes.yml
summary_line: 13 scopes · authorizationCode/clientCredentials
tags:
- Company
- Trading
- Algorithmic Trading
- Quantitative Finance
- Backtesting
- Risk Management
- Artificial Intelligence
- MCP
- Python SDK
token_bound: false
token_urls:
- https://api.cpz-lab.com/oauth/token
---
