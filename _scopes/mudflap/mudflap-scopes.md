---
authorization_urls:
- https://api.mudflapinc.com/oauth/authorize
description: ''
docs: https://api.mudflapinc.com/.well-known/oauth-authorization-server
flows:
- authorizationCode
- password
kind: oauth-scopes
layout: scope
method: searched
name: Mudflap Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Mudflap publishes 3 OAuth 2.0 scopes via the authorizationCode and password flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Mudflap API on a user''s behalf.


  Tokens are issued from https://api.mudflapinc.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Mudflap
provider_slug: mudflap
schemes:
- flows:
  - authorizationUrl: https://api.mudflapinc.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.mudflapinc.com/oauth/token
  - flow: password
    tokenUrl: https://api.mudflapinc.com/oauth/token
  name: OAuth2
  source: https://api.mudflapinc.com/.well-known/oauth-authorization-server
scope_count: 3
scope_names:
- openid
- profile
- email
scopes:
- description: OpenID Connect authentication; issue an id_token identifying the end user.
  flows:
  - authorizationCode
  - password
  scope: openid
- description: Access to the end user's basic profile claims (name, preferred_username).
  flows:
  - authorizationCode
  - password
  scope: profile
- description: Access to the end user's email address claim.
  flows:
  - authorizationCode
  - password
  scope: email
slug: mudflap-scopes
source_filename: mudflap-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://api.mudflapinc.com/.well-known/oauth-authorization-server\ndocs: https://api.mudflapinc.com/.well-known/oauth-authorization-server\nschemes:\n- name: OAuth2\n  source: https://api.mudflapinc.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.mudflapinc.com/oauth/authorize\n    tokenUrl: https://api.mudflapinc.com/oauth/token\n  - flow: password\n    tokenUrl: https://api.mudflapinc.com/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an id_token identifying the end user.\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - https://api.mudflapinc.com/.well-known/oauth-authorization-server\n- scope: profile\n  description: Access to the end user's basic profile claims (name, preferred_username).\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - https://api.mudflapinc.com/.well-known/oauth-authorization-server\n\
  - scope: email\n  description: Access to the end user's email address claim.\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - https://api.mudflapinc.com/.well-known/oauth-authorization-server\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mudflap/refs/heads/main/scopes/mudflap-scopes.yml
summary_line: 3 scopes · authorizationCode/password
tags:
- Company
- Fintech
- Fuel
- Trucking
- Payments
- Fleet Management
- Logistics
- Fuel Card
token_urls:
- https://api.mudflapinc.com/oauth/token
---
