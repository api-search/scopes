---
authorization_urls:
- https://org-account.snowflakecomputing.com/oauth/authorize
- /oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Snowflake Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Snowflake publishes 1 OAuth 2.0 scope via the authorizationCode and implicit flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Snowflake API on a user''s behalf.


  Tokens are issued from https://org-account.snowflakecomputing.com/oauth/token-request.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Snowflake
provider_slug: snowflake
schemes:
- description: Snowflake OAuth authentication flow.
  flows:
  - authorizationUrl: https://org-account.snowflakecomputing.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://org-account.snowflakecomputing.com/oauth/token-request
  name: snowflakeOAuth
  source: openapi/snowflake-sql-rest-api.yaml
- flows:
  - authorizationUrl: /oauth/authorize
    flow: implicit
  name: snowflakeOAuth
  source: openapi/sqlapi.yaml
scope_count: 1
scope_names:
- session:role:PUBLIC
scopes:
- description: Default public role access
  flows:
  - authorizationCode
  scope: session:role:PUBLIC
slug: snowflake-scopes
source_filename: snowflake-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/snowflake-sql-rest-api.yaml, openapi/sqlapi.yaml\nschemes:\n- name: snowflakeOAuth\n  source: openapi/snowflake-sql-rest-api.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://org-account.snowflakecomputing.com/oauth/authorize\n    tokenUrl: https://org-account.snowflakecomputing.com/oauth/token-request\n  description: Snowflake OAuth authentication flow.\n- name: snowflakeOAuth\n  source: openapi/sqlapi.yaml\n  flows:\n  - flow: implicit\n    authorizationUrl: /oauth/authorize\nscopes:\n- scope: session:role:PUBLIC\n  description: Default public role access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/snowflake-sql-rest-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/scopes/snowflake-scopes.yml
summary_line: 1 scope · authorizationCode/implicit
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
token_urls:
- https://org-account.snowflakecomputing.com/oauth/token-request
---
