---
authorization_urls: []
description: ''
docs: https://community.centralreach.com/s/article/knowledge-api-permissions
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Centralreach Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CentralReach publishes 4 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the CentralReach API on a user''s behalf.


  Tokens are issued from https://login.centralreach.com/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CentralReach
provider_slug: centralreach
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://login.centralreach.com/connect/token
  name: clientCredentials
  source: https://login.centralreach.com/.well-known/openid-configuration
scope_count: 4
scope_names:
- openid
- cr
- cr-api
- offline_access
scopes:
- description: OpenID Connect authentication scope; requests an ID token identifying the subject.
  flows:
  - clientCredentials
  scope: openid
- description: CentralReach platform access scope.
  flows:
  - clientCredentials
  scope: cr
- description: Access to the CentralReach Enhanced API (partners-api enterprise endpoints).
  flows:
  - clientCredentials
  scope: cr-api
- description: Requests a refresh token for long-lived, offline access.
  flows:
  - clientCredentials
  scope: offline_access
slug: centralreach-scopes
source_filename: centralreach-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://login.centralreach.com/.well-known/openid-configuration\ndocs: https://community.centralreach.com/s/article/knowledge-api-permissions\nschemes:\n- name: clientCredentials\n  source: https://login.centralreach.com/.well-known/openid-configuration\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.centralreach.com/connect/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication scope; requests an ID token identifying the subject.\n  flows: [clientCredentials]\n  sources: [https://login.centralreach.com/.well-known/openid-configuration]\n- scope: cr\n  description: CentralReach platform access scope.\n  flows: [clientCredentials]\n  sources: [https://login.centralreach.com/.well-known/openid-configuration]\n- scope: cr-api\n  description: Access to the CentralReach Enhanced API (partners-api enterprise endpoints).\n  flows: [clientCredentials]\n  sources: [https://login.centralreach.com/.well-known/openid-configuration]\n\
  - scope: offline_access\n  description: Requests a refresh token for long-lived, offline access.\n  flows: [clientCredentials]\n  sources: [https://login.centralreach.com/.well-known/openid-configuration]\nnotes: >-\n  scopes_supported advertised by the CentralReach OpenID Connect discovery\n  document. Fine-grained per-endpoint API permissions are additionally governed\n  by organization-level API permissions (see the API Permissions knowledge\n  article); those permission grants are administered in-app rather than expressed\n  as OAuth scopes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centralreach/refs/heads/main/scopes/centralreach-scopes.yml
summary_line: 4 scopes · clientCredentials
tags:
- Company
- Healthcare
- ABA Therapy
- Autism
- IDD
- EMR
- Practice Management
- Behavioral Health
- Special Education
- Billing
- OAuth
token_urls:
- https://login.centralreach.com/connect/token
---
