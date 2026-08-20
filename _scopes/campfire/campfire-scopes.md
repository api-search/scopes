---
api_specs:
- filename: campfire-accounts-payable-api-openapi.yml
  format: yaml
  label: Campfire Accounts Payable API
  slug: campfire-accounts-payable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-accounts-payable-api-openapi.yml
- filename: campfire-accounts-receivable-api-openapi.yml
  format: yaml
  label: Campfire Accounts Receivable API
  slug: campfire-accounts-receivable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-accounts-receivable-api-openapi.yml
- filename: campfire-bank-reconciliation-api-openapi.yml
  format: yaml
  label: Campfire Bank Reconciliation API
  slug: campfire-bank-reconciliation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-bank-reconciliation-api-openapi.yml
- filename: campfire-cash-management-api-openapi.yml
  format: yaml
  label: Campfire Cash Management API
  slug: campfire-cash-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-cash-management-api-openapi.yml
- filename: campfire-coa-api-openapi.yml
  format: yaml
  label: Campfire coa API
  slug: campfire-coa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-coa-api-openapi.yml
- filename: campfire-company-objects-api-openapi.yml
  format: yaml
  label: Campfire Company Objects API
  slug: campfire-company-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-company-objects-api-openapi.yml
- filename: campfire-core-accounting-api-openapi.yml
  format: yaml
  label: Campfire Core Accounting API
  slug: campfire-core-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-core-accounting-api-openapi.yml
- filename: campfire-custom-fields-api-openapi.yml
  format: yaml
  label: Campfire Custom Fields API
  slug: campfire-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-custom-fields-api-openapi.yml
- filename: campfire-financial-statements-api-openapi.yml
  format: yaml
  label: Campfire Financial Statements API
  slug: campfire-financial-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-financial-statements-api-openapi.yml
- filename: campfire-integrations-api-openapi.yml
  format: yaml
  label: Campfire Integrations API
  slug: campfire-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-integrations-api-openapi.yml
- filename: campfire-revenue-recognition-api-openapi.yml
  format: yaml
  label: Campfire Revenue Recognition API
  slug: campfire-revenue-recognition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-revenue-recognition-api-openapi.yml
- filename: campfire-settings-api-openapi.yml
  format: yaml
  label: Campfire Settings API
  slug: campfire-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-settings-api-openapi.yml
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
- Artificial Intelligence
token_urls:
- https://api.meetcampfire.com/auth/token
---
