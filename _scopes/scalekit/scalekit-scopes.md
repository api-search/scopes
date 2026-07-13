---
api_specs:
- filename: scalekit-openapi.yml
  format: yaml
  label: Scalekit SSO Connections API
  slug: scalekit-sso-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalekit/refs/heads/main/openapi/scalekit-openapi.yml
- filename: scalekit-openapi.yml
  format: yaml
  label: Scalekit Organizations API
  slug: scalekit-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalekit/refs/heads/main/openapi/scalekit-openapi.yml
- filename: scalekit-openapi.yml
  format: yaml
  label: Scalekit Directory / SCIM API
  slug: scalekit-directory-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalekit/refs/heads/main/openapi/scalekit-openapi.yml
- filename: scalekit-openapi.yml
  format: yaml
  label: Scalekit Users & Memberships API
  slug: scalekit-users-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalekit/refs/heads/main/openapi/scalekit-openapi.yml
- filename: scalekit-openapi.yml
  format: yaml
  label: Scalekit Agent / M2M Auth API
  slug: scalekit-agent-m2m-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalekit/refs/heads/main/openapi/scalekit-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.scalekit.com/apis/
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Scalekit Scopes
name_suffix: OAuth Scopes
note: Scalekit's own API is secured with OAuth 2.0 client credentials and publishes no scopes for its endpoints; the scopes documented at https://docs.scalekit.com/guides/m2m/scopes/ are customer-defined permissions for their own API clients, not Scalekit API scopes (https://docs.scalekit.com/apis/).
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
  source: openapi/scalekit-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: scalekit-scopes
source_filename: scalekit-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/scalekit-openapi.yml\ndocs: https://docs.scalekit.com/apis/\nnote: Scalekit's own API is secured with OAuth 2.0 client credentials and publishes\n  no scopes for its endpoints; the scopes documented at\n  https://docs.scalekit.com/guides/m2m/scopes/ are customer-defined permissions\n  for their own API clients, not Scalekit API scopes\n  (https://docs.scalekit.com/apis/).\nschemes:\n- name: oauth2ClientCredentials\n  source: openapi/scalekit-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{environment}.scalekit.com/oauth/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scalekit/refs/heads/main/scopes/scalekit-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Authentication
- SSO
- SCIM
- Identity
- B2B SaaS
- Agent Auth
token_urls:
- https://{environment}.scalekit.com/oauth/token
---
