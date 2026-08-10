---
authorization_urls: []
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: probed
name: Callminer Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CallMiner publishes 5 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the CallMiner API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CallMiner
provider_slug: callminer
schemes:
- authorization_url: https://idp.callminer.net/connect/authorize
  flows:
  - authorizationCode
  - clientCredentials
  name: CallMinerOAuth2
  token_url: https://idp.callminer.net/connect/token
scope_count: 5
scope_names:
- openid
- profile
- offline_access
- https://callminer.net/auth/platform-ingestion
- https://callminer.net/auth/platform-bulkexport
scopes:
- description: OpenID Connect authentication; returns an id_token.
  flows:
  - authorizationCode
  scope: openid
- description: Standard OpenID Connect profile claims for the signed-in user.
  flows:
  - authorizationCode
  scope: profile
- description: Issue a refresh token so the client can obtain new access tokens without user interaction.
  flows:
  - authorizationCode
  scope: offline_access
- description: Access to the CallMiner Eureka Ingestion API surface — adding and updating media and metadata for contacts. Observed as the resource scope requested by the Swagger UI served at https://api.callminer.net/swagger.
  flows:
  - authorizationCode
  scope: https://callminer.net/auth/platform-ingestion
- description: Access to the CallMiner Eureka Bulk Export API surface — creating and retrieving bulk export jobs. Observed as the resource scope requested by the Swagger UI served at https://api.callminer.net/bulkexport/swagger.
  flows:
  - authorizationCode
  scope: https://callminer.net/auth/platform-bulkexport
slug: callminer-scopes
source_filename: callminer-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: https://api.callminer.net/swagger\nnotes: >-\n  CallMiner publishes no public scope reference. The scopes below were observed\n  on the wire: the OpenID Connect discovery document advertises only\n  offline_access under scopes_supported, while CallMiner's own first-party\n  Swagger UIs request resource scopes in their /connect/authorize redirects.\n  Those resource scopes are recorded verbatim from the observed Location header.\n  This is not a complete scope catalog — a full list would require the gated\n  documentation or authenticated introspection.\ndocs: null\nschemes:\n- name: CallMinerOAuth2\n  authorization_url: https://idp.callminer.net/connect/authorize\n  token_url: https://idp.callminer.net/connect/token\n  flows:\n  - authorizationCode\n  - clientCredentials\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; returns an id_token.\n  kind: standard\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - https://api.callminer.net/swagger\n- scope: profile\n  description: Standard OpenID Connect profile claims for the signed-in user.\n  kind: standard\n  flows:\n  - authorizationCode\n  sources:\n  - https://api.callminer.net/swagger\n- scope: offline_access\n  description: Issue a refresh token so the client can obtain new access tokens without user interaction.\n  kind: standard\n  flows:\n  - authorizationCode\n  sources:\n  - https://idp.callminer.net/.well-known/openid-configuration\n  - https://api.callminer.net/swagger\n- scope: https://callminer.net/auth/platform-ingestion\n  description: >-\n    Access to the CallMiner Eureka Ingestion API surface — adding and updating\n    media and metadata for contacts. Observed as the resource scope requested by\n    the Swagger UI served at https://api.callminer.net/swagger.\n  kind: resource\n  api: CallMiner Eureka Ingestion API\n  flows:\n  - authorizationCode\n  sources:\n  - https://api.callminer.net/swagger\n- scope: https://callminer.net/auth/platform-bulkexport\n\
  \  description: >-\n    Access to the CallMiner Eureka Bulk Export API surface — creating and\n    retrieving bulk export jobs. Observed as the resource scope requested by the\n    Swagger UI served at https://api.callminer.net/bulkexport/swagger.\n  kind: resource\n  api: CallMiner Eureka Bulk Export API\n  flows:\n  - authorizationCode\n  sources:\n  - https://api.callminer.net/bulkexport/swagger\ncompleteness:\n  complete: false\n  reason: >-\n    scopes_supported in the discovery document lists only offline_access, so the\n    resource scopes are not enumerable anonymously. Only the two resource scopes\n    CallMiner's own UIs request could be observed.\nx-evidence:\n  fetched: '2026-08-09'\n  evidence:\n  - url: https://idp.callminer.net/.well-known/openid-configuration\n    http_status: 200\n  - url: https://api.callminer.net/swagger\n    http_status: 302\n  - url: https://api.callminer.net/bulkexport/swagger\n    http_status: 302\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/callminer/refs/heads/main/scopes/callminer-scopes.yml
summary_line: 5 scopes · authorizationCode/clientCredentials
tags:
- Company
- Conversation Intelligence
- Speech Analytics
- Contact Center
- Customer Experience
- Artificial Intelligence
- Analytics
- Transcription
- Quality Management
- Compliance
token_urls: []
---
