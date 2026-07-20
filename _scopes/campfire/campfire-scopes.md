---
api_specs:
- filename: campfire-openapi-original.json
  format: json
  label: Campfire Developer APIs
  slug: campfire-developer-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-openapi-original.json
authorization_urls:
- https://api.meetcampfire.com/auth/authorize
description: ''
docs: https://docs.campfire.ai/quickstart
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Campfire Scopes
name_suffix: OAuth Scopes
note: Campfire's OpenAPI declares only the Token (apiKey) scheme, but the API host publishes OAuth 2.0 Authorization Server + OIDC discovery metadata advertising an authorization_code + client_credentials OAuth surface with the three OIDC scopes below. API-token roles (admin / clerk / view-only, set per API user in Settings > API Keys) provide the coarse permission model for Token auth.
overview: 'Campfire publishes 3 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Campfire API on a user''s behalf.


  Tokens are issued from https://api.meetcampfire.com/auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Campfire
provider_slug: campfire
schemes:
- flows:
  - authorizationUrl: https://api.meetcampfire.com/auth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://api.meetcampfire.com/auth/token
  - flow: clientCredentials
    tokenUrl: https://api.meetcampfire.com/auth/token
  name: OAuth2 / OIDC
  registration_endpoint: https://api.meetcampfire.com/auth/register
  source: https://api.meetcampfire.com/.well-known/oauth-authorization-server
scope_count: 3
scope_names:
- openid
- email
- profile
scopes:
- description: OpenID Connect sign-in; issues an ID token identifying the authenticated user.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the user's email address claim.
  flows:
  - authorizationCode
  scope: email
- description: Access to the user's basic profile claims.
  flows:
  - authorizationCode
  scope: profile
slug: campfire-scopes
source_filename: campfire-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://api.meetcampfire.com/.well-known/openid-configuration\ndocs: https://docs.campfire.ai/quickstart\nnote: >\n  Campfire's OpenAPI declares only the Token (apiKey) scheme, but the API host\n  publishes OAuth 2.0 Authorization Server + OIDC discovery metadata advertising\n  an authorization_code + client_credentials OAuth surface with the three OIDC\n  scopes below. API-token roles (admin / clerk / view-only, set per API user in\n  Settings > API Keys) provide the coarse permission model for Token auth.\nschemes:\n  - name: OAuth2 / OIDC\n    source: https://api.meetcampfire.com/.well-known/oauth-authorization-server\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://api.meetcampfire.com/auth/authorize\n        tokenUrl: https://api.meetcampfire.com/auth/token\n        pkce: S256\n      - flow: clientCredentials\n        tokenUrl: https://api.meetcampfire.com/auth/token\n    registration_endpoint:\
  \ https://api.meetcampfire.com/auth/register\nscopes:\n  - scope: openid\n    description: OpenID Connect sign-in; issues an ID token identifying the authenticated user.\n    flows: [authorizationCode]\n  - scope: email\n    description: Access to the user's email address claim.\n    flows: [authorizationCode]\n  - scope: profile\n    description: Access to the user's basic profile claims.\n    flows: [authorizationCode]\ntoken_roles:\n  - role: admin\n    grants: All APIs\n  - role: clerk\n    grants: View all APIs and post draft entries\n  - role: view only\n    grants: GET (read-only) APIs\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/scopes/campfire-scopes.yml
summary_line: 3 scopes · authorizationCode/clientCredentials
tags:
- Company
- Accounting
- ERP
- Finance
- Revenue Recognition
- Accounts Payable
- Accounts Receivable
- AI
token_urls:
- https://api.meetcampfire.com/auth/token
---
