---
api_specs:
- filename: ariba-sourcing-approval-tasks-api-openapi.yml
  format: yaml
  label: Ariba Sourcing Approval Tasks API
  slug: ariba-sourcing-approval-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ariba-sourcing/refs/heads/main/openapi/ariba-sourcing-approval-tasks-api-openapi.yml
- filename: ariba-sourcing-documents-api-openapi.yml
  format: yaml
  label: Ariba Sourcing Documents API
  slug: ariba-sourcing-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ariba-sourcing/refs/heads/main/openapi/ariba-sourcing-documents-api-openapi.yml
- filename: ariba-sourcing-groups-api-openapi.yml
  format: yaml
  label: Ariba Sourcing Groups API
  slug: ariba-sourcing-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ariba-sourcing/refs/heads/main/openapi/ariba-sourcing-groups-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Ariba Sourcing Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Ariba Sourcing uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.ariba.com/v2/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Ariba Sourcing
provider_slug: ariba-sourcing
schemes:
- description: OAuth 2.0 authentication. Obtain access token from https://api.ariba.com/v2/oauth/token using client credentials.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.ariba.com/v2/oauth/token
  name: OAuth2
  source: openapi/ariba-sourcing-approval-tasks-api-openapi.yml
- description: OAuth 2.0 authentication. Obtain access token from https://api.ariba.com/v2/oauth/token using client credentials.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.ariba.com/v2/oauth/token
  name: OAuth2
  source: openapi/ariba-sourcing-documents-api-openapi.yml
- description: OAuth 2.0 authentication. Obtain access token from https://api.ariba.com/v2/oauth/token using client credentials.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.ariba.com/v2/oauth/token
  name: OAuth2
  source: openapi/ariba-sourcing-groups-api-openapi.yml
- description: OAuth 2.0 authentication. Obtain access token from https://api.ariba.com/v2/oauth/token using client credentials.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.ariba.com/v2/oauth/token
  name: OAuth2
  source: openapi/ariba-sourcing-external-approval-api.yaml
scope_count: 0
scope_names: []
scopes: []
slug: ariba-sourcing-scopes
source_filename: ariba-sourcing-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/ariba-sourcing-approval-tasks-api-openapi.yml, openapi/ariba-sourcing-documents-api-openapi.yml,\n  openapi/ariba-sourcing-external-approval-api.yaml, openapi/ariba-sourcing-groups-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/ariba-sourcing-approval-tasks-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.ariba.com/v2/oauth/token\n  description: OAuth 2.0 authentication. Obtain access token from https://api.ariba.com/v2/oauth/token\n    using client credentials.\n- name: OAuth2\n  source: openapi/ariba-sourcing-documents-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.ariba.com/v2/oauth/token\n  description: OAuth 2.0 authentication. Obtain access token from https://api.ariba.com/v2/oauth/token\n    using client credentials.\n- name: OAuth2\n  source: openapi/ariba-sourcing-groups-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n   \
  \ tokenUrl: https://api.ariba.com/v2/oauth/token\n  description: OAuth 2.0 authentication. Obtain access token from https://api.ariba.com/v2/oauth/token\n    using client credentials.\n- name: OAuth2\n  source: openapi/ariba-sourcing-external-approval-api.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.ariba.com/v2/oauth/token\n  description: OAuth 2.0 authentication. Obtain access token from https://api.ariba.com/v2/oauth/token\n    using client credentials.\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ariba-sourcing/refs/heads/main/scopes/ariba-sourcing-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Approvals
- Auctions
- B2B
- Contracts
- Procurement
- RFx
- SAP
- Sourcing
- Supplier Management
- Supply Chain
token_bound: false
token_urls:
- https://api.ariba.com/v2/oauth/token
---
