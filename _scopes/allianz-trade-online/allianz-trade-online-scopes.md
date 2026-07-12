---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Allianz Trade Online Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Allianz Trade publishes 8 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Allianz Trade API on a user''s behalf.


  Tokens are issued from https://api.allianz-trade.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Allianz Trade
provider_slug: allianz-trade-online
schemes:
- description: OAuth2 client credentials for Allianz Trade API access
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.allianz-trade.com/oauth2/token
  name: OAuth2
  source: openapi/allianz-trade-claims.yaml
- description: OAuth2 client credentials for Allianz Trade API access
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.allianz-trade.com/oauth2/token
  name: OAuth2
  source: openapi/allianz-trade-company-grade.yaml
- description: OAuth2 client credentials for Allianz Trade API access
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.allianz-trade.com/oauth2/token
  name: OAuth2
  source: openapi/allianz-trade-payment-overdues.yaml
- description: OAuth2 client credentials for Allianz Trade API access
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.allianz-trade.com/oauth2/token
  name: OAuth2
  source: openapi/allianz-trade-policy.yaml
scope_count: 8
scope_names:
- claims:read
- claims:write
- grades:read
- grades:write
- overdues:read
- overdues:write
- policy:read
- policy:write
scopes:
- description: Read insurance claims
  flows:
  - clientCredentials
  scope: claims:read
- description: Submit and manage insurance claims
  flows:
  - clientCredentials
  scope: claims:write
- description: Read company grades
  flows:
  - clientCredentials
  scope: grades:read
- description: Request company grades
  flows:
  - clientCredentials
  scope: grades:write
- description: Read payment overdues
  flows:
  - clientCredentials
  scope: overdues:read
- description: Report and manage payment overdues
  flows:
  - clientCredentials
  scope: overdues:write
- description: Read policy details
  flows:
  - clientCredentials
  scope: policy:read
- description: Manage policy configurations
  flows:
  - clientCredentials
  scope: policy:write
slug: allianz-trade-online-scopes
source_filename: allianz-trade-online-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/allianz-trade-claims.yaml, openapi/allianz-trade-company-grade.yaml, openapi/allianz-trade-payment-overdues.yaml,\n  openapi/allianz-trade-policy.yaml\nschemes:\n- name: OAuth2\n  source: openapi/allianz-trade-claims.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.allianz-trade.com/oauth2/token\n  description: OAuth2 client credentials for Allianz Trade API access\n- name: OAuth2\n  source: openapi/allianz-trade-company-grade.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.allianz-trade.com/oauth2/token\n  description: OAuth2 client credentials for Allianz Trade API access\n- name: OAuth2\n  source: openapi/allianz-trade-payment-overdues.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.allianz-trade.com/oauth2/token\n  description: OAuth2 client credentials for Allianz Trade API access\n- name: OAuth2\n  source: openapi/allianz-trade-policy.yaml\n  flows:\n\
  \  - flow: clientCredentials\n    tokenUrl: https://api.allianz-trade.com/oauth2/token\n  description: OAuth2 client credentials for Allianz Trade API access\nscopes:\n- scope: claims:read\n  description: Read insurance claims\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/allianz-trade-claims.yaml\n- scope: claims:write\n  description: Submit and manage insurance claims\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/allianz-trade-claims.yaml\n- scope: grades:read\n  description: Read company grades\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/allianz-trade-company-grade.yaml\n- scope: grades:write\n  description: Request company grades\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/allianz-trade-company-grade.yaml\n- scope: overdues:read\n  description: Read payment overdues\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/allianz-trade-payment-overdues.yaml\n- scope: overdues:write\n  description: Report and manage payment overdues\n\
  \  flows:\n  - clientCredentials\n  sources:\n  - openapi/allianz-trade-payment-overdues.yaml\n- scope: policy:read\n  description: Read policy details\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/allianz-trade-policy.yaml\n- scope: policy:write\n  description: Manage policy configurations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/allianz-trade-policy.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allianz-trade-online/refs/heads/main/scopes/allianz-trade-online-scopes.yml
summary_line: 8 scopes · clientCredentials
tags:
- Credit Insurance
- Insurance
- Risk Management
- Trade Credit
- E-Commerce
- Surety
token_urls:
- https://api.allianz-trade.com/oauth2/token
---
