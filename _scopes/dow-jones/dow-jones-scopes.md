---
api_specs:
- filename: dow-jones-screening-and-monitoring-api-openapi.json
  format: json
  label: Dow Jones Screening and Monitoring API
  slug: screening-and-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones/refs/heads/main/openapi/dow-jones-screening-and-monitoring-api-openapi.json
- filename: dow-jones-screening-and-monitoring-private-lists-api-openapi.json
  format: json
  label: Dow Jones Screening and Monitoring Private Lists API
  slug: screening-and-monitoring-private-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones/refs/heads/main/openapi/dow-jones-screening-and-monitoring-private-lists-api-openapi.json
- filename: dow-jones-advanced-screening-and-monitoring-api-openapi.json
  format: json
  label: Dow Jones Advanced Screening and Monitoring API
  slug: advanced-screening-and-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones/refs/heads/main/openapi/dow-jones-advanced-screening-and-monitoring-api-openapi.json
- filename: dow-jones-risk-search-api-openapi.json
  format: json
  label: Dow Jones Risk Search API
  slug: risk-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones/refs/heads/main/openapi/dow-jones-risk-search-api-openapi.json
- filename: dow-jones-risk-profiles-api-openapi.json
  format: json
  label: Dow Jones Risk Profiles API
  slug: risk-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones/refs/heads/main/openapi/dow-jones-risk-profiles-api-openapi.json
- filename: dow-jones-risk-taxonomy-api-openapi.json
  format: json
  label: Dow Jones Risk Taxonomy API
  slug: risk-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones/refs/heads/main/openapi/dow-jones-risk-taxonomy-api-openapi.json
- filename: dow-jones-profile-version-history-api-openapi.json
  format: json
  label: Dow Jones Profile Version History API
  slug: profile-version-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones/refs/heads/main/openapi/dow-jones-profile-version-history-api-openapi.json
- filename: dow-jones-due-diligence-reports-api-openapi.json
  format: json
  label: Dow Jones Due Diligence Reports API
  slug: due-diligence-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones/refs/heads/main/openapi/dow-jones-due-diligence-reports-api-openapi.json
- filename: dow-jones-riskcenter-third-party-api-0-2-openapi.json
  format: json
  label: Dow Jones RiskCenter Third Party Platform API
  slug: riskcenter-third-party-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones/refs/heads/main/openapi/dow-jones-riskcenter-third-party-api-0-2-openapi.json
- filename: dow-jones-newswires-real-time-api-openapi.json
  format: json
  label: Dow Jones Newswires Real-Time API
  slug: newswires-real-time-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones/refs/heads/main/openapi/dow-jones-newswires-real-time-api-openapi.json
- filename: dow-jones-top-stories-api-openapi.json
  format: json
  label: Dow Jones Top Stories API
  slug: top-stories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones/refs/heads/main/openapi/dow-jones-top-stories-api-openapi.json
- filename: dow-jones-calendar-live-api-openapi.json
  format: json
  label: Dow Jones Calendar Live API
  slug: calendar-live-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones/refs/heads/main/openapi/dow-jones-calendar-live-api-openapi.json
- filename: dow-jones-newswires-content-api-openapi.json
  format: json
  label: Dow Jones Newswires Content API
  slug: newswires-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones/refs/heads/main/openapi/dow-jones-newswires-content-api-openapi.json
- filename: dow-jones-content-api-swagger.json
  format: json
  label: Dow Jones Content API
  slug: content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones/refs/heads/main/openapi/dow-jones-content-api-swagger.json
- filename: dow-jones-newsletters-api-openapi.json
  format: json
  label: Dow Jones Factiva Newsletters API
  slug: newsletters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones/refs/heads/main/openapi/dow-jones-newsletters-api-openapi.json
- filename: dow-jones-company-news-radar-api-openapi.json
  format: json
  label: Dow Jones Company News Radar API
  slug: company-news-radar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones/refs/heads/main/openapi/dow-jones-company-news-radar-api-openapi.json
authorization_urls:
- https://sso.accounts.dowjones.com/authorize
description: ''
docs: https://developer.dowjones.com/documents/factiva_integration-essentials-authentication
flows:
- authorizationCode
- implicit
- password
- jwt-bearer
- refresh_token
kind: oauth-scopes
layout: scope
method: searched
name: Dow Jones Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Dow Jones publishes 7 OAuth 2.0 scopes via the authorizationCode, implicit, password, jwt-bearer, and refresh_token flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Dow Jones API on a user''s behalf.


  Tokens are issued from https://sso.accounts.dowjones.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Dow Jones
