---
api_specs:
- filename: treasure-data-bulk-loads-api-openapi.yml
  format: yaml
  label: Treasure Data Bulk Loads API
  slug: treasure-data-bulk-loads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/openapi/treasure-data-bulk-loads-api-openapi.yml
- filename: treasure-data-system-api-openapi.yml
  format: yaml
  label: Treasure Data System API
  slug: treasure-data-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/openapi/treasure-data-system-api-openapi.yml
- filename: treasure-data-postback-api-openapi.yml
  format: yaml
  label: Treasure Data Postback API
  slug: treasure-data-postback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/openapi/treasure-data-postback-api-openapi.yml
- filename: treasure-data-bulk-import-api-openapi.yml
  format: yaml
  label: Treasure Data Bulk Import API
  slug: treasure-data-bulk-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/openapi/treasure-data-bulk-import-api-openapi.yml
- filename: treasure-data-bulk-loads-api-openapi.yml
  format: yaml
  label: Treasure Data Bulk Loads API
  slug: treasure-data-bulk-loads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/openapi/treasure-data-bulk-loads-api-openapi.yml
- filename: treasure-data-connectors-api-openapi.yml
  format: yaml
  label: Treasure Data Connectors API
  slug: treasure-data-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/openapi/treasure-data-connectors-api-openapi.yml
- filename: treasure-data-databases-api-openapi.yml
  format: yaml
  label: Treasure Data Databases API
  slug: treasure-data-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/openapi/treasure-data-databases-api-openapi.yml
- filename: treasure-data-jobs-api-openapi.yml
  format: yaml
  label: Treasure Data Jobs API
  slug: treasure-data-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/openapi/treasure-data-jobs-api-openapi.yml
- filename: treasure-data-sso-api-openapi.yml
  format: yaml
  label: Treasure Data SSO API
  slug: treasure-data-sso-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/openapi/treasure-data-sso-api-openapi.yml
- filename: treasure-data-system-api-openapi.yml
  format: yaml
  label: Treasure Data System API
  slug: treasure-data-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/openapi/treasure-data-system-api-openapi.yml
- filename: treasure-data-tables-api-openapi.yml
  format: yaml
  label: Treasure Data Tables API
  slug: treasure-data-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/openapi/treasure-data-tables-api-openapi.yml
- filename: treasure-data-users-api-openapi.yml
  format: yaml
  label: Treasure Data Users API
  slug: treasure-data-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/openapi/treasure-data-users-api-openapi.yml
- filename: treasure-data-td-api-v3-openapi.yml
  format: yaml
  label: Treasure Data API v3
  slug: treasure-data-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/openapi/treasure-data-td-api-v3-openapi.yml
- filename: treasure-data-cdp-api-openapi.yml
  format: yaml
  label: Treasure Data CDP API
  slug: treasure-data-cdp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/openapi/treasure-data-cdp-api-openapi.yml
- filename: treasure-data-llm-api-openapi.yml
  format: yaml
  label: Treasure Data LLM API
  slug: treasure-data-llm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/openapi/treasure-data-llm-api-openapi.yml
- filename: treasure-data-workflow-api-openapi.yml
  format: yaml
  label: Treasure Workflow API
  slug: treasure-data-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/openapi/treasure-data-workflow-api-openapi.yml
- filename: treasure-data-dwh-integration-api-openapi.yml
  format: yaml
  label: Treasure Data Data Warehouse Integration API
  slug: treasure-data-dwh-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/openapi/treasure-data-dwh-integration-api-openapi.yml
- filename: treasure-data-personalization-api-openapi.yml
  format: yaml
  label: Treasure Data Personalization Service
  slug: treasure-data-personalization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/openapi/treasure-data-personalization-api-openapi.yml
- filename: treasure-data-postback-api-openapi.yml
  format: yaml
  label: Treasure Data Postback API
  slug: treasure-data-postback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/openapi/treasure-data-postback-api-openapi.yml
- filename: treasure-data-postback-api-v2-openapi.yml
  format: yaml
  label: Treasure Data Postback API v2
  slug: treasure-data-postback-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/openapi/treasure-data-postback-api-v2-openapi.yml
