---
api_specs:
- filename: altoira-handoffs-api-openapi.yml
  format: yaml
  label: AltoIRA Handoffs API
  slug: altoira-handoffs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altoira/refs/heads/main/openapi/altoira-handoffs-api-openapi.yml
- filename: altoira-investment-api-openapi.yml
  format: yaml
  label: AltoIRA Investment API
  slug: altoira-investment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altoira/refs/heads/main/openapi/altoira-investment-api-openapi.yml
- filename: altoira-oauth-api-openapi.yml
  format: yaml
  label: AltoIRA OAUTH API
  slug: altoira-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altoira/refs/heads/main/openapi/altoira-oauth-api-openapi.yml
- filename: altoira-offering-api-openapi.yml
  format: yaml
  label: AltoIRA Offering API
  slug: altoira-offering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altoira/refs/heads/main/openapi/altoira-offering-api-openapi.yml
- filename: altoira-user-api-openapi.yml
  format: yaml
  label: AltoIRA User API
  slug: altoira-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altoira/refs/heads/main/openapi/altoira-user-api-openapi.yml
authorization_urls:
- https://altoira.sandbox.altoira.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Altoira Scopes
name_suffix: OAuth Scopes
note: The partner API's oauth2 authorizationCode flow declares an EMPTY scopes map, and Alto's developer hub documents no scope reference page. The /oauth/authorize operation accepts a `scope` query parameter but no permitted values are published, so an integrator cannot determine what to send. This is a provider-fixable documentation gap. Separately, Alto runs an Auth0 tenant at auth.altoira.com for the investor/issuer web application which DOES publish scopes_supported (openid, profile, offline_access, name, given_name, family_name, nickname, email, email_verified, picture, created_at, identities, phone, address). That is a DIFFERENT authorization server from the partner API's own OAuth endpoints and its scopes are deliberately NOT listed as partner-API scopes here. See well-known/altoira-well-known.yml.
overview: 'AltoIRA uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://altoira.sandbox.altoira.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AltoIRA
provider_slug: altoira
schemes:
- description: Redirect your users to /oauth/authorize to get started (see the OAuth section on this documentation)
  flows:
  - authorizationUrl: https://altoira.sandbox.altoira.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://altoira.sandbox.altoira.com/oauth/token
  name: UserOauth
  source: openapi/altoira-partner-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: altoira-scopes
source_filename: altoira-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: derived\nsource: openapi/altoira-partner-api-openapi.yml\nschemes:\n- name: UserOauth\n  source: openapi/altoira-partner-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://altoira.sandbox.altoira.com/oauth/authorize\n    tokenUrl: https://altoira.sandbox.altoira.com/oauth/token\n  description: Redirect your users to /oauth/authorize to get started (see the OAuth section on this\n    documentation)\nscopes: []\ndocs: null\nnote: 'The partner API''s oauth2 authorizationCode flow declares an EMPTY scopes map, and Alto''s\n  developer hub documents no scope reference page. The /oauth/authorize operation accepts a `scope`\n  query parameter but no permitted values are published, so an integrator cannot determine what to\n  send. This is a provider-fixable documentation gap.\n\n  Separately, Alto runs an Auth0 tenant at auth.altoira.com for the investor/issuer web application\n  which DOES publish scopes_supported\
  \ (openid, profile, offline_access, name, given_name, family_name,\n  nickname, email, email_verified, picture, created_at, identities, phone, address). That is a DIFFERENT\n  authorization server from the partner API''s own OAuth endpoints and its scopes are deliberately\n  NOT listed as partner-API scopes here. See well-known/altoira-well-known.yml.'\nseparate_authorization_server:\n  issuer: https://auth.altoira.com/\n  provider: Auth0\n  role: investor + issuer web application login (app.altoira.com)\n  discovery: well-known/altoira-openid-configuration.json\n  scopes_supported:\n  - openid\n  - profile\n  - offline_access\n  - name\n  - given_name\n  - family_name\n  - nickname\n  - email\n  - email_verified\n  - picture\n  - created_at\n  - identities\n  - phone\n  - address\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/altoira/refs/heads/main/scopes/altoira-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Financial Services
- Retirement
- Self-Directed IRA
- Alternative Investments
- Private Markets
- Fintech
- Custody
- Cryptocurrency
- Wealth Management
- Investing
- Capital Raising
token_urls:
- https://altoira.sandbox.altoira.com/oauth/token
---
