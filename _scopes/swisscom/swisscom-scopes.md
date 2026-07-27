---
api_specs:
- filename: swisscom-sign-integration-api-openapi.json
  format: json
  label: Swisscom Sign Integration API
  slug: swisscom-sign-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swisscom/refs/heads/main/openapi/swisscom-sign-integration-api-openapi.json
- filename: swisscom-all-in-signing-service-openapi.yml
  format: yaml
  label: Swisscom All-in Signing Service (AIS) API
  slug: swisscom-all-in-signing-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swisscom/refs/heads/main/openapi/swisscom-all-in-signing-service-openapi.yml
authorization_urls: []
description: ''
docs: https://sign.swisscom.ch/docs/guide/authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Swisscom Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Swisscom publishes 3 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Swisscom API on a user''s behalf.


  Tokens are issued from https://sign.swisscom.ch/realms/swisscom-public/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Swisscom
provider_slug: swisscom
schemes:
- description: OAuth 2.0 Client Credentials flow for accessing the Swisscom Sign Integration API.
  flows:
  - flow: clientCredentials
    tokenUrl: https://sign.swisscom.ch/realms/swisscom-public/protocol/openid-connect/token
  name: SwisscomSignOAuth2
  source: openapi/swisscom-sign-integration-api-openapi.json
scope_count: 3
scope_names:
- sswp:process:create
- sswp:process:read
- sswp:process:read:all
scopes:
- description: Create, configure, and submit a new signature process including documents, invitees, and signature options.
  flows:
  - clientCredentials
  scope: sswp:process:create
- description: Read process metadata or download associated documents.
  flows:
  - clientCredentials
  scope: sswp:process:read
- description: Read metadata of all processes within the organization, with optional filtering.
  flows:
  - clientCredentials
  scope: sswp:process:read:all
slug: swisscom-scopes
source_filename: swisscom-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: openapi/swisscom-sign-integration-api-openapi.json\ndocs: https://sign.swisscom.ch/docs/guide/authentication\nlegacy_docs: https://github.com/swisscom-api/doc/wiki/oauth-scopes.html\nschemes:\n- name: SwisscomSignOAuth2\n  source: openapi/swisscom-sign-integration-api-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://sign.swisscom.ch/realms/swisscom-public/protocol/openid-connect/token\n  description: OAuth 2.0 Client Credentials flow for accessing the Swisscom Sign Integration\n    API.\nscopes:\n- scope: sswp:process:create\n  description: Create, configure, and submit a new signature process including documents, invitees,\n    and signature options.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/swisscom-sign-integration-api-openapi.json\n- scope: sswp:process:read\n  description: Read process metadata or download associated documents.\n  flows:\n  - clientCredentials\n  sources:\n  -\
  \ openapi/swisscom-sign-integration-api-openapi.json\n- scope: sswp:process:read:all\n  description: Read metadata of all processes within the organization, with optional filtering.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/swisscom-sign-integration-api-openapi.json\nissuer: https://sign.swisscom.ch/realms/swisscom-public\njwks_uri: https://sign.swisscom.ch/realms/swisscom-public/protocol/openid-connect/certs\naudience: swisscom-sign-api\ntenancy_claim: organization_id\nscope_usage:\n- scope: sswp:process:create\n  operations: [create, setup, release, attach]\n- scope: sswp:process:read\n  operations: [open, getProcess, getStatus, getRecords, getFile, getFileContent]\n- scope: sswp:process:read:all\n  operations: [findAll]\ncredential_issuance: >-\n  Client id and secret are generated per subscription in the Swisscom Sign cockpit under the API\n  Credentials tab; TEST and production credentials are issued separately on their respective hosts.\nother_surfaces:\n- surface:\
  \ api.swisscom.com legacy gateway\n  docs: https://github.com/swisscom-api/doc/wiki/oauth-scopes.html\n  authorization_endpoint: https://consent.swisscom.com/c/oauth2/auth\n  token_endpoint: https://consent.swisscom.com/o/oauth2/token\n  convention: '<action>-<resource>, where action is read or write; space-delimited in the scope parameter'\n  published_examples:\n  - read-basicprofile\n  - read-phone\n  - read-email\n  - read-voip-callforwardings\n  - write-voip-callforwardings\n  note: >-\n    Documented in the swisscom-api wiki as examples, not as a complete scope registry. The full scope\n    list for the marketplace products sits behind the Swisscom login and is not machine-readable.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swisscom/refs/heads/main/scopes/swisscom-scopes.yml
summary_line: 3 scopes · clientCredentials
tags:
- Telecommunications
- Switzerland
- Mobile Network Operator
- Broadband
- Network APIs
- Open Gateway
- Messaging
- SMS
- Voice
- Identity Verification
- Mobility Data
- Digital Signatures
- eSIM
- Artificial Intelligence
token_urls:
- https://sign.swisscom.ch/realms/swisscom-public/protocol/openid-connect/token
---
