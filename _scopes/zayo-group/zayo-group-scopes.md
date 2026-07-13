---
api_specs:
- filename: zayo-group-openapi.yml
  format: yaml
  label: Zayo Group Holdings API
  slug: zayo-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zayo-group/refs/heads/main/openapi/zayo-group-openapi.yml
authorization_urls: []
description: ''
docs: https://developer.zayo.com/docs/getting-started
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Zayo Group Scopes
name_suffix: OAuth Scopes
note: Zayo APIs use OAuth 2.0 client_credentials only; the Getting Started docs show a single standard `openid` scope in the token request and publish no granular permission scopes — access is governed by the issued client credentials (https://developer.zayo.com/docs/getting-started).
overview: 'Zayo Group Holdings publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Zayo Group Holdings API on a user''s behalf.


  Tokens are issued from https://auth.api.zayo.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Zayo Group Holdings
provider_slug: zayo-group
schemes:
- description: 'OAuth 2.0 Client Credentials grant. Exchange client_id / client_secret at

    the authorization server token endpoint for a short-lived bearer token

    (tokens expire hourly).'
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.api.zayo.com/oauth/token
  name: oauth2ClientCredentials
  source: openapi/zayo-group-openapi.yml
scope_count: 1
scope_names:
- openid
scopes:
- description: Standard OpenID Connect scope; the only scope value Zayo's docs instruct clients to include in the client_credentials token request. Zayo does not publish granular per-API permission scopes.
  flows: []
  scope: openid
slug: zayo-group-scopes
source_filename: zayo-group-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/zayo-group-openapi.yml\ndocs: https://developer.zayo.com/docs/getting-started\nnote: >-\n  Zayo APIs use OAuth 2.0 client_credentials only; the Getting Started docs\n  show a single standard `openid` scope in the token request and publish no\n  granular permission scopes — access is governed by the issued client\n  credentials (https://developer.zayo.com/docs/getting-started).\nschemes:\n- name: oauth2ClientCredentials\n  source: openapi/zayo-group-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.api.zayo.com/oauth/token\n  description: |-\n    OAuth 2.0 Client Credentials grant. Exchange client_id / client_secret at\n    the authorization server token endpoint for a short-lived bearer token\n    (tokens expire hourly).\nscopes:\n- scope: openid\n  description: >-\n    Standard OpenID Connect scope; the only scope value Zayo's docs instruct\n    clients to include in the client_credentials\
  \ token request. Zayo does not\n    publish granular per-API permission scopes.\n  sources:\n  - https://developer.zayo.com/docs/getting-started\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zayo-group/refs/heads/main/scopes/zayo-group-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Fiber
- Network
- Infrastructure
token_urls:
- https://auth.api.zayo.com/oauth/token
---
