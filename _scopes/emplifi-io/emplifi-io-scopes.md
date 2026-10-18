---
api_specs:
- filename: emplifi-io-ads-api-openapi.yml
  format: yaml
  label: Emplifi Ads API
  slug: emplifi-io-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emplifi-io/refs/heads/main/openapi/emplifi-io-ads-api-openapi.yml
- filename: emplifi-io-assets-api-openapi.yml
  format: yaml
  label: Emplifi Assets API
  slug: emplifi-io-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emplifi-io/refs/heads/main/openapi/emplifi-io-assets-api-openapi.yml
- filename: emplifi-io-care-api-openapi.yml
  format: yaml
  label: Emplifi Care API
  slug: emplifi-io-care-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emplifi-io/refs/heads/main/openapi/emplifi-io-care-api-openapi.yml
- filename: emplifi-io-community-api-openapi.yml
  format: yaml
  label: Emplifi Community API
  slug: emplifi-io-community-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emplifi-io/refs/heads/main/openapi/emplifi-io-community-api-openapi.yml
- filename: emplifi-io-listening-api-openapi.yml
  format: yaml
  label: Emplifi Listening API
  slug: emplifi-io-listening-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emplifi-io/refs/heads/main/openapi/emplifi-io-listening-api-openapi.yml
- filename: emplifi-io-posts-api-openapi.yml
  format: yaml
  label: Emplifi Posts API
  slug: emplifi-io-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emplifi-io/refs/heads/main/openapi/emplifi-io-posts-api-openapi.yml
- filename: emplifi-io-profile-metrics-api-openapi.yml
  format: yaml
  label: Emplifi Profile Metrics API
  slug: emplifi-io-profile-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emplifi-io/refs/heads/main/openapi/emplifi-io-profile-metrics-api-openapi.yml
- filename: emplifi-io-reference-api-openapi.yml
  format: yaml
  label: Emplifi Reference API
  slug: emplifi-io-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emplifi-io/refs/heads/main/openapi/emplifi-io-reference-api-openapi.yml
authorization_urls:
- https://api.emplifi.io/oauth2/0/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: none
name: Emplifi Io Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Emplifi uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.emplifi.io/oauth2/0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Emplifi
provider_slug: emplifi-io
schemes:
- description: OAuth 2.0 authorization code flow. Create a Custom integration in Emplifi Settings to obtain client credentials.
  flows:
  - authorizationUrl: https://api.emplifi.io/oauth2/0/auth
    flow: authorizationCode
    tokenUrl: https://api.emplifi.io/oauth2/0/token
  name: oauth2
  source: openapi/emplifi-io-ads-api-openapi.yml
- description: OAuth 2.0 authorization code flow. Create a Custom integration in Emplifi Settings to obtain client credentials.
  flows:
  - authorizationUrl: https://api.emplifi.io/oauth2/0/auth
    flow: authorizationCode
    tokenUrl: https://api.emplifi.io/oauth2/0/token
  name: oauth2
  source: openapi/emplifi-io-assets-api-openapi.yml
- description: OAuth 2.0 authorization code flow. Create a Custom integration in Emplifi Settings to obtain client credentials.
  flows:
  - authorizationUrl: https://api.emplifi.io/oauth2/0/auth
    flow: authorizationCode
    tokenUrl: https://api.emplifi.io/oauth2/0/token
  name: oauth2
  source: openapi/emplifi-io-care-api-openapi.yml
- description: OAuth 2.0 authorization code flow. Create a Custom integration in Emplifi Settings to obtain client credentials.
  flows:
  - authorizationUrl: https://api.emplifi.io/oauth2/0/auth
    flow: authorizationCode
    tokenUrl: https://api.emplifi.io/oauth2/0/token
  name: oauth2
  source: openapi/emplifi-io-community-api-openapi.yml
- description: OAuth 2.0 authorization code flow. Create a Custom integration in Emplifi Settings to obtain client credentials.
  flows:
  - authorizationUrl: https://api.emplifi.io/oauth2/0/auth
    flow: authorizationCode
    tokenUrl: https://api.emplifi.io/oauth2/0/token
  name: oauth2
  source: openapi/emplifi-io-listening-api-openapi.yml
