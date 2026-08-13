---
authorization_urls: []
description: ''
docs: https://dev.zemanta.com/one/api/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Zemanta Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Zemanta uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Zemanta
provider_slug: zemanta
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: zemanta-scopes
source_filename: zemanta-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://dev.zemanta.com/one/api/\ndocs: https://dev.zemanta.com/one/api/\napi: zemanta:teads-dsp-api\nauthorization_server: https://oneapi.zemanta.com/o/token/\nflow: clientCredentials\nscope_model: coarse\nscope_count: 2\nscopes:\n- name: read\n  description: >-\n    Read access to the Teads DSP campaign-management resources (accounts, credits,\n    campaigns, budgets, goals, ad groups, ads, creatives, audiences, publisher groups,\n    deals, keyword lists, reports and statistics).\n  source: token response\n- name: write\n  description: >-\n    Create and update access to the same campaign-management resources, including\n    POST/PUT/DELETE on campaigns, ad groups, ads, creatives, bid modifiers, deals\n    and keyword lists.\n  source: token response\nevidence: >-\n  The documented token response for POST https://oneapi.zemanta.com/o/token/ is\n  {\"access_token\": \"...\", \"token_type\": \"Bearer\", \"expires_in\": 36000,\
  \ \"scope\": \"read write\"}.\n  The docs publish no per-resource scope reference page; \"read write\" is granted to the\n  application as a whole.\nnotes:\n- >-\n  There is no published scopes/permissions reference beyond the read/write pair returned\n  in the token response — the API does not document per-resource or per-operation scopes.\n- >-\n  No /.well-known/oauth-authorization-server document is served, so the scope list could\n  not be confirmed from a discovery document (see well-known/zemanta-well-known.yml).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zemanta/refs/heads/main/scopes/zemanta-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Advertising
- Native Advertising
- Programmatic
- DSP
- AdTech
- Content Recommendation
- Marketing
- Campaign Management
- Demand Side Platform
- Media Buying
token_urls: []
---
