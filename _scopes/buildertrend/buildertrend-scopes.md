---
api_specs:
- filename: buildertrend-authentication-api-openapi.yml
  format: yaml
  label: Buildertrend Authentication API
  slug: buildertrend-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildertrend/openapi/buildertrend-authentication-api-openapi.yml
- filename: buildertrend-jobs-api-openapi.yml
  format: yaml
  label: Buildertrend Jobs API
  slug: buildertrend-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildertrend/openapi/buildertrend-jobs-api-openapi.yml
- filename: buildertrend-tasks-api-openapi.yml
  format: yaml
  label: Buildertrend Tasks API
  slug: buildertrend-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildertrend/openapi/buildertrend-tasks-api-openapi.yml
- filename: buildertrend-utility-api-openapi.yml
  format: yaml
  label: Buildertrend Utility API
  slug: buildertrend-utility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildertrend/openapi/buildertrend-utility-api-openapi.yml
authorization_urls:
- https://login.buildertrend.com/authorize
description: ''
docs: https://developer.buildertrend.com/apis/open-api
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Buildertrend Scopes
name_suffix: OAuth Scopes
note: The API has no resource-level scopes. What a token can read or write is the permissions of the Buildertrend user (linked account for client credentials; the signed-in person for PKCE). The four scopes above are sign-in (OIDC) scopes from the documented authorize URL.
overview: 'Buildertrend publishes 4 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Buildertrend API on a user''s behalf.


  Tokens are issued from /api/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Buildertrend
provider_slug: buildertrend
schemes:
- description: Client-credentials tokens carry no scopes; access is the permissions of the linked Buildertrend user.
  flows:
  - flow: clientCredentials
    tokenUrl: /api/token
  name: clientCredentials
  scopes: []
  source: openapi/buildertrend-openapi.yml
- flows:
  - authorizationUrl: https://login.buildertrend.com/authorize
    flow: authorizationCode
    tokenUrl: https://login.buildertrend.com/oauth/token
  name: userSignInPkce
  source: openapi/buildertrend-openapi.yml (info.description, PKCE sign-in example)
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: OpenID Connect sign-in scope, requested in the documented PKCE authorize URL.
  flows: []
  scope: openid
- description: OpenID Connect profile claims, requested in the documented PKCE authorize URL.
  flows: []
  scope: profile
- description: OpenID Connect email claim, requested in the documented PKCE authorize URL.
  flows: []
  scope: email
- description: Requests a refresh token (refresh tokens rotate; 30 days, or 15 days without use).
  flows: []
  scope: offline_access
slug: buildertrend-scopes
source_filename: buildertrend-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: searched\nsource: openapi/buildertrend-openapi.yml\ndocs: https://developer.buildertrend.com/apis/open-api\nschemes:\n- name: clientCredentials\n  source: openapi/buildertrend-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /api/token\n  scopes: []\n  description: Client-credentials tokens carry no scopes; access is the permissions of the linked Buildertrend user.\n- name: userSignInPkce\n  source: openapi/buildertrend-openapi.yml (info.description, PKCE sign-in example)\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.buildertrend.com/authorize\n    tokenUrl: https://login.buildertrend.com/oauth/token\nscopes:\n- name: openid\n  scheme: userSignInPkce\n  description: OpenID Connect sign-in scope, requested in the documented PKCE authorize URL.\n- name: profile\n  scheme: userSignInPkce\n  description: OpenID Connect profile claims, requested in the documented PKCE authorize URL.\n- name: email\n\
  \  scheme: userSignInPkce\n  description: OpenID Connect email claim, requested in the documented PKCE authorize URL.\n- name: offline_access\n  scheme: userSignInPkce\n  description: Requests a refresh token (refresh tokens rotate; 30 days, or 15 days without use).\nnote: The API has no resource-level scopes. What a token can read or write is the permissions of the Buildertrend user (linked account for client credentials; the signed-in person for PKCE). The four scopes above are sign-in (OIDC) scopes from the documented authorize URL.\n"
source_yaml_url: https://artifacts.apis.io/buildertrend/scopes/buildertrend-scopes.yml
summary_line: 4 scopes · clientCredentials/authorizationCode
tags:
- Construction
- Construction Management
- Residential Construction
- Home Builders
- Remodeling
- Specialty Contractors
- Project Management
- Job Costing
- Estimating
- Scheduling
- CRM
- Proposals
- Change Orders
- Purchase Orders
- Invoicing
- Client Portal
- Subcontractor Portal
- Mobile App
- Software-as-a-Service
- Vertical SaaS
- Construction Technology
token_bound: false
token_urls:
- /api/token
- https://login.buildertrend.com/oauth/token
---
