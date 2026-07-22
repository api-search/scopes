---
api_specs:
- filename: zayo-openapi-original.yml
  format: yaml
  label: Zayo APIs
  slug: zayo-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zayo/refs/heads/main/openapi/zayo-openapi-original.yml
authorization_urls: []
description: ''
docs: https://developer.zayo.com/docs/getting-started
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Zayo Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Zayo publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Zayo API on a user''s behalf.


  Tokens are issued from https://auth.api.zayo.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Zayo
provider_slug: zayo
schemes:
- description: OAuth 2.0 using the Client Credentials grant type.
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.api.zayo.com/oauth/token
  name: OAuthClientCredentials
  source: openapi/zayo-openapi-original.yml
scope_count: 1
scope_names:
- openid
scopes:
- description: openid scope
  flows:
  - clientCredentials
  scope: openid
slug: zayo-scopes
source_filename: zayo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/zayo-openapi-original.yml\ndocs: https://developer.zayo.com/docs/getting-started\nnotes: >-\n  Zayo's client-credentials flow offers a single scope, openid. No finer-grained\n  permission/scope reference is published; access is provisioned per client_id.\nschemes:\n- name: OAuthClientCredentials\n  source: openapi/zayo-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.api.zayo.com/oauth/token\n  description: OAuth 2.0 using the Client Credentials grant type.\nscopes:\n- scope: openid\n  description: openid scope\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/zayo-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zayo/refs/heads/main/scopes/zayo-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Company
- Telecommunications
- Networking
- Connectivity
- Fiber
- Infrastructure
- Bandwidth
- Cloud Connectivity
- Ordering
- Ticketing
token_urls:
- https://auth.api.zayo.com/oauth/token
---
