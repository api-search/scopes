---
authorization_urls: []
description: Tailor's platform authorization server publishes RFC 8414 metadata but does NOT advertise a scopes_supported list. The only scope vocabulary Tailor documents is the two-value read/write pair attached to personal access tokens. Application-level OAuth2 clients declare their own grant types in code; scope names are chosen by the customer building the application, not by Tailor, so there is no platform-wide scope catalog to harvest.
docs: https://docs.tailor.tech/guides/auth/overview
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Tailor Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Tailor uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Tailor
provider_slug: tailor
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: tailor-scopes
source_filename: tailor-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: https://api.tailor.tech/.well-known/oauth-authorization-server\ndocs: https://docs.tailor.tech/guides/auth/overview\nname: Tailor OAuth scopes and grants\ndescription: >-\n  Tailor's platform authorization server publishes RFC 8414 metadata but does NOT\n  advertise a scopes_supported list. The only scope vocabulary Tailor documents is the\n  two-value read/write pair attached to personal access tokens. Application-level OAuth2\n  clients declare their own grant types in code; scope names are chosen by the customer\n  building the application, not by Tailor, so there is no platform-wide scope catalog to\n  harvest.\nauthorization_server: https://api.tailor.tech\nscopes_supported_published: false\nscopes:\n- name: read\n  description: Read access for a Tailor personal access token.\n  surface: personal-access-token\n  source: https://github.com/tailor-platform/tailor-mcp#authentication\n- name: write\n  description: Write access\
  \ for a Tailor personal access token.\n  surface: personal-access-token\n  source: https://github.com/tailor-platform/tailor-mcp#authentication\ngrant_types_supported:\n- authorization_code\n- refresh_token\n- client_credentials\nresponse_types_supported:\n- code\ncode_challenge_methods_supported:\n- S256\ngaps:\n- >-\n  scopes_supported is absent from the published authorization server metadata, so an\n  agent cannot discover the platform scope vocabulary without documentation.\n- >-\n  Application OAuth2 clients are declared with redirectURIs and grantTypes in\n  `defineAuth()`; the docs show no scope parameter, so per-application authorization is\n  expressed through roles and attributes rather than OAuth scopes.\nx-evidence:\n  fetched: '2026-08-29'\n  probes:\n  - url: https://api.tailor.tech/.well-known/oauth-authorization-server\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tailor/refs/heads/main/scopes/tailor-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- ERP
- Headless ERP
- Retail
- E-Commerce
- Supply Chain
- Inventory Management
- GraphQL
- gRPC
- Low-Code
- Composable Commerce
- Manufacturing
token_urls: []
---
