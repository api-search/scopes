---
authorization_urls:
- https://secure.blueleaf.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Blueleaf Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'BlueLeaf publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the BlueLeaf API on a user''s behalf.


  Tokens are issued from https://secure.blueleaf.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: BlueLeaf
provider_slug: blueleaf
schemes:
- flows:
  - authorizationUrl: https://secure.blueleaf.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://secure.blueleaf.com/oauth/token
  name: OAuth2
  source: well-known/blueleaf-openid-configuration.json
scope_count: 3
scope_names:
- openid
- email
- profile
scopes:
- description: OpenID Connect authentication; issue an ID token for the end user.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the user's email and email_verified claims.
  flows:
  - authorizationCode
  scope: email
- description: Access to profile claims (name, given_name, family_name, preferred_username, bl_id, firm_id, firm_name, role).
  flows:
  - authorizationCode
  scope: profile
slug: blueleaf-scopes
source_filename: blueleaf-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://secure.blueleaf.com/.well-known/openid-configuration\nschemes:\n- name: OAuth2\n  source: well-known/blueleaf-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://secure.blueleaf.com/oauth/authorize\n    tokenUrl: https://secure.blueleaf.com/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token for the end user.\n  flows: [authorizationCode]\n  sources: [well-known/blueleaf-openid-configuration.json]\n- scope: email\n  description: Access to the user's email and email_verified claims.\n  flows: [authorizationCode]\n  sources: [well-known/blueleaf-openid-configuration.json]\n- scope: profile\n  description: Access to profile claims (name, given_name, family_name, preferred_username, bl_id, firm_id, firm_name, role).\n  flows: [authorizationCode]\n  sources: [well-known/blueleaf-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blueleaf/refs/heads/main/scopes/blueleaf-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- Wealth Management
- Fintech
- Financial Advisors
- Investment Reporting
- Account Aggregation
- Client Portal
- OAuth
- OpenID Connect
token_urls:
- https://secure.blueleaf.com/oauth/token
---
