---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: State Street Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'State Street publishes 8 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the State Street API on a user''s behalf.


  Tokens are issued from https://api.statestreet.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: State Street
provider_slug: state-street
schemes:
- description: OAuth 2.0 Client Credentials flow per RFC 6749 Section 4.4.2. Requires multifactor authentication for all user access.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.statestreet.com/oauth/token
  name: OAuth2
  source: openapi/state-street-alpha-data-platform-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.statestreet.com/oauth/token
  name: OAuth2
  source: openapi/state-street-fund-connect-openapi.yml
scope_count: 8
scope_names:
- fund-connect:baskets:read
- fund-connect:orders:read
- fund-connect:orders:write
- performance:read
- portfolio:read
- positions:read
- risk:read
- transactions:read
scopes:
- description: Read ETF portfolio basket compositions
  flows:
  - clientCredentials
  scope: fund-connect:baskets:read
- description: Read ETF order history and status
  flows:
  - clientCredentials
  scope: fund-connect:orders:read
- description: Submit and cancel ETF orders
  flows:
  - clientCredentials
  scope: fund-connect:orders:write
- description: Read performance measurement and attribution data
  flows:
  - clientCredentials
  scope: performance:read
- description: Read portfolio metadata and account information
  flows:
  - clientCredentials
  scope: portfolio:read
- description: Read portfolio positions and holdings
  flows:
  - clientCredentials
  scope: positions:read
- description: Read risk analytics and exposure data
  flows:
  - clientCredentials
  scope: risk:read
- description: Read transaction history
  flows:
  - clientCredentials
  scope: transactions:read
slug: state-street-scopes
source_filename: state-street-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/state-street-alpha-data-platform-openapi.yml, openapi/state-street-fund-connect-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/state-street-alpha-data-platform-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.statestreet.com/oauth/token\n  description: OAuth 2.0 Client Credentials flow per RFC 6749 Section 4.4.2. Requires multifactor\n    authentication for all user access.\n- name: OAuth2\n  source: openapi/state-street-fund-connect-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.statestreet.com/oauth/token\nscopes:\n- scope: fund-connect:baskets:read\n  description: Read ETF portfolio basket compositions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/state-street-fund-connect-openapi.yml\n- scope: fund-connect:orders:read\n  description: Read ETF order history and status\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/state-street-fund-connect-openapi.yml\n\
  - scope: fund-connect:orders:write\n  description: Submit and cancel ETF orders\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/state-street-fund-connect-openapi.yml\n- scope: performance:read\n  description: Read performance measurement and attribution data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/state-street-alpha-data-platform-openapi.yml\n- scope: portfolio:read\n  description: Read portfolio metadata and account information\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/state-street-alpha-data-platform-openapi.yml\n- scope: positions:read\n  description: Read portfolio positions and holdings\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/state-street-alpha-data-platform-openapi.yml\n- scope: risk:read\n  description: Read risk analytics and exposure data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/state-street-alpha-data-platform-openapi.yml\n- scope: transactions:read\n  description: Read transaction history\n  flows:\n\
  \  - clientCredentials\n  sources:\n  - openapi/state-street-alpha-data-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/state-street/refs/heads/main/scopes/state-street-scopes.yml
summary_line: 8 scopes · clientCredentials
tags:
- Fortune 500
token_urls:
- https://api.statestreet.com/oauth/token
---
