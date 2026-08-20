---
api_specs:
- filename: vim-rest-api-openapi-original.json
  format: json
  label: Vim Applications & Organizations API
  slug: vim-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vim/refs/heads/main/openapi/vim-rest-api-openapi-original.json
- filename: vim-rest-api-openapi-original.json
  format: json
  label: Vim Invitations API
  slug: vim-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vim/refs/heads/main/openapi/vim-rest-api-openapi-original.json
- filename: vim-rest-api-openapi-original.json
  format: json
  label: Vim Appointments API
  slug: vim-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vim/refs/heads/main/openapi/vim-rest-api-openapi-original.json
- filename: vim-rest-api-openapi-original.json
  format: json
  label: Vim Chart Retrieval API
  slug: vim-chart-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vim/refs/heads/main/openapi/vim-rest-api-openapi-original.json
- filename: vim-data-source-openapi-original.json
  format: json
  label: Vim Data Source
  slug: vim-data-source
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vim/refs/heads/main/openapi/vim-data-source-openapi-original.json
authorization_urls: []
description: ''
docs: https://auth.getvim.com/.well-known/openid-configuration
flows:
- implicit
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Vim Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Vim publishes 4 OAuth 2.0 scopes via the implicit and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Vim API on a user''s behalf.


  Tokens are issued from https://auth.getvim.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Vim
provider_slug: vim
schemes:
- flows:
  - flow: implicit
  name: service
  source: openapi/vim-data-source-openapi-original.json
  type: oauth2
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.getvim.com/oauth/token
  name: auth.getvim.com (Auth0 tenant)
  source: well-known/vim-openid-configuration.json
  type: oauth2
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: OIDC — issue an ID token.
  flows: []
  scope: openid
- description: Basic profile claims.
  flows: []
  scope: profile
- description: Email claim.
  flows: []
  scope: email
- description: Issue a refresh token.
  flows: []
  scope: offline_access
slug: vim-scopes
source_filename: vim-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: openapi/vim-data-source-openapi-original.json\ndocs: https://auth.getvim.com/.well-known/openid-configuration\n# The Data Source OpenAPI declares an oauth2 scheme with no populated scopes;\n# real client-credentials auth issues a bearer JWT (audience-scoped, not\n# scope-scoped). The Auth0 authorization server backing the Vim REST API\n# (auth.getvim.com) advertises the standard OIDC scopes below.\nschemes:\n  - name: service\n    type: oauth2\n    source: openapi/vim-data-source-openapi-original.json\n    flows:\n      - flow: implicit\n  - name: auth.getvim.com (Auth0 tenant)\n    type: oauth2\n    source: well-known/vim-openid-configuration.json\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://auth.getvim.com/oauth/token\nscopes:\n  - scope: openid\n    description: OIDC — issue an ID token.\n    sources: [well-known/vim-openid-configuration.json]\n  - scope: profile\n    description: Basic profile\
  \ claims.\n    sources: [well-known/vim-openid-configuration.json]\n  - scope: email\n    description: Email claim.\n    sources: [well-known/vim-openid-configuration.json]\n  - scope: offline_access\n    description: Issue a refresh token.\n    sources: [well-known/vim-openid-configuration.json]\nnotes: >-\n  scopes_supported at auth.getvim.com also includes name, given_name,\n  family_name, nickname, email_verified, picture, created_at, identities, phone,\n  address. Machine-to-machine Data Source access uses the client_credentials\n  grant with an audience rather than granular scopes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vim/refs/heads/main/scopes/vim-scopes.yml
summary_line: 4 scopes · implicit/clientCredentials
tags:
- Healthcare
- United States
- Clinical AI
- EHR Integration
- Point of Care
- Interoperability
- Value-Based Care
- Care Gaps
- Authentication
token_urls:
- https://auth.getvim.com/oauth/token
---
