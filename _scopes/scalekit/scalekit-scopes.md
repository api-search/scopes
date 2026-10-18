---
api_specs:
- filename: scalekit-admin-portal-api-openapi.yml
  format: yaml
  label: Scalekit Admin Portal API
  slug: scalekit-admin-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalekit/refs/heads/main/openapi/scalekit-admin-portal-api-openapi.yml
- filename: scalekit-authentication-api-openapi.yml
  format: yaml
  label: Scalekit Authentication API
  slug: scalekit-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalekit/refs/heads/main/openapi/scalekit-authentication-api-openapi.yml
- filename: scalekit-connected-accounts-api-openapi.yml
  format: yaml
  label: Scalekit Connected Accounts API
  slug: scalekit-connected-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalekit/refs/heads/main/openapi/scalekit-connected-accounts-api-openapi.yml
- filename: scalekit-connections-api-openapi.yml
  format: yaml
  label: Scalekit Connections API
  slug: scalekit-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalekit/refs/heads/main/openapi/scalekit-connections-api-openapi.yml
- filename: scalekit-directories-api-openapi.yml
  format: yaml
  label: Scalekit Directories API
  slug: scalekit-directories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalekit/refs/heads/main/openapi/scalekit-directories-api-openapi.yml
- filename: scalekit-organization-settings-api-openapi.yml
  format: yaml
  label: Scalekit Organization Settings API
  slug: scalekit-organization-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalekit/refs/heads/main/openapi/scalekit-organization-settings-api-openapi.yml
- filename: scalekit-organizations-api-openapi.yml
  format: yaml
  label: Scalekit Organizations API
  slug: scalekit-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalekit/refs/heads/main/openapi/scalekit-organizations-api-openapi.yml
- filename: scalekit-roles-api-openapi.yml
  format: yaml
  label: Scalekit Roles API
  slug: scalekit-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalekit/refs/heads/main/openapi/scalekit-roles-api-openapi.yml
- filename: scalekit-users-memberships-api-openapi.yml
  format: yaml
  label: Scalekit Users & Memberships API
  slug: scalekit-users-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalekit/refs/heads/main/openapi/scalekit-users-memberships-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Scalekit Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Scalekit uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://{environment}.scalekit.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Scalekit
provider_slug: scalekit
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://{environment}.scalekit.com/oauth/token
  name: oauth2ClientCredentials
  source: openapi/scalekit-admin-portal-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://{environment}.scalekit.com/oauth/token
  name: oauth2ClientCredentials
  source: openapi/scalekit-authentication-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://{environment}.scalekit.com/oauth/token
  name: oauth2ClientCredentials
  source: openapi/scalekit-connected-accounts-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://{environment}.scalekit.com/oauth/token
  name: oauth2ClientCredentials
  source: openapi/scalekit-connections-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://{environment}.scalekit.com/oauth/token
  name: oauth2ClientCredentials
  source: openapi/scalekit-directories-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://{environment}.scalekit.com/oauth/token
  name: oauth2ClientCredentials
  source: openapi/scalekit-organization-settings-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://{environment}.scalekit.com/oauth/token
  name: oauth2ClientCredentials
  source: openapi/scalekit-organizations-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://{environment}.scalekit.com/oauth/token
  name: oauth2ClientCredentials
  source: openapi/scalekit-roles-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://{environment}.scalekit.com/oauth/token
  name: oauth2ClientCredentials
  source: openapi/scalekit-users-memberships-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: scalekit-scopes
source_filename: scalekit-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/scalekit-admin-portal-api-openapi.yml, openapi/scalekit-authentication-api-openapi.yml,\n  openapi/scalekit-connected-accounts-api-openapi.yml, openapi/scalekit-connections-api-openapi.yml,\n  openapi/scalekit-directories-api-openapi.yml, openapi/scalekit-organization-settings-api-openapi.yml,\n  openapi/scalekit-organizations-api-openapi.yml, openapi/scalekit-roles-api-openapi.yml, openapi/scalekit-users-memberships-api-openapi.yml\nschemes:\n- name: oauth2ClientCredentials\n  source: openapi/scalekit-admin-portal-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{environment}.scalekit.com/oauth/token\n- name: oauth2ClientCredentials\n  source: openapi/scalekit-authentication-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{environment}.scalekit.com/oauth/token\n- name: oauth2ClientCredentials\n  source: openapi/scalekit-connected-accounts-api-openapi.yml\n  flows:\n\
  \  - flow: clientCredentials\n    tokenUrl: https://{environment}.scalekit.com/oauth/token\n- name: oauth2ClientCredentials\n  source: openapi/scalekit-connections-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{environment}.scalekit.com/oauth/token\n- name: oauth2ClientCredentials\n  source: openapi/scalekit-directories-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{environment}.scalekit.com/oauth/token\n- name: oauth2ClientCredentials\n  source: openapi/scalekit-organization-settings-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{environment}.scalekit.com/oauth/token\n- name: oauth2ClientCredentials\n  source: openapi/scalekit-organizations-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{environment}.scalekit.com/oauth/token\n- name: oauth2ClientCredentials\n  source: openapi/scalekit-roles-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl:\
  \ https://{environment}.scalekit.com/oauth/token\n- name: oauth2ClientCredentials\n  source: openapi/scalekit-users-memberships-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{environment}.scalekit.com/oauth/token\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scalekit/refs/heads/main/scopes/scalekit-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Authentication
- SSO
- SCIM
- Identity
- B2B SaaS
- Agent Auth
- Identity Federation
token_bound: false
token_urls:
- https://{environment}.scalekit.com/oauth/token
---
