---
api_specs:
- filename: trade.yaml
  format: yaml
  label: Saxo Bank OpenAPI
  slug: saxo-bank-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saxo/refs/heads/main/openapi/trade.yaml
authorization_urls:
- https://sim.logonvalidation.net/authorize
description: ''
docs: https://developer.saxobank.com/openapi/learn/security
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Saxo Scopes
name_suffix: OAuth Scopes
note: Saxo Bank OpenAPI does not use OAuth scopes ("scope - Not used" in the authorization code grant docs); access is governed by claims-based access control, with token claims granting Read/Subscribe/Write on resource access levels (https://developer.saxobank.com/openapi/learn/security).
overview: 'Saxo Bank uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://sim.logonvalidation.net/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Saxo Bank
provider_slug: saxo
schemes:
- flows:
  - authorizationUrl: https://sim.logonvalidation.net/authorize
    flow: authorizationCode
    tokenUrl: https://sim.logonvalidation.net/token
  name: OpenApiOAuthSecurityScheme
  source: openapi/at.yaml
- flows:
  - authorizationUrl: https://sim.logonvalidation.net/authorize
    flow: authorizationCode
    tokenUrl: https://sim.logonvalidation.net/token
  name: OpenApiOAuthSecurityScheme
  source: openapi/atr.yaml
- flows:
  - authorizationUrl: https://sim.logonvalidation.net/authorize
    flow: authorizationCode
    tokenUrl: https://sim.logonvalidation.net/token
  name: OpenApiOAuthSecurityScheme
  source: openapi/ca.yaml
- flows:
  - authorizationUrl: https://sim.logonvalidation.net/authorize
    flow: authorizationCode
    tokenUrl: https://sim.logonvalidation.net/token
  name: OpenApiOAuthSecurityScheme
  source: openapi/chart.yaml
- flows:
  - authorizationUrl: https://sim.logonvalidation.net/authorize
    flow: authorizationCode
    tokenUrl: https://sim.logonvalidation.net/token
  name: OpenApiOAuthSecurityScheme
  source: openapi/cm.yaml
- flows:
  - authorizationUrl: https://sim.logonvalidation.net/authorize
    flow: authorizationCode
    tokenUrl: https://sim.logonvalidation.net/token
  name: OpenApiOAuthSecurityScheme
  source: openapi/cr.yaml
- flows:
  - authorizationUrl: https://sim.logonvalidation.net/authorize
    flow: authorizationCode
    tokenUrl: https://sim.logonvalidation.net/token
  name: OpenApiOAuthSecurityScheme
  source: openapi/cs.yaml
- flows:
  - authorizationUrl: https://sim.logonvalidation.net/authorize
    flow: authorizationCode
    tokenUrl: https://sim.logonvalidation.net/token
  name: OpenApiOAuthSecurityScheme
  source: openapi/developer.yaml
- flows:
  - authorizationUrl: https://sim.logonvalidation.net/authorize
    flow: authorizationCode
    tokenUrl: https://sim.logonvalidation.net/token
  name: OpenApiOAuthSecurityScheme
  source: openapi/ens.yaml
- flows:
  - authorizationUrl: https://sim.logonvalidation.net/authorize
    flow: authorizationCode
    tokenUrl: https://sim.logonvalidation.net/token
  name: OpenApiOAuthSecurityScheme
  source: openapi/hist.yaml
- flows:
  - authorizationUrl: https://sim.logonvalidation.net/authorize
    flow: authorizationCode
    tokenUrl: https://sim.logonvalidation.net/token
  name: OpenApiOAuthSecurityScheme
  source: openapi/mkt.yaml
- flows:
  - authorizationUrl: https://sim.logonvalidation.net/authorize
    flow: authorizationCode
    tokenUrl: https://sim.logonvalidation.net/token
  name: OpenApiOAuthSecurityScheme
  source: openapi/partnerintegration.yaml
- flows:
  - authorizationUrl: https://sim.logonvalidation.net/authorize
    flow: authorizationCode
    tokenUrl: https://sim.logonvalidation.net/token
  name: OpenApiOAuthSecurityScheme
  source: openapi/port.yaml
- flows:
  - authorizationUrl: https://sim.logonvalidation.net/authorize
    flow: authorizationCode
    tokenUrl: https://sim.logonvalidation.net/token
  name: OpenApiOAuthSecurityScheme
  source: openapi/ref.yaml
- flows:
  - authorizationUrl: https://sim.logonvalidation.net/authorize
    flow: authorizationCode
    tokenUrl: https://sim.logonvalidation.net/token
  name: OpenApiOAuthSecurityScheme
  source: openapi/root.yaml
- flows:
  - authorizationUrl: https://sim.logonvalidation.net/authorize
    flow: authorizationCode
    tokenUrl: https://sim.logonvalidation.net/token
  name: OpenApiOAuthSecurityScheme
  source: openapi/trade.yaml
- flows:
  - authorizationUrl: https://sim.logonvalidation.net/authorize
    flow: authorizationCode
    tokenUrl: https://sim.logonvalidation.net/token
  name: OpenApiOAuthSecurityScheme
  source: openapi/vas.yaml
scope_count: 0
scope_names: []
scopes: []
slug: saxo-scopes
source_filename: saxo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\ndocs: https://developer.saxobank.com/openapi/learn/security\nnote: Saxo Bank OpenAPI does not use OAuth scopes (\"scope - Not used\" in the authorization\n  code grant docs); access is governed by claims-based access control, with token claims\n  granting Read/Subscribe/Write on resource access levels (https://developer.saxobank.com/openapi/learn/security).\nsource: openapi/at.yaml, openapi/atr.yaml, openapi/ca.yaml, openapi/chart.yaml, openapi/cm.yaml,\n  openapi/cr.yaml, openapi/cs.yaml, openapi/developer.yaml, openapi/ens.yaml, openapi/hist.yaml,\n  openapi/mkt.yaml, openapi/partnerintegration.yaml, openapi/port.yaml, openapi/ref.yaml, openapi/root.yaml,\n  openapi/trade.yaml, openapi/vas.yaml\nschemes:\n- name: OpenApiOAuthSecurityScheme\n  source: openapi/at.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sim.logonvalidation.net/authorize\n    tokenUrl: https://sim.logonvalidation.net/token\n- name: OpenApiOAuthSecurityScheme\n\
  \  source: openapi/atr.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sim.logonvalidation.net/authorize\n    tokenUrl: https://sim.logonvalidation.net/token\n- name: OpenApiOAuthSecurityScheme\n  source: openapi/ca.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sim.logonvalidation.net/authorize\n    tokenUrl: https://sim.logonvalidation.net/token\n- name: OpenApiOAuthSecurityScheme\n  source: openapi/chart.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sim.logonvalidation.net/authorize\n    tokenUrl: https://sim.logonvalidation.net/token\n- name: OpenApiOAuthSecurityScheme\n  source: openapi/cm.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sim.logonvalidation.net/authorize\n    tokenUrl: https://sim.logonvalidation.net/token\n- name: OpenApiOAuthSecurityScheme\n  source: openapi/cr.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sim.logonvalidation.net/authorize\n\
  \    tokenUrl: https://sim.logonvalidation.net/token\n- name: OpenApiOAuthSecurityScheme\n  source: openapi/cs.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sim.logonvalidation.net/authorize\n    tokenUrl: https://sim.logonvalidation.net/token\n- name: OpenApiOAuthSecurityScheme\n  source: openapi/developer.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sim.logonvalidation.net/authorize\n    tokenUrl: https://sim.logonvalidation.net/token\n- name: OpenApiOAuthSecurityScheme\n  source: openapi/ens.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sim.logonvalidation.net/authorize\n    tokenUrl: https://sim.logonvalidation.net/token\n- name: OpenApiOAuthSecurityScheme\n  source: openapi/hist.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sim.logonvalidation.net/authorize\n    tokenUrl: https://sim.logonvalidation.net/token\n- name: OpenApiOAuthSecurityScheme\n  source: openapi/mkt.yaml\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sim.logonvalidation.net/authorize\n    tokenUrl: https://sim.logonvalidation.net/token\n- name: OpenApiOAuthSecurityScheme\n  source: openapi/partnerintegration.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sim.logonvalidation.net/authorize\n    tokenUrl: https://sim.logonvalidation.net/token\n- name: OpenApiOAuthSecurityScheme\n  source: openapi/port.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sim.logonvalidation.net/authorize\n    tokenUrl: https://sim.logonvalidation.net/token\n- name: OpenApiOAuthSecurityScheme\n  source: openapi/ref.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sim.logonvalidation.net/authorize\n    tokenUrl: https://sim.logonvalidation.net/token\n- name: OpenApiOAuthSecurityScheme\n  source: openapi/root.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sim.logonvalidation.net/authorize\n\
  \    tokenUrl: https://sim.logonvalidation.net/token\n- name: OpenApiOAuthSecurityScheme\n  source: openapi/trade.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sim.logonvalidation.net/authorize\n    tokenUrl: https://sim.logonvalidation.net/token\n- name: OpenApiOAuthSecurityScheme\n  source: openapi/vas.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sim.logonvalidation.net/authorize\n    tokenUrl: https://sim.logonvalidation.net/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/saxo/refs/heads/main/scopes/saxo-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Investment Banking
- Trading
- Equities
- Forex
- Options
- Futures
- Market Data
- Portfolio Management
- Orders
- Financial
token_urls:
- https://sim.logonvalidation.net/token
---
