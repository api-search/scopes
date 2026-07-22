---
authorization_urls:
- https://api.supermetrics.com/oauth/authorize
description: ''
docs: https://supermetrics.com/docs/product-api-oauth/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Supermetrics Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Supermetrics publishes 13 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Supermetrics API on a user''s behalf.


  Tokens are issued from https://api.supermetrics.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Supermetrics
provider_slug: supermetrics
schemes:
- flows:
  - authorizationUrl: https://api.supermetrics.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.supermetrics.com/oauth/token
  name: OAuth2
  source: well-known/supermetrics-openid-configuration.json
scope_count: 13
scope_names:
- openid
- profile
- email
- offline_access
- team_read
- user_read
- ds_logins_read
- ds_accounts_read
- ds_queries_run
- ds_platform_write
- ds_login_links_read
- ds_login_links_write
- auth_create_account
scopes:
- description: OpenID Connect authentication (issue an ID token)
  flows:
  - authorizationCode
  scope: openid
- description: Access to the user's basic profile claims (name
  flows:
  - authorizationCode
  scope: profile
- description: Access to the user's email claim
  flows:
  - authorizationCode
  scope: email
- description: Issue a refresh token for long-lived offline access
  flows:
  - authorizationCode
  scope: offline_access
- description: Read team settings and membership
  flows:
  - authorizationCode
  scope: team_read
- description: Read the authenticated user
  flows:
  - authorizationCode
  scope: user_read
- description: Read data source logins (authentications)
  flows:
  - authorizationCode
  scope: ds_logins_read
- description: Read the accounts available under a data source
  flows:
  - authorizationCode
  scope: ds_accounts_read
- description: Run data queries against connected data sources
  flows:
  - authorizationCode
  scope: ds_queries_run
- description: Write access to data source / platform configuration
  flows:
  - authorizationCode
  scope: ds_platform_write
- description: Read single-use data source login links
  flows:
  - authorizationCode
  scope: ds_login_links_read
- description: Create single-use data source login links
  flows:
  - authorizationCode
  scope: ds_login_links_write
- description: Create a Supermetrics account during the auth flow
  flows:
  - authorizationCode
  scope: auth_create_account
slug: supermetrics-scopes
source_filename: supermetrics-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://api.supermetrics.com/.well-known/openid-configuration\ndocs: https://supermetrics.com/docs/product-api-oauth/\nschemes:\n- name: OAuth2\n  source: well-known/supermetrics-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.supermetrics.com/oauth/authorize\n    tokenUrl: https://api.supermetrics.com/oauth/token\nscopes:\n- {scope: openid, description: OpenID Connect authentication (issue an ID token), flows: [authorizationCode]}\n- {scope: profile, description: Access to the user's basic profile claims (name, given_name, family_name), flows: [authorizationCode]}\n- {scope: email, description: Access to the user's email claim, flows: [authorizationCode]}\n- {scope: offline_access, description: Issue a refresh token for long-lived offline access, flows: [authorizationCode]}\n- {scope: team_read, description: Read team settings and membership, flows: [authorizationCode]}\n\
  - {scope: user_read, description: Read the authenticated user, flows: [authorizationCode]}\n- {scope: ds_logins_read, description: Read data source logins (authentications), flows: [authorizationCode]}\n- {scope: ds_accounts_read, description: Read the accounts available under a data source, flows: [authorizationCode]}\n- {scope: ds_queries_run, description: Run data queries against connected data sources, flows: [authorizationCode]}\n- {scope: ds_platform_write, description: Write access to data source / platform configuration, flows: [authorizationCode]}\n- {scope: ds_login_links_read, description: Read single-use data source login links, flows: [authorizationCode]}\n- {scope: ds_login_links_write, description: Create single-use data source login links, flows: [authorizationCode]}\n- {scope: auth_create_account, description: Create a Supermetrics account during the auth flow, flows: [authorizationCode]}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/supermetrics/refs/heads/main/scopes/supermetrics-scopes.yml
summary_line: 13 scopes · authorizationCode
tags:
- Company
- Marketing
- Analytics
- Advertising
- Data
- Reporting
- Business Intelligence
- Data Warehouse
token_urls:
- https://api.supermetrics.com/oauth/token
---