provider_slug: dow-jones
schemes:
- discovery: https://accounts.dowjones.com/.well-known/openid-configuration
  flows:
  - authorizationUrl: https://sso.accounts.dowjones.com/authorize
    flow: authorizationCode
    tokenUrl: https://sso.accounts.dowjones.com/oauth/token
  - authorizationUrl: https://sso.accounts.dowjones.com/authorize
    flow: implicit
  - flow: password
    note: Service Account Integration (connection=service-account) exchanges service-account credentials for AuthN tokens.
    tokenUrl: https://accounts.dowjones.com/oauth2/v1/token
  - flow: jwt-bearer
    note: grant_type urn:ietf:params:oauth:grant-type:jwt-bearer exchanges the AuthN ID token for the AuthZ access token.
    tokenUrl: https://accounts.dowjones.com/oauth2/v1/token
  - flow: refresh_token
    tokenUrl: https://accounts.dowjones.com/oauth2/v1/token
  issuer: https://sso.accounts.dowjones.com/
  name: Dow Jones Identity Service (OAuth 2.0 / OIDC)
scope_count: 7
scope_names:
- openid
- email
- given_name
- family_name
- offline_access
- service_account_id
- pib
scopes:
- description: Access your identity in Factiva. Provides the ID token (JWT).
  flows: []
  scope: openid
- description: View your email address. Provides the user's email in the ID token.
  flows: []
  scope: email
- description: View your given name in the ID token.
  flows: []
  scope: given_name
- description: View your family name in the ID token.
  flows: []
  scope: family_name
- description: Indicates that a Refresh token is returned.
  flows: []
  scope: offline_access
- description: Requests the AuthN tokens for a service account (used with the password grant, connection=service-account).
  flows: []
  scope: service_account_id
- description: Requested together with openid when exchanging AuthN tokens for the AuthZ access token that calls the APIs (scope value "openid pib").
  flows: []
  scope: pib
slug: dow-jones-scopes
source_filename: dow-jones-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: https://developer.dowjones.com/documents/site-docs-getting_started-sessions_and_authentication-dow_jones_identity_service\ndocs: https://developer.dowjones.com/documents/factiva_integration-essentials-authentication\nschemes:\n  - name: Dow Jones Identity Service (OAuth 2.0 / OIDC)\n    issuer: https://sso.accounts.dowjones.com/\n    discovery: https://accounts.dowjones.com/.well-known/openid-configuration\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://sso.accounts.dowjones.com/authorize\n        tokenUrl: https://sso.accounts.dowjones.com/oauth/token\n      - flow: implicit\n        authorizationUrl: https://sso.accounts.dowjones.com/authorize\n      - flow: password\n        tokenUrl: https://accounts.dowjones.com/oauth2/v1/token\n        note: Service Account Integration (connection=service-account) exchanges service-account credentials for AuthN tokens.\n      - flow: jwt-bearer\n      \
  \  tokenUrl: https://accounts.dowjones.com/oauth2/v1/token\n        note: 'grant_type urn:ietf:params:oauth:grant-type:jwt-bearer exchanges the AuthN ID token for the AuthZ access token.'\n      - flow: refresh_token\n        tokenUrl: https://accounts.dowjones.com/oauth2/v1/token\nscopes:\n  - scope: openid\n    description: Access your identity in Factiva. Provides the ID token (JWT).\n  - scope: email\n    description: View your email address. Provides the user's email in the ID token.\n  - scope: given_name\n    description: View your given name in the ID token.\n  - scope: family_name\n    description: View your family name in the ID token.\n  - scope: offline_access\n    description: Indicates that a Refresh token is returned.\n  - scope: service_account_id\n    description: Requests the AuthN tokens for a service account (used with the password grant, connection=service-account).\n  - scope: pib\n    description: Requested together with openid when exchanging AuthN tokens for the\
  \ AuthZ access token that calls the APIs (scope value \"openid pib\").\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dow-jones/refs/heads/main/scopes/dow-jones-scopes.yml
summary_line: 7 scopes · authorizationCode/implicit/password/jwt-bearer/refresh_token
tags:
- Financial
- Market Data
- News
- Publishing
- Risk and Compliance
- Screening
- Due Diligence
- Media Monitoring
token_urls:
- https://sso.accounts.dowjones.com/oauth/token
- https://accounts.dowjones.com/oauth2/v1/token
---
