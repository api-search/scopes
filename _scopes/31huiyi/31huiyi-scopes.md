---
api_specs:
- filename: 31huiyi-openapi.postman_collection.json
  format: json
  label: 31 OpenAPI
  slug: 31huiyi-openapi
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/31huiyi/refs/heads/main/postman/31huiyi-openapi.postman_collection.json
authorization_urls: []
description: Scope inventory read from the anonymously-published OpenID Connect discovery document on the 31 authorization server, cross-checked against the scope value the developer center tells OpenAPI clients to request. 31 publishes no per-endpoint scope/permission reference page; the documented OpenAPI client requests one coarse gateway scope plus offline_access, and authorization is enforced per client rather than per named business scope.
docs: https://api-help.31huiyi.com/zh/home
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: 31Huiyi Scopes
name_suffix: OAuth Scopes
note: ''
overview: '31huiyi publishes 9 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the 31huiyi API on a user''s behalf.


  Tokens are issued from https://oauth.31huiyi.com/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: 31huiyi
provider_slug: 31huiyi
schemes: []
scope_count: 9
scope_names:
- OpenAppGateway
- offline_access
- AppGateway
- api1
- openid
- profile
- email
- address
- roles
scopes:
- description: The scope the developer center instructs 31 OpenAPI clients to request; grants access to the /op/ gateway surface on 31api.31huiyi.com.
  flows: []
  scope: OpenAppGateway
- description: Requests a refresh_token alongside the access token (OIDC offline access).
  flows: []
  scope: offline_access
- description: Sibling gateway scope advertised by the authorization server; not documented for OpenAPI clients.
  flows: []
  scope: AppGateway
- description: Generic API scope advertised by the authorization server; not documented for OpenAPI clients.
  flows: []
  scope: api1
- description: OIDC — request an id_token.
  flows: []
  scope: openid
- description: OIDC standard profile claims.
  flows: []
  scope: profile
- description: OIDC standard email claim.
  flows: []
  scope: email
- description: OIDC standard address claim.
  flows: []
  scope: address
- description: Role claims for the authenticated subject.
  flows: []
  scope: roles
slug: 31huiyi-scopes
source_filename: 31huiyi-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: https://oauth.31huiyi.com/.well-known/openid-configuration\ndocs: https://api-help.31huiyi.com/zh/home\nname: 31huiyi OAuth scopes\ndescription: >-\n  Scope inventory read from the anonymously-published OpenID Connect discovery document on the 31\n  authorization server, cross-checked against the scope value the developer center tells OpenAPI\n  clients to request. 31 publishes no per-endpoint scope/permission reference page; the documented\n  OpenAPI client requests one coarse gateway scope plus offline_access, and authorization is enforced\n  per client rather than per named business scope.\nauthorization_server: https://oauth.31huiyi.com\ntoken_endpoint: https://oauth.31huiyi.com/connect/token\ndocumented_openapi_scope_string: offline_access OpenAppGateway\nscopes:\n- name: OpenAppGateway\n  description: >-\n    The scope the developer center instructs 31 OpenAPI clients to request; grants access to the\n    /op/ gateway surface\
  \ on 31api.31huiyi.com.\n  documented: true\n  source: https://api-help.31huiyi.com/zh/home\n- name: offline_access\n  description: Requests a refresh_token alongside the access token (OIDC offline access).\n  documented: true\n  source: https://api-help.31huiyi.com/zh/home\n- name: AppGateway\n  description: Sibling gateway scope advertised by the authorization server; not documented for OpenAPI clients.\n  documented: false\n- name: api1\n  description: Generic API scope advertised by the authorization server; not documented for OpenAPI clients.\n  documented: false\n- name: openid\n  description: OIDC — request an id_token.\n  documented: false\n- name: profile\n  description: OIDC standard profile claims.\n  documented: false\n- name: email\n  description: OIDC standard email claim.\n  documented: false\n- name: address\n  description: OIDC standard address claim.\n  documented: false\n- name: roles\n  description: Role claims for the authenticated subject.\n  documented: false\nclaims_supported:\n\
  - userid\nscope_count: 9\nnotes:\n- No granular per-operation scopes (e.g. attendee:read) are published; the gateway scope is coarse.\n- Operations under the /op/notoken/ prefix are documented as not requiring a user token.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/31huiyi/refs/heads/main/scopes/31huiyi-scopes.yml
summary_line: 9 scopes
tags:
- Company
- Event
- Event Management
- Conferences
- Exhibitions
- Registration
- Check-in
- Scheduling
- Ticketing
- Software-as-a-Service
- China
token_bound: false
token_urls:
- https://oauth.31huiyi.com/connect/token
---
