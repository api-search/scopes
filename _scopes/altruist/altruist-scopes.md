---
authorization_urls:
- https://oauth.stage1.altruistnet.tech/api/oauth2/authorize
description: ''
docs: https://developer.altruist.com/docs/open-api-authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Altruist Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Altruist publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Altruist API on a user''s behalf.


  Tokens are issued from https://openapi.altruist.com/altruist-open-api/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Altruist
provider_slug: altruist
schemes:
- api: Altruist Open API
  flows:
  - authorizationUrl: https://oauth.stage1.altruistnet.tech/api/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://openapi.altruist.com/altruist-open-api/oauth2/token
  name: OpenAPI-OAuth2-AuthorizationCode
scope_count: 1
scope_names:
- openid
scopes:
- description: OpenID Connect scope requested during the Open API authorization-code flow; yields an ID/access token used as the Authorization header for subsequent Open API requests. Altruist documents `scope=openid` as the value to send on the authorization request.
  flows:
  - authorizationCode
  scope: openid
slug: altruist-scopes
source_filename: altruist-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://developer.altruist.com/docs/open-api-authentication\ndocs: https://developer.altruist.com/docs/open-api-authentication\nschemes:\n- name: OpenAPI-OAuth2-AuthorizationCode\n  api: Altruist Open API\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth.stage1.altruistnet.tech/api/oauth2/authorize\n    tokenUrl: https://openapi.altruist.com/altruist-open-api/oauth2/token\nscopes:\n- scope: openid\n  description: >-\n    OpenID Connect scope requested during the Open API authorization-code flow;\n    yields an ID/access token used as the Authorization header for subsequent\n    Open API requests. Altruist documents `scope=openid` as the value to send on\n    the authorization request.\n  flows: [authorizationCode]\n  sources: [https://developer.altruist.com/docs/open-api-authentication]\nnotes: >-\n  Altruist does not publish a granular scope/permission catalog. The Open API\n  authorization request\
  \ documents a single `openid` scope; access to resources\n  is governed by the partner integration grant and the Altruist user's own\n  permissions rather than fine-grained OAuth scopes. The Realtime API uses a\n  password grant with no scope parameter documented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/altruist/refs/heads/main/scopes/altruist-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Fintech
- Custody
- Wealth Management
- Financial Advisors
- RIA
- Investing
- OAuth
token_urls:
- https://openapi.altruist.com/altruist-open-api/oauth2/token
---
