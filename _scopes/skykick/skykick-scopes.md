---
authorization_urls: []
description: ''
docs: https://skykick.developer.azure-api.net/getstarted
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Skykick Scopes
name_suffix: OAuth Scopes
note: 'These are the only scope values SkyKick publishes anonymously. The Get Started page states them verbatim as "Valid scopes: Partner, Distributor" in the body of the token request. There is no OpenAPI oauth2 securityScheme to derive a fuller list from, and no published scopes/permissions reference page, so this artifact records exactly the two values the provider documents and nothing more. Per-scope operation mapping requires authenticated access to the gated API reference.'
overview: 'SkyKick uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SkyKick
provider_slug: skykick
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: skykick-scopes
source_filename: skykick-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: searched\nsource: https://skykick.developer.azure-api.net/getstarted\ndocs: https://skykick.developer.azure-api.net/getstarted\napi: SkyKick Partner Integration API\nflow: clientCredentials\ntoken_url: https://apis.cloudservices.connectwise.com/auth/token\nnote: >-\n  These are the only scope values SkyKick publishes anonymously. The Get Started\n  page states them verbatim as \"Valid scopes: Partner, Distributor\" in the body of\n  the token request. There is no OpenAPI oauth2 securityScheme to derive a fuller\n  list from, and no published scopes/permissions reference page, so this artifact\n  records exactly the two values the provider documents and nothing more. Per-scope\n  operation mapping requires authenticated access to the gated API reference.\nscope_count: 2\nscopes:\n- name: Partner\n  description: >-\n    Requested by an MSP partner tenant calling the Partner Integration API on its\n    own behalf. Named as the example value in\
  \ the provider's sample token request.\n  evidence: 'grant_type=client_credentials&scope=Partner'\n- name: Distributor\n  description: >-\n    Requested by a distributor tenant. Listed by the provider alongside Partner as\n    a valid scope value; the provider publishes no further description of what it\n    grants.\n  evidence: 'Valid scopes: Partner, Distributor'\ngaps:\n- No published scope-to-operation mapping.\n- No published reference page enumerating fine-grained permissions.\n- No /.well-known/oauth-authorization-server document (probed 2026-08-28, HTTP 404).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skykick/refs/heads/main/scopes/skykick-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Backup
- Migration
- Microsoft-365
- Managed Service Providers
- SaaS Security
- Cloud Automation
- Data Protection
- Azure API Management
token_urls: []
---
