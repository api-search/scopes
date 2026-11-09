---
authorization_urls: []
description: ''
docs: https://rslstandard.org/rsl
flows: []
kind: oauth-scopes
layout: scope
method: none
name: Rslcollective Org Scopes
name_suffix: OAuth Scopes
note: 'OLP is documented as an OAuth 2.0 extension (client_credentials grant), but the /token request defines no `scope` parameter: the granted rights are expressed by the RSL <license> XML element sent in the request (permits/prohibits usage such as search, ai-train, ai-input). The only scope-like term in the spec is the /key error `insufficient_scope` ("The license does not permit access to the encryption key for this resource."). No OAuth scope list is published.'
overview: 'RSL Collective uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: RSL Collective
provider_slug: rslcollective-org
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: rslcollective-org-scopes
source_filename: rslcollective-org-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: none\nsource: https://rslstandard.org/rsl\ndocs: https://rslstandard.org/rsl\nscopes: []\nnote: >-\n  OLP is documented as an OAuth 2.0 extension (client_credentials grant), but the /token request defines no\n  `scope` parameter: the granted rights are expressed by the RSL <license> XML element sent in the request\n  (permits/prohibits usage such as search, ai-train, ai-input). The only scope-like term in the spec is the\n  /key error `insufficient_scope` (\"The license does not permit access to the encryption key for this\n  resource.\"). No OAuth scope list is published.\n"
source_yaml_url: https://artifacts.apis.io/rslcollective-org/scopes/rslcollective-org-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- AI Licensing
- Content Licensing
- Collective Rights
- Publishers
- Royalties
- Non-Profit
- RSL Standard
token_bound: false
token_urls: []
---
