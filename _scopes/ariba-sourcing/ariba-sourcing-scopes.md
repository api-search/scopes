---
api_specs:
- filename: ariba-sourcing-external-approval-api.yaml
  format: yaml
  label: Ariba Sourcing - External Approval API
  slug: ariba-sourcing-external-approval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ariba-sourcing/refs/heads/main/openapi/ariba-sourcing-external-approval-api.yaml
authorization_urls: []
description: ''
docs: https://help.sap.com/docs/ariba-apis/help-for-sap-ariba-developer-portal/use-of-api-gateway-and-oauth-to-authenticate-applications
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Ariba Sourcing Scopes
name_suffix: OAuth Scopes
note: SAP Ariba APIs use a two-legged OAuth client credentials flow (grant_type=client_credentials) with no scope parameter; access is governed by per-API access requests, application keys, and realm approval rather than documented OAuth scopes (https://help.sap.com/docs/ariba-apis/help-for-sap-ariba-developer-portal/use-of-api-gateway-and-oauth-to-authenticate-applications).
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
  source: openapi/ariba-sourcing-external-approval-api.yaml
scope_count: 0
scope_names: []
scopes: []
slug: ariba-sourcing-scopes
source_filename: ariba-sourcing-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ariba-sourcing-external-approval-api.yaml\ndocs: https://help.sap.com/docs/ariba-apis/help-for-sap-ariba-developer-portal/use-of-api-gateway-and-oauth-to-authenticate-applications\nnote: SAP Ariba APIs use a two-legged OAuth client credentials flow (grant_type=client_credentials)\n  with no scope parameter; access is governed by per-API access requests, application\n  keys, and realm approval rather than documented OAuth scopes (https://help.sap.com/docs/ariba-apis/help-for-sap-ariba-developer-portal/use-of-api-gateway-and-oauth-to-authenticate-applications).\nschemes:\n- name: OAuth2\n  source: openapi/ariba-sourcing-external-approval-api.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.ariba.com/v2/oauth/token\n  description: OAuth 2.0 authentication. Obtain access token from https://api.ariba.com/v2/oauth/token\n    using client credentials.\nscopes: []\n"
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
token_urls:
- https://api.ariba.com/v2/oauth/token
---