- description: OAuth 2.0 authorization code flow. Create a Custom integration in Emplifi Settings to obtain client credentials.
  flows:
  - authorizationUrl: https://api.emplifi.io/oauth2/0/auth
    flow: authorizationCode
    tokenUrl: https://api.emplifi.io/oauth2/0/token
  name: oauth2
  source: openapi/emplifi-io-posts-api-openapi.yml
- description: OAuth 2.0 authorization code flow. Create a Custom integration in Emplifi Settings to obtain client credentials.
  flows:
  - authorizationUrl: https://api.emplifi.io/oauth2/0/auth
    flow: authorizationCode
    tokenUrl: https://api.emplifi.io/oauth2/0/token
  name: oauth2
  source: openapi/emplifi-io-profile-metrics-api-openapi.yml
- description: OAuth 2.0 authorization code flow. Create a Custom integration in Emplifi Settings to obtain client credentials.
  flows:
  - authorizationUrl: https://api.emplifi.io/oauth2/0/auth
    flow: authorizationCode
    tokenUrl: https://api.emplifi.io/oauth2/0/token
  name: oauth2
  source: openapi/emplifi-io-reference-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: emplifi-io-scopes
source_filename: emplifi-io-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/emplifi-io-ads-api-openapi.yml, openapi/emplifi-io-assets-api-openapi.yml, openapi/emplifi-io-care-api-openapi.yml,\n  openapi/emplifi-io-community-api-openapi.yml, openapi/emplifi-io-listening-api-openapi.yml,\n  openapi/emplifi-io-posts-api-openapi.yml, openapi/emplifi-io-profile-metrics-api-openapi.yml,\n  openapi/emplifi-io-reference-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/emplifi-io-ads-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.emplifi.io/oauth2/0/auth\n    tokenUrl: https://api.emplifi.io/oauth2/0/token\n  description: OAuth 2.0 authorization code flow. Create a Custom integration in Emplifi Settings\n    to obtain client credentials.\n- name: oauth2\n  source: openapi/emplifi-io-assets-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.emplifi.io/oauth2/0/auth\n    tokenUrl: https://api.emplifi.io/oauth2/0/token\n\
  \  description: OAuth 2.0 authorization code flow. Create a Custom integration in Emplifi Settings\n    to obtain client credentials.\n- name: oauth2\n  source: openapi/emplifi-io-care-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.emplifi.io/oauth2/0/auth\n    tokenUrl: https://api.emplifi.io/oauth2/0/token\n  description: OAuth 2.0 authorization code flow. Create a Custom integration in Emplifi Settings\n    to obtain client credentials.\n- name: oauth2\n  source: openapi/emplifi-io-community-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.emplifi.io/oauth2/0/auth\n    tokenUrl: https://api.emplifi.io/oauth2/0/token\n  description: OAuth 2.0 authorization code flow. Create a Custom integration in Emplifi Settings\n    to obtain client credentials.\n- name: oauth2\n  source: openapi/emplifi-io-listening-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.emplifi.io/oauth2/0/auth\n\
  \    tokenUrl: https://api.emplifi.io/oauth2/0/token\n  description: OAuth 2.0 authorization code flow. Create a Custom integration in Emplifi Settings\n    to obtain client credentials.\n- name: oauth2\n  source: openapi/emplifi-io-posts-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.emplifi.io/oauth2/0/auth\n    tokenUrl: https://api.emplifi.io/oauth2/0/token\n  description: OAuth 2.0 authorization code flow. Create a Custom integration in Emplifi Settings\n    to obtain client credentials.\n- name: oauth2\n  source: openapi/emplifi-io-profile-metrics-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.emplifi.io/oauth2/0/auth\n    tokenUrl: https://api.emplifi.io/oauth2/0/token\n  description: OAuth 2.0 authorization code flow. Create a Custom integration in Emplifi Settings\n    to obtain client credentials.\n- name: oauth2\n  source: openapi/emplifi-io-reference-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n\
  \    authorizationUrl: https://api.emplifi.io/oauth2/0/auth\n    tokenUrl: https://api.emplifi.io/oauth2/0/token\n  description: OAuth 2.0 authorization code flow. Create a Custom integration in Emplifi Settings\n    to obtain client credentials.\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emplifi-io/refs/heads/main/scopes/emplifi-io-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Marketing
- Social Media
- Analytics
- Social Media Analytics
- Social Listening
- Marketing Analytics
- Digital Asset Management
- Customer Care
- Emplifi
token_bound: false
token_urls:
- https://api.emplifi.io/oauth2/0/token
---
