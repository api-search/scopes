---
api_specs:
- filename: litmus-hiring-openapi.yml
  format: yaml
  label: Litmus Hiring REST API
  slug: litmus-hiring-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litmus-hiring/refs/heads/main/openapi/litmus-hiring-openapi.yml
authorization_urls:
- https://clerk.litmushiring.com/oauth/authorize
description: ''
docs: https://clerk.com/docs/oauth/scoped-access
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Litmus Hiring Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Litmus Hiring publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Litmus Hiring API on a user''s behalf.


  Tokens are issued from https://clerk.litmushiring.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Litmus Hiring
provider_slug: litmus-hiring
schemes:
- flows:
  - authorizationUrl: https://clerk.litmushiring.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://clerk.litmushiring.com/oauth/token
  name: clerkOAuth
  source: well-known/litmus-hiring-oauth-authorization-server.json
scope_count: 7
scope_names:
- openid
- profile
- email
- public_metadata
- private_metadata
- offline_access
- user:org:read
scopes:
- description: OpenID Connect sign-in; issue an ID token identifying the user.
  flows: []
  scope: openid
- description: Access the user's basic profile claims (name).
  flows: []
  scope: profile
- description: Access the user's email address.
  flows: []
  scope: email
- description: Read the user's public metadata.
  flows: []
  scope: public_metadata
- description: Read the user's private metadata.
  flows: []
  scope: private_metadata
- description: Issue a refresh token for long-lived, non-interactive access.
  flows: []
  scope: offline_access
- description: Read the user's organization membership and organization-scoped data.
  flows: []
  scope: user:org:read
slug: litmus-hiring-scopes
source_filename: litmus-hiring-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: well-known/litmus-hiring-oauth-authorization-server.json\ndocs: https://clerk.com/docs/oauth/scoped-access\nnotes: >-\n  OAuth scopes apply to the hosted MCP server's Clerk OAuth flow (interactive\n  agent clients). The REST API itself is authenticated with an\n  organization-scoped bearer API key and does not expose a scope surface.\nschemes:\n  - name: clerkOAuth\n    source: well-known/litmus-hiring-oauth-authorization-server.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://clerk.litmushiring.com/oauth/authorize\n        tokenUrl: https://clerk.litmushiring.com/oauth/token\nscopes:\n  - scope: openid\n    description: OpenID Connect sign-in; issue an ID token identifying the user.\n  - scope: profile\n    description: Access the user's basic profile claims (name).\n  - scope: email\n    description: Access the user's email address.\n  - scope: public_metadata\n    description: Read the\
  \ user's public metadata.\n  - scope: private_metadata\n    description: Read the user's private metadata.\n  - scope: offline_access\n    description: Issue a refresh token for long-lived, non-interactive access.\n  - scope: 'user:org:read'\n    description: Read the user's organization membership and organization-scoped data.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/litmus-hiring/refs/heads/main/scopes/litmus-hiring-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Company
- Hiring
- Recruitment
- Technical Assessment
- Developer Hiring
- MCP
- Interviewing
- Y Combinator
token_urls:
- https://clerk.litmushiring.com/oauth/token
---
