---
authorization_urls: []
description: ''
docs: https://developer.wealth.com/advisor/authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Wealthcom Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Wealth.com publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Wealth.com API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Wealth.com
provider_slug: wealthcom
schemes:
- api: Wealth.com Advisor API
  flows:
  - flow: authorizationCode
    note: Authorization/token URLs not published in public docs; discovered via advisor onboarding.
    pkce: true
  name: AdvisorOAuth2
scope_count: 3
scope_names:
- openid
- email
- profile
scopes:
- description: OpenID Connect authentication; issue an ID token for the signed-in advisor user.
  flows:
  - authorizationCode
  scope: openid
- description: Access the advisor user's email address claim.
  flows:
  - authorizationCode
  scope: email
- description: Access the advisor user's basic profile claims.
  flows:
  - authorizationCode
  scope: profile
slug: wealthcom-scopes
source_filename: wealthcom-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.wealth.com/advisor/authentication\ndocs: https://developer.wealth.com/advisor/authentication\nschemes:\n- name: AdvisorOAuth2\n  api: Wealth.com Advisor API\n  flows:\n  - flow: authorizationCode\n    pkce: true\n    note: Authorization/token URLs not published in public docs; discovered via advisor onboarding.\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token for the signed-in advisor user.\n  flows: [authorizationCode]\n- scope: email\n  description: Access the advisor user's email address claim.\n  flows: [authorizationCode]\n- scope: profile\n  description: Access the advisor user's basic profile claims.\n  flows: [authorizationCode]\nnotes: >-\n  Wealth.com documents the standard OpenID Connect scopes (openid, email, profile) plus\n  \"any custom configured scopes\" negotiated per integration. A full custom-scope reference\n  is not published on the public developer\
  \ portal.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wealthcom/refs/heads/main/scopes/wealthcom-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- Enterprise
- Estate Planning
- Tax Planning
- Wealth Management
- Financial Advisors
- Fintech
- Artificial Intelligence
token_urls: []
---
