---
api_specs:
- filename: fluotest-com-mcp-api-openapi.yml
  format: yaml
  label: FluoTest MCP API
  slug: fluotest-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluotest-com/openapi/fluotest-com-mcp-api-openapi.yml
- filename: fluotest-com-status-api-openapi.yml
  format: yaml
  label: FluoTest Status API
  slug: fluotest-com-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluotest-com/openapi/fluotest-com-status-api-openapi.yml
authorization_urls:
- https://abvrtonacdgcxpkkrpie.supabase.co/auth/v1/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: FluoTest Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'FluoTest publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the FluoTest API on a user''s behalf.


  Tokens are issued from https://abvrtonacdgcxpkkrpie.supabase.co/auth/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: FluoTest
provider_slug: fluotest-com
schemes:
- description: 'Supabase OAuth 2.1 server: sign in and approve on a consent screen, no keys to copy.'
  flows:
  - authorizationUrl: https://abvrtonacdgcxpkkrpie.supabase.co/auth/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://abvrtonacdgcxpkkrpie.supabase.co/auth/v1/oauth/token
  name: oauth2
  source: openapi/fluotest-com-openapi.json
scope_count: 3
scope_names:
- email
- openid
- profile
scopes:
- description: Email address
  flows:
  - authorizationCode
  scope: email
- description: OpenID Connect
  flows:
  - authorizationCode
  scope: openid
- description: Profile info
  flows:
  - authorizationCode
  scope: profile
slug: fluotest-com-scopes
source_filename: fluotest-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/fluotest-com-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/fluotest-com-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://abvrtonacdgcxpkkrpie.supabase.co/auth/v1/oauth/authorize\n    tokenUrl: https://abvrtonacdgcxpkkrpie.supabase.co/auth/v1/oauth/token\n  description: 'Supabase OAuth 2.1 server: sign in and approve on a consent screen, no keys\n    to copy.'\nscopes:\n- scope: email\n  description: Email address\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fluotest-com-openapi.json\n- scope: openid\n  description: OpenID Connect\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fluotest-com-openapi.json\n- scope: profile\n  description: Profile info\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fluotest-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/fluotest-com/scopes/fluotest-com-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- Quiz
- No-Code
- Education
- Marketing
token_bound: false
token_urls:
- https://abvrtonacdgcxpkkrpie.supabase.co/auth/v1/oauth/token
---
