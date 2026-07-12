---
authorization_urls: []
description: ''
docs: https://developer.mashery.com/docs/read/mashery_api/30/Authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Tibco Scopes
name_suffix: OAuth Scopes
note: TIBCO does not publish a named OAuth scope catalog — the Mashery V3 API's scope parameter carries the customer's Mashery Area UUID rather than permissions (https://developer.mashery.com/docs/read/mashery_api/30/Authentication), and TIBCO Cloud access tokens are scoped to product domains (e.g. TSC, TCI) with permissions governed by user roles rather than documented scopes.
overview: 'TIBCO uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.mashery.com/v3/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: TIBCO
provider_slug: tibco
schemes:
- description: OAuth 2.0 client credentials for Mashery API access
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.mashery.com/v3/token
  name: oauth2
  source: openapi/tibco-mashery-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: tibco-scopes
source_filename: tibco-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tibco-mashery-openapi.yml\ndocs: https://developer.mashery.com/docs/read/mashery_api/30/Authentication\nnote: >-\n  TIBCO does not publish a named OAuth scope catalog — the Mashery V3 API's scope\n  parameter carries the customer's Mashery Area UUID rather than permissions\n  (https://developer.mashery.com/docs/read/mashery_api/30/Authentication), and TIBCO\n  Cloud access tokens are scoped to product domains (e.g. TSC, TCI) with permissions\n  governed by user roles rather than documented scopes.\nschemes:\n- name: oauth2\n  source: openapi/tibco-mashery-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.mashery.com/v3/token\n  description: OAuth 2.0 client credentials for Mashery API access\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tibco/refs/heads/main/scopes/tibco-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Analytics
- API Management
- Cloud
- Enterprise Software
- Integration
- Messaging
- Real-Time Data
token_urls:
- https://api.mashery.com/v3/token
---
