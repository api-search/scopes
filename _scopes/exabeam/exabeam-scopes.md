---
authorization_urls:
- https://api.us-west.exabeam.cloud/oauth/authorize
description: ''
docs: https://developers.exabeam.com/exabeam/docs/api-keys
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Exabeam Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Exabeam publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Exabeam API on a user''s behalf.


  Tokens are issued from https://api.us-west.exabeam.cloud/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Exabeam
provider_slug: exabeam
schemes:
- flows:
  - authorizationUrl: https://api.us-west.exabeam.cloud/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.us-west.exabeam.cloud/oauth/token
  name: OAuth2
  source: https://api.us-west.exabeam.cloud/.well-known/oauth-authorization-server
scope_count: 3
scope_names:
- openid
- profile
- offline_access
scopes:
- description: OpenID Connect authentication.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the authenticated principal's profile.
  flows:
  - authorizationCode
  scope: profile
- description: Issue a refresh token for continued (offline) access.
  flows:
  - authorizationCode
  scope: offline_access
slug: exabeam-scopes
source_filename: exabeam-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api.us-west.exabeam.cloud/.well-known/oauth-authorization-server\ndocs: https://developers.exabeam.com/exabeam/docs/api-keys\nschemes:\n- name: OAuth2\n  source: https://api.us-west.exabeam.cloud/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.us-west.exabeam.cloud/oauth/authorize\n    tokenUrl: https://api.us-west.exabeam.cloud/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication.\n  flows: [authorizationCode]\n  sources: [well-known/exabeam-oauth-authorization-server.json]\n- scope: profile\n  description: Access to the authenticated principal's profile.\n  flows: [authorizationCode]\n  sources: [well-known/exabeam-oauth-authorization-server.json]\n- scope: offline_access\n  description: Issue a refresh token for continued (offline) access.\n  flows: [authorizationCode]\n  sources: [well-known/exabeam-oauth-authorization-server.json]\n\
  notes: >-\n  Scopes are taken verbatim from the published RFC 8414 authorization-server\n  metadata (scope: \"openid profile offline_access\"). Fine-grained,\n  product-level API permissions are governed by the role assigned to the API\n  key in the Exabeam console rather than by additional OAuth scopes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exabeam/refs/heads/main/scopes/exabeam-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- Cybersecurity
- Security
- SIEM
- UEBA
- Threat Detection
- Security Operations
- SOC
- Log Management
- Incident Response
token_urls:
- https://api.us-west.exabeam.cloud/oauth/token
---
