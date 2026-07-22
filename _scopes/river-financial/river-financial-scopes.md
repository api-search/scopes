---
authorization_urls:
- https://river.com/oauth2/authorize
description: ''
docs: https://river.com/.well-known/openid-configuration
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: River Financial Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'River Financial publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the River Financial API on a user''s behalf.


  Tokens are issued from https://river.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: River Financial
provider_slug: river-financial
schemes:
- flows:
  - authorizationUrl: https://river.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://river.com/oauth2/token
  name: OAuth2
  source: https://river.com/.well-known/openid-configuration
scope_count: 6
scope_names:
- openid
- offline_access
- balances:read
- transactions:read
- identity:read
- payment_networks:read
scopes:
- description: OpenID Connect authentication; issue an ID token for the subject.
  flows:
  - authorizationCode
  scope: openid
- description: Issue a refresh token for long-lived access without user presence.
  flows:
  - authorizationCode
  scope: offline_access
- description: Read access to account cash and bitcoin balances.
  flows:
  - authorizationCode
  scope: balances:read
- description: Read access to transaction history.
  flows:
  - authorizationCode
  scope: transactions:read
- description: Read access to account holder identity information.
  flows:
  - authorizationCode
  scope: identity:read
- description: Read access to configured payment networks / payout rails.
  flows:
  - authorizationCode
  scope: payment_networks:read
slug: river-financial-scopes
source_filename: river-financial-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://river.com/.well-known/openid-configuration\ndocs: https://river.com/.well-known/openid-configuration\nschemes:\n- name: OAuth2\n  source: https://river.com/.well-known/openid-configuration\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://river.com/oauth2/authorize\n    tokenUrl: https://river.com/oauth2/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token for the subject.\n  flows:\n  - authorizationCode\n- scope: offline_access\n  description: Issue a refresh token for long-lived access without user presence.\n  flows:\n  - authorizationCode\n- scope: balances:read\n  description: Read access to account cash and bitcoin balances.\n  flows:\n  - authorizationCode\n- scope: transactions:read\n  description: Read access to transaction history.\n  flows:\n  - authorizationCode\n- scope: identity:read\n  description: Read access to account holder identity\
  \ information.\n  flows:\n  - authorizationCode\n- scope: payment_networks:read\n  description: Read access to configured payment networks / payout rails.\n  flows:\n  - authorizationCode\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/river-financial/refs/heads/main/scopes/river-financial-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Company
- Bitcoin Services
- Cryptocurrency
- Financial Services
- Banking
- OAuth
- API
token_urls:
- https://river.com/oauth2/token
---
