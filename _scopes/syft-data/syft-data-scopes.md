---
api_specs:
- filename: syft-data-export-api-openapi.yml
  format: yaml
  label: Syft Data Export API
  slug: syft-data-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syft-data/refs/heads/main/openapi/syft-data-export-api-openapi.yml
- filename: syft-data-lookup-api-openapi.yml
  format: yaml
  label: Syft Data Lookup API
  slug: syft-data-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syft-data/refs/heads/main/openapi/syft-data-lookup-api-openapi.yml
- filename: syft-data-events-api-openapi.yml
  format: yaml
  label: Syft Data Event Collection API
  slug: syft-data-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syft-data/refs/heads/main/openapi/syft-data-events-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.syftdata.com/ai-agents/connect
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Syft Data Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Syft Data uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Syft Data
provider_slug: syft-data
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: syft-data-scopes
source_filename: syft-data-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://app.syftdata.com/.well-known/openid-configuration\ndocs: https://docs.syftdata.com/ai-agents/connect\nsummary: >-\n  OAuth scopes advertised by the Auth0 tenant (syft-studio.us.auth0.com) that\n  backs Syft app login and the MCP server OAuth flow. These are standard OIDC\n  scopes; the REST Lookup/Export APIs use a Server Secret Key rather than scoped\n  OAuth tokens.\nissuer: https://syft-studio.us.auth0.com/\nscopes:\n  - name: openid\n    description: OpenID Connect sign-in; issues an ID token.\n  - name: profile\n    description: Access to the user's basic profile claims.\n  - name: email\n    description: Access to the user's email address.\n  - name: offline_access\n    description: Issue a refresh token for long-lived sessions.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/syft-data/refs/heads/main/scopes/syft-data-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Lead Intelligence
- Intent Data
- Website Visitor Identification
- Sales Intelligence
- Go-To-Market
- Analytics
- MCP
token_urls: []
---
