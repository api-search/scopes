---
api_specs:
- filename: ecosio-approval-request-status-api-openapi.yml
  format: yaml
  label: ecosio Approval Request Status API
  slug: ecosio-approval-request-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecosio/openapi/ecosio-approval-request-status-api-openapi.yml
- filename: ecosio-archive-messages-api-openapi.yml
  format: yaml
  label: ecosio Archive messages API
  slug: ecosio-archive-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecosio/openapi/ecosio-archive-messages-api-openapi.yml
- filename: ecosio-check-user-credentials-api-openapi.yml
  format: yaml
  label: ecosio Check user credentials API
  slug: ecosio-check-user-credentials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecosio/openapi/ecosio-check-user-credentials-api-openapi.yml
- filename: ecosio-companies-api-openapi.yml
  format: yaml
  label: ecosio Companies API
  slug: ecosio-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecosio/openapi/ecosio-companies-api-openapi.yml
- filename: ecosio-connectors-api-openapi.yml
  format: yaml
  label: ecosio Connectors API
  slug: ecosio-connectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecosio/openapi/ecosio-connectors-api-openapi.yml
- filename: ecosio-deliver-messages-to-the-hub-api-openapi.yml
  format: yaml
  label: ecosio Deliver messages to the Hub API
  slug: ecosio-deliver-messages-to-the-hub-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecosio/openapi/ecosio-deliver-messages-to-the-hub-api-openapi.yml
- filename: ecosio-fetch-messages-from-the-hub-api-openapi.yml
  format: yaml
  label: ecosio Fetch messages from the Hub API
  slug: ecosio-fetch-messages-from-the-hub-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecosio/openapi/ecosio-fetch-messages-from-the-hub-api-openapi.yml
- filename: ecosio-message-controller-api-openapi.yml
  format: yaml
  label: ecosio Message Controller API
  slug: ecosio-message-controller-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecosio/openapi/ecosio-message-controller-api-openapi.yml
- filename: ecosio-request-the-documents-for-an-e-invoice-api-openapi.yml
  format: yaml
  label: ecosio Request the documents for an e-invoice API
  slug: ecosio-request-the-documents-for-an-e-invoice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecosio/openapi/ecosio-request-the-documents-for-an-e-invoice-api-openapi.yml
- filename: ecosio-scenarios-api-openapi.yml
  format: yaml
  label: ecosio Scenarios API
  slug: ecosio-scenarios-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecosio/openapi/ecosio-scenarios-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Ecosio Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'ecosio uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://dev-auth.vtxdev.net/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ecosio
provider_slug: ecosio
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://dev-auth.vtxdev.net/oauth/token
  name: oauth2_client_credentials_flow
  source: openapi/ecosio-vertex-messaging-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: ecosio-scopes
source_filename: ecosio-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: none\nsource: openapi/ecosio-vertex-messaging-api-openapi.yml\nschemes:\n- name: oauth2_client_credentials_flow\n  source: openapi/ecosio-vertex-messaging-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://dev-auth.vtxdev.net/oauth/token\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://artifacts.apis.io/ecosio/scopes/ecosio-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- EDI
- E-Invoicing
- B2B Integration
- VAT Compliance
- PEPPOL
- Supply Chain
- Messaging
token_bound: false
token_urls:
- https://dev-auth.vtxdev.net/oauth/token
---
