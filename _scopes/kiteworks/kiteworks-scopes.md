---
api_specs:
- filename: kiteworks-core-openapi-original.json
  format: json
  label: Kiteworks Core API
  slug: core
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kiteworks/refs/heads/main/openapi/kiteworks-core-openapi-original.json
- filename: kiteworks-pubsub-openapi-original.yml
  format: yaml
  label: Kiteworks PubSub Consumer API
  slug: pubsub
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kiteworks/refs/heads/main/openapi/kiteworks-pubsub-openapi-original.yml
authorization_urls:
- https://{kiteworks_server}/oauth/authorize
description: ''
docs: https://developer.kiteworks.com/authentication.html
flows:
- authorizationCode
- jwt-bearer
kind: oauth-scopes
layout: scope
method: searched
name: Kiteworks Scopes
name_suffix: OAuth Scopes
note: 'Kiteworks does not publish a fixed enumerated scope list. Scopes are configured per custom application in the Admin console and requested as a space-separated list. The scope grammar is hierarchical and pattern-based: {HTTP_METHOD}/{resource}/{qualifier}, where * is a wildcard in any position. The derive-oauth-scopes.py baseline returns nothing because the published v28 OpenAPI declares no securitySchemes.'
overview: 'Kiteworks uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://{kiteworks_server}/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kiteworks
provider_slug: kiteworks
schemes:
- flows:
  - authorizationUrl: https://{kiteworks_server}/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://{kiteworks_server}/oauth/token
  - flow: jwt-bearer
    tokenUrl: https://{kiteworks_server}/oauth/token
  name: OAuth2
  source: https://developer.kiteworks.com/authentication.html
scope_count: 0
scope_names: []
scopes: []
slug: kiteworks-scopes
source_filename: kiteworks-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developer.kiteworks.com/authentication.html\ndocs: https://developer.kiteworks.com/authentication.html\nnote: 'Kiteworks does not publish a fixed enumerated scope list. Scopes are configured per custom application\n  in the Admin console and requested as a space-separated list. The scope grammar is hierarchical and\n  pattern-based: {HTTP_METHOD}/{resource}/{qualifier}, where * is a wildcard in any position. The derive-oauth-scopes.py\n  baseline returns nothing because the published v28 OpenAPI declares no securitySchemes.'\nschemes:\n- name: OAuth2\n  source: https://developer.kiteworks.com/authentication.html\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{kiteworks_server}/oauth/authorize\n    tokenUrl: https://{kiteworks_server}/oauth/token\n  - flow: jwt-bearer\n    tokenUrl: https://{kiteworks_server}/oauth/token\ngrammar:\n  pattern: '{METHOD}/{resource}/{qualifier}'\n  delimiter: space-separated\
  \ list\n  wildcards: '* matches any value in a position'\n  methods:\n  - GET\n  - POST\n  - PUT\n  - DELETE\n  - '*'\n  configuration: Permitted scopes are whitelisted per custom application in the Kiteworks Admin console.\ndocumented_examples:\n- scope: GET/users/*\n  description: Read access across the users resource family.\n  source: authentication.html Python sample\n- scope: '*/files/*'\n  description: All methods across the files resource family.\n  source: authentication.html Python sample\nresource_families:\n  note: Scope resource segments correspond to the OpenAPI tags in openapi/kiteworks-core-openapi-original.json.\n  derived_from_spec_tags:\n  - activities\n  - admin\n  - adminRoles\n  - advancedForms\n  - cards\n  - clientEventLogs\n  - clients\n  - comments\n  - contacts\n  - devices\n  - dli\n  - externalDL\n  - favorites\n  - files\n  - folders\n  - groups\n  - internal\n  - languages\n  - ldapGroups\n  - locations\n  - mail\n  - mobileSync\n  - notifications\n  - permissions\n\
  \  - profiles\n  - requestFile\n  - roles\n  - scim\n  - search\n  - settings\n  - sharedMailbox\n  - shortLinks\n  - sourceTypes\n  - sources\n  - system\n  - tasks\n  - uploads\n  - userSshPublicKeys\n  - users\n  - webForms\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kiteworks/refs/heads/main/scopes/kiteworks-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Secure File Sharing
- Managed File Transfer
- Secure Email
- Data Governance
- Regulatory Compliance
- Content Security
- Private Data Network
- CMMC
- SCIM
token_urls:
- https://{kiteworks_server}/oauth/token
---
