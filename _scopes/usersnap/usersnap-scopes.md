---
api_specs:
- filename: usersnap-api-openapi-original.json
  format: json
  label: Usersnap Platform REST API
  slug: usersnap-platform-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usersnap/refs/heads/main/openapi/usersnap-api-openapi-original.json
authorization_urls:
- https://id.usersnap.com/auth/oauth2/authorize
description: ''
docs: https://help.usersnap.com/docs/mcp-connector
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Usersnap Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Usersnap publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Usersnap API on a user''s behalf.


  Tokens are issued from https://id.usersnap.com/auth/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Usersnap
provider_slug: usersnap
schemes:
- flows:
  - authorizationUrl: https://id.usersnap.com/auth/oauth2/authorize
    flow: authorizationCode
    pkce: S256
    refresh_token: true
    tokenUrl: https://id.usersnap.com/auth/oauth2/token
  issuer: https://id.usersnap.com
  name: usersnap-oauth
  registrationUrl: https://id.usersnap.com/auth/oauth2/register
  revocationUrl: https://id.usersnap.com/auth/oauth2/revoke
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - none
scope_count: 2
scope_names:
- read:feedback
- write:opportunity
scopes:
- description: Read access to feedback data (as scoped to the authorizing user's permissions).
  flows:
  - authorizationCode
  scope: read:feedback
- description: Create Opportunities and link feedback; cannot edit or delete existing feedback.
  flows:
  - authorizationCode
  scope: write:opportunity
slug: usersnap-scopes
source_filename: usersnap-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://id.usersnap.com/.well-known/oauth-authorization-server\ndocs: https://help.usersnap.com/docs/mcp-connector\nnotes: >-\n  OAuth scopes published in Usersnap's RFC 8414 authorization-server metadata\n  (issuer id.usersnap.com), used by the hosted MCP connector\n  (mcp.usersnap.com/mcp) via OAuth 2.1 authorization_code + PKCE (S256).\n  The platform REST API itself uses self-signed JWT bearer auth, not OAuth\n  (see authentication/usersnap-authentication.yml).\nschemes:\n  - name: usersnap-oauth\n    issuer: https://id.usersnap.com\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://id.usersnap.com/auth/oauth2/authorize\n        tokenUrl: https://id.usersnap.com/auth/oauth2/token\n        refresh_token: true\n        pkce: S256\n    revocationUrl: https://id.usersnap.com/auth/oauth2/revoke\n    registrationUrl: https://id.usersnap.com/auth/oauth2/register\n    token_endpoint_auth_methods: [client_secret_basic,\
  \ client_secret_post, none]\nscopes:\n  - scope: read:feedback\n    description: Read access to feedback data (as scoped to the authorizing user's permissions).\n    flows: [authorizationCode]\n    sources: [https://id.usersnap.com/.well-known/oauth-authorization-server]\n  - scope: write:opportunity\n    description: Create Opportunities and link feedback; cannot edit or delete existing feedback.\n    flows: [authorizationCode]\n    sources: [https://id.usersnap.com/.well-known/oauth-authorization-server]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usersnap/refs/heads/main/scopes/usersnap-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Feedback
- Bug Tracking
- Customer Experience
- Product Management
- Surveys
- SaaS
token_urls:
- https://id.usersnap.com/auth/oauth2/token
---
