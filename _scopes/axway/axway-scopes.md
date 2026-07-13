---
api_specs:
- filename: axway-amplify-platform-openapi-original.json
  format: json
  label: Axway Amplify Platform API
  slug: axway-amplify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axway/refs/heads/main/openapi/axway-amplify-platform-openapi-original.json
authorization_urls:
- https://login.axway.com/auth/realms/Broker/openid-connect/auth
description: ''
docs: https://blog.axway.com/product-insights/amplify-platform/axway-amplify-platform-api-calls
flows:
- clientCredentials
- authorizationCode
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Axway Scopes
name_suffix: OAuth Scopes
note: Axway does not publish OAuth scopes for the Amplify Platform API; authorization is handled through org roles assigned to client-secret service accounts, and tokens carry only generic OIDC scopes (see https://blog.axway.com/product-insights/amplify-platform/axway-amplify-platform-api-calls).
overview: 'Axway uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://login.axway.com/auth/realms/Broker/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Axway
provider_slug: axway
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://login.axway.com/auth/realms/Broker/protocol/openid-connect/token
  - authorizationUrl: https://login.axway.com/auth/realms/Broker/openid-connect/auth
    flow: authorizationCode
    tokenUrl: https://login.axway.com/auth/realms/Broker/openid-connect/token
  - authorizationUrl: https://login.axway.com/auth/realms/Broker/openid-connect/auth
    flow: implicit
  name: OAuth2
  source: openapi/axway-amplify-platform-openapi-original.json
scope_count: 0
scope_names: []
scopes: []
slug: axway-scopes
source_filename: axway-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/axway-amplify-platform-openapi-original.json\ndocs: https://blog.axway.com/product-insights/amplify-platform/axway-amplify-platform-api-calls\nnote: >-\n  Axway does not publish OAuth scopes for the Amplify Platform API; authorization is\n  handled through org roles assigned to client-secret service accounts, and tokens carry\n  only generic OIDC scopes (see\n  https://blog.axway.com/product-insights/amplify-platform/axway-amplify-platform-api-calls).\nschemes:\n- name: OAuth2\n  source: openapi/axway-amplify-platform-openapi-original.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.axway.com/auth/realms/Broker/protocol/openid-connect/token\n  - flow: authorizationCode\n    authorizationUrl: https://login.axway.com/auth/realms/Broker/openid-connect/auth\n    tokenUrl: https://login.axway.com/auth/realms/Broker/openid-connect/token\n  - flow: implicit\n    authorizationUrl: https://login.axway.com/auth/realms/Broker/openid-connect/auth\n\
  scopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axway/refs/heads/main/scopes/axway-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- API Management
- Enterprise
- Integration
- Security
token_urls:
- https://login.axway.com/auth/realms/Broker/protocol/openid-connect/token
- https://login.axway.com/auth/realms/Broker/openid-connect/token
---
