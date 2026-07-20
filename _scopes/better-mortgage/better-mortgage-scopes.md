---
authorization_urls:
- https://prod.bettermg.com/api/idp/sso
description: ''
docs: https://www.better.com/.well-known/openid-configuration
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Better Mortgage Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Better Mortgage publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Better Mortgage API on a user''s behalf.


  Tokens are issued from https://prod.bettermg.com/api/idp/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Better Mortgage
provider_slug: better-mortgage
schemes:
- flows:
  - authorizationUrl: https://prod.bettermg.com/api/idp/sso
    flow: authorizationCode
    tokenUrl: https://prod.bettermg.com/api/idp/token
  name: OpenIDConnect
  source: well-known/better-mortgage-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- phone
- profile
scopes:
- description: OpenID Connect authentication; required to obtain an ID token.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the user's email address claim.
  flows:
  - authorizationCode
  scope: email
- description: Access to the user's phone number claim.
  flows:
  - authorizationCode
  scope: phone
- description: Access to the user's basic profile claims.
  flows:
  - authorizationCode
  scope: profile
slug: better-mortgage-scopes
source_filename: better-mortgage-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.better.com/.well-known/openid-configuration\ndocs: https://www.better.com/.well-known/openid-configuration\nschemes:\n- name: OpenIDConnect\n  source: well-known/better-mortgage-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://prod.bettermg.com/api/idp/sso\n    tokenUrl: https://prod.bettermg.com/api/idp/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; required to obtain an ID token.\n  flows: [authorizationCode]\n  sources: [well-known/better-mortgage-openid-configuration.json]\n- scope: email\n  description: Access to the user's email address claim.\n  flows: [authorizationCode]\n  sources: [well-known/better-mortgage-openid-configuration.json]\n- scope: phone\n  description: Access to the user's phone number claim.\n  flows: [authorizationCode]\n  sources: [well-known/better-mortgage-openid-configuration.json]\n- scope: profile\n  description:\
  \ Access to the user's basic profile claims.\n  flows: [authorizationCode]\n  sources: [well-known/better-mortgage-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/better-mortgage/refs/heads/main/scopes/better-mortgage-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Fintech
- Mortgage
- Lending
- Real Estate
- Home Finance
- HELOC
- OpenID Connect
token_urls:
- https://prod.bettermg.com/api/idp/token
---
