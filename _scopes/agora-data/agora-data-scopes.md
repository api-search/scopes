---
api_specs:
- filename: agora-data-health-api-openapi.yml
  format: yaml
  label: Agora Data Health API
  slug: agora-data-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/openapi/agora-data-health-api-openapi.yml
- filename: agora-data-hooks-api-openapi.yml
  format: yaml
  label: Agora Data Hooks API
  slug: agora-data-hooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/openapi/agora-data-hooks-api-openapi.yml
- filename: agora-data-import-api-openapi.yml
  format: yaml
  label: Agora Data Import API
  slug: agora-data-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/openapi/agora-data-import-api-openapi.yml
- filename: agora-data-inventory-api-openapi.yml
  format: yaml
  label: Agora Data Inventory API
  slug: agora-data-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/openapi/agora-data-inventory-api-openapi.yml
- filename: agora-data-loans-api-openapi.yml
  format: yaml
  label: Agora Data Loans API
  slug: agora-data-loans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/openapi/agora-data-loans-api-openapi.yml
- filename: agora-data-login-api-openapi.yml
  format: yaml
  label: Agora Data Login API
  slug: agora-data-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/openapi/agora-data-login-api-openapi.yml
- filename: agora-data-oauth-api-openapi.yml
  format: yaml
  label: Agora Data OAUTH API
  slug: agora-data-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/openapi/agora-data-oauth-api-openapi.yml
- filename: agora-data-providers-api-openapi.yml
  format: yaml
  label: Agora Data Providers API
  slug: agora-data-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/openapi/agora-data-providers-api-openapi.yml
- filename: agora-data-status-api-openapi.yml
  format: yaml
  label: Agora Data Status API
  slug: agora-data-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/openapi/agora-data-status-api-openapi.yml
- filename: agora-data-uploads-api-openapi.yml
  format: yaml
  label: Agora Data Uploads API
  slug: agora-data-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/openapi/agora-data-uploads-api-openapi.yml
authorization_urls:
- https://agora-data.us.auth0.com/authorize
- https://api.agoradata.com/oauth/authorize
description: ''
docs: https://agora-data.us.auth0.com/.well-known/openid-configuration
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Agora Data Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Agora Data publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Agora Data API on a user''s behalf.


  Tokens are issued from https://agora-data.us.auth0.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Agora Data
provider_slug: agora-data
schemes:
- flows:
  - authorizationUrl: https://agora-data.us.auth0.com/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://agora-data.us.auth0.com/oauth/token
  issuer: https://agora-data.us.auth0.com/
  name: agora-portal-oidc
  source: well-known/agora-data-openid-configuration.json
- flows:
  - authorizationUrl: https://api.agoradata.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.agoradata.com/oauth/token
  name: agora-api-oauth
  scopes_published: false
  source: openapi/agora-data-openapi-original.json
scope_count: 6
scope_names:
- openid
- profile
- email
- offline_access
- address
- phone
scopes:
- description: Request an OIDC ID token.
  flows:
  - authorizationCode
  scope: openid
- description: Basic profile claims (name, given_name, family_name, nickname, picture).
  flows:
  - authorizationCode
  scope: profile
- description: Email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Issue a refresh token so the portal session can be renewed.
  flows:
  - authorizationCode
  scope: offline_access
- description: Address claim.
  flows:
  - authorizationCode
  scope: address
- description: Phone number claim.
  flows:
  - authorizationCode
  scope: phone
slug: agora-data-scopes
source_filename: agora-data-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nsource: well-known/agora-data-openid-configuration.json\ndocs: https://agora-data.us.auth0.com/.well-known/openid-configuration\nnotes: >-\n  Agora Data's loan-import API at api.agoradata.com hosts its own /oauth/authorize and\n  /oauth/token endpoints and returns a `scope` field on TokenRequestResponse, but it\n  publishes NO scope vocabulary — the OpenAPI declares no oauth2 securityScheme and no\n  flow `scopes` map, and there is no public scopes/permissions reference page. The only\n  scope vocabulary Agora Data actually publishes is the standard OIDC set advertised by\n  the Auth0 tenant that fronts AgoraPortal. Those are identity scopes for the portal, not\n  authorization scopes for the loan-import API. Nothing below is invented; the API's own\n  scope vocabulary remains undocumented.\nschemes:\n- name: agora-portal-oidc\n  source: well-known/agora-data-openid-configuration.json\n  issuer: https://agora-data.us.auth0.com/\n \
  \ flows:\n  - flow: authorizationCode\n    authorizationUrl: https://agora-data.us.auth0.com/authorize\n    tokenUrl: https://agora-data.us.auth0.com/oauth/token\n    pkce: S256\n- name: agora-api-oauth\n  source: openapi/agora-data-openapi-original.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.agoradata.com/oauth/authorize\n    tokenUrl: https://api.agoradata.com/oauth/token\n  scopes_published: false\nscopes:\n- scope: openid\n  description: Request an OIDC ID token.\n  flows: [authorizationCode]\n  sources: [well-known/agora-data-openid-configuration.json]\n- scope: profile\n  description: Basic profile claims (name, given_name, family_name, nickname, picture).\n  flows: [authorizationCode]\n  sources: [well-known/agora-data-openid-configuration.json]\n- scope: email\n  description: Email address and email_verified claim.\n  flows: [authorizationCode]\n  sources: [well-known/agora-data-openid-configuration.json]\n- scope: offline_access\n  description:\
  \ Issue a refresh token so the portal session can be renewed.\n  flows: [authorizationCode]\n  sources: [well-known/agora-data-openid-configuration.json]\n- scope: address\n  description: Address claim.\n  flows: [authorizationCode]\n  sources: [well-known/agora-data-openid-configuration.json]\n- scope: phone\n  description: Phone number claim.\n  flows: [authorizationCode]\n  sources: [well-known/agora-data-openid-configuration.json]\nobserved_portal_request:\n  audience: dealer-portal\n  scope: openid profile email offline_access\n  source: https://portal.agoradata.com/ 302 redirect\ngaps:\n- The loan-import API returns a `scope` on its token response but publishes no scope vocabulary.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/scopes/agora-data-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Company
- Auto Finance
- Automotive
- Lending
- Financial-Services
- Fintech
- Loan Origination
- Data Analytics
- Artificial Intelligence
- Capital Markets
token_urls:
- https://agora-data.us.auth0.com/oauth/token
- https://api.agoradata.com/oauth/token
---