authorization_urls:
- https://console.us01.treasuredata.com/oauth/authorize
description: OAuth 2.0 / OpenID Connect scopes advertised by Treasure Data's authorization server. Read from the provider's own discovery document rather than from an OpenAPI securityScheme — none of the eight published Treasure AI OpenAPI descriptions declares an oauth2 flow, so the discovery document is the only machine-readable source for the scope set.
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Treasure Data Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Treasure Data publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Treasure Data API on a user''s behalf.


  Tokens are issued from https://console.us01.treasuredata.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Treasure Data
provider_slug: treasure-data
schemes:
- flows:
  - authorizationUrl: https://console.us01.treasuredata.com/oauth/authorize
    flow: authorizationCode
    pkce:
    - S256
    - plain
    refreshUrl: https://console.us01.treasuredata.com/oauth/token
    tokenUrl: https://console.us01.treasuredata.com/oauth/token
  name: TreasureDataOAuth
  source: well-known/treasure-data-openid-configuration.json
  type: openIdConnect
scope_count: 4
scope_names:
- public
- openid
- email
- profile
scopes:
- description: Treasure Data's own application scope. Advertised alongside the three standard OIDC scopes; the authorization server does not publish a description for it and no docs page documents it further.
  flows:
  - authorizationCode
  scope: public
- description: Request an ID token — standard OpenID Connect Core scope.
  flows:
  - authorizationCode
  scope: openid
- description: Release the email and email_verified claims.
  flows:
  - authorizationCode
  scope: email
- description: Release the standard profile claims.
  flows:
  - authorizationCode
  scope: profile
slug: treasure-data-scopes
source_filename: treasure-data-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "name: Treasure Data OAuth Scopes\ndescription: >-\n  OAuth 2.0 / OpenID Connect scopes advertised by Treasure Data's authorization server. Read from the\n  provider's own discovery document rather than from an OpenAPI securityScheme — none of the eight\n  published Treasure AI OpenAPI descriptions declares an oauth2 flow, so the discovery document is the\n  only machine-readable source for the scope set.\nspecificationVersion: '0.1'\ngenerated: '2026-08-13'\nmethod: probed\nsource: https://api.treasuredata.com/.well-known/openid-configuration\nfile: well-known/treasure-data-openid-configuration.json\nissuer: https://console.us01.treasuredata.com\nschemes:\n  - name: TreasureDataOAuth\n    type: openIdConnect\n    source: well-known/treasure-data-openid-configuration.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://console.us01.treasuredata.com/oauth/authorize\n        tokenUrl: https://console.us01.treasuredata.com/oauth/token\n        refreshUrl:\
  \ https://console.us01.treasuredata.com/oauth/token\n        pkce: [S256, plain]\nscopes:\n  - scope: public\n    description: >-\n      Treasure Data's own application scope. Advertised alongside the three standard OIDC scopes; the\n      authorization server does not publish a description for it and no docs page documents it further.\n    flows: [authorizationCode]\n    sources: [well-known/treasure-data-openid-configuration.json]\n    standard: false\n  - scope: openid\n    description: Request an ID token — standard OpenID Connect Core scope.\n    flows: [authorizationCode]\n    sources: [well-known/treasure-data-openid-configuration.json]\n    standard: true\n  - scope: email\n    description: Release the email and email_verified claims.\n    flows: [authorizationCode]\n    sources: [well-known/treasure-data-openid-configuration.json]\n    standard: true\n  - scope: profile\n    description: Release the standard profile claims.\n    flows: [authorizationCode]\n    sources: [well-known/treasure-data-openid-configuration.json]\n\
  \    standard: true\nscope_count: 4\nclaims:\n  - iss\n  - sub\n  - aud\n  - exp\n  - iat\n  - email\n  - email_verified\n  - td_account_id\n  - administrator\nnotes:\n  - >-\n    Only one non-standard scope (`public`) exists. There is no read/write or per-resource scope model —\n    an access token issued by this server is coarse-grained, and fine-grained authorization is handled\n    separately by the Access Control policy/permission system in the TD API\n    (/access_control/policies, /access_control/permissions).\n  - >-\n    No public scopes reference page was found in the documentation; the discovery document is the\n    authoritative published list. Absence of a docs page is recorded, not guessed around.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/scopes/treasure-data-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Customer Data Platform
- CDP
- Big Data
- Data Warehouse
- Hive
- Presto
- Enterprise
- AI
- Marketing
- Analytics
token_urls:
- https://console.us01.treasuredata.com/oauth/token
---
