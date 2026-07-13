---
api_specs:
- filename: bloomerang-openapi.yml
  format: yaml
  label: Bloomerang Constituents API
  slug: bloomerang-constituents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomerang/refs/heads/main/openapi/bloomerang-openapi.yml
- filename: bloomerang-openapi.yml
  format: yaml
  label: Bloomerang Households API
  slug: bloomerang-households-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomerang/refs/heads/main/openapi/bloomerang-openapi.yml
- filename: bloomerang-openapi.yml
  format: yaml
  label: Bloomerang Transactions API
  slug: bloomerang-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomerang/refs/heads/main/openapi/bloomerang-openapi.yml
- filename: bloomerang-openapi.yml
  format: yaml
  label: Bloomerang Interactions API
  slug: bloomerang-interactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomerang/refs/heads/main/openapi/bloomerang-openapi.yml
- filename: bloomerang-openapi.yml
  format: yaml
  label: Bloomerang Notes API
  slug: bloomerang-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomerang/refs/heads/main/openapi/bloomerang-openapi.yml
- filename: bloomerang-openapi.yml
  format: yaml
  label: Bloomerang Relationships API
  slug: bloomerang-relationships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomerang/refs/heads/main/openapi/bloomerang-openapi.yml
- filename: bloomerang-openapi.yml
  format: yaml
  label: Bloomerang Custom Fields API
  slug: bloomerang-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomerang/refs/heads/main/openapi/bloomerang-openapi.yml
- filename: bloomerang-openapi.yml
  format: yaml
  label: Bloomerang Lists API
  slug: bloomerang-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomerang/refs/heads/main/openapi/bloomerang-openapi.yml
- filename: bloomerang-openapi.yml
  format: yaml
  label: Bloomerang Webhooks API
  slug: bloomerang-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomerang/refs/heads/main/openapi/bloomerang-openapi.yml
- filename: bloomerang-openapi.yml
  format: yaml
  label: Bloomerang Accounts and Users API
  slug: bloomerang-accounts-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomerang/refs/heads/main/openapi/bloomerang-openapi.yml
authorization_urls:
- https://crm.bloomerang.co/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Bloomerang Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Bloomerang publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Bloomerang API on a user''s behalf.


  Tokens are issued from https://api.bloomerang.co/v2/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bloomerang
provider_slug: bloomerang
schemes:
- description: 'OAuth 2.0 access token for third-party applications, presented as `Authorization: Bearer {access_token}`.'
  flows:
  - authorizationUrl: https://crm.bloomerang.co/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.bloomerang.co/v2/oauth/token
  name: oauth2Bearer
  source: openapi/bloomerang-openapi.yml
scope_count: 1
scope_names:
- api
scopes:
- description: Full read/write access to account data.
  flows:
  - authorizationCode
  scope: api
slug: bloomerang-scopes
source_filename: bloomerang-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bloomerang-openapi.yml\nschemes:\n- name: oauth2Bearer\n  source: openapi/bloomerang-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://crm.bloomerang.co/oauth/authorize\n    tokenUrl: https://api.bloomerang.co/v2/oauth/token\n  description: 'OAuth 2.0 access token for third-party applications, presented as `Authorization:\n    Bearer {access_token}`.'\nscopes:\n- scope: api\n  description: Full read/write access to account data.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bloomerang-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomerang/refs/heads/main/scopes/bloomerang-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Nonprofit
- Donor Management
- CRM
- Fundraising
- Fundraising Software
token_urls:
- https://api.bloomerang.co/v2/oauth/token
---
