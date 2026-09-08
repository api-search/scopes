---
api_specs:
- filename: benchmark-minerals-prices-api.yml
  format: yaml
  label: Benchmark Minerals API
  slug: benchmark-minerals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benchmark-minerals/refs/heads/main/openapi/benchmark-minerals-prices-api.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Benchmark Minerals Scopes
name_suffix: OAuth Scopes
note: Benchmark runs two distinct permission vocabularies and publishes neither in prose. (1) The MCP gateway uses real OAuth 2.0 scopes, discoverable anonymously in its RFC 9728 protected-resource document. (2) The REST OpenAPI declares scope STRINGS on an apiKey security scheme — syntactically legal but semantically unusual, since an API key carries no scope grant; they read as an entitlement map describing which market a key must be subscribed to. Both sets are recorded verbatim; neither is invented.
overview: 'Benchmark Minerals uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Benchmark Minerals
provider_slug: benchmark-minerals
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: benchmark-minerals-scopes
source_filename: benchmark-minerals-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: https://mcp.benchmarkminerals.com/.well-known/oauth-protected-resource + openapi/benchmark-minerals-prices-api.yml\nprovider: Benchmark Minerals\nproviderId: benchmark-minerals\ndocs: null\nnote: Benchmark runs two distinct permission vocabularies and publishes neither in prose. (1) The MCP\n  gateway uses real OAuth 2.0 scopes, discoverable anonymously in its RFC 9728 protected-resource document.\n  (2) The REST OpenAPI declares scope STRINGS on an apiKey security scheme — syntactically legal but semantically\n  unusual, since an API key carries no scope grant; they read as an entitlement map describing which market\n  a key must be subscribed to. Both sets are recorded verbatim; neither is invented.\nscope_sets:\n- surface: MCP gateway\n  endpoint: https://mcp.benchmarkminerals.com/mcp\n  type: oauth2\n  issuer: https://cognito-idp.eu-west-2.amazonaws.com/eu-west-2_GuiZRnNNK\n  evidence: https://mcp.benchmarkminerals.com/.well-known/oauth-protected-resource\
  \ (HTTP 200) and the\n    WWW-Authenticate challenge\n  scopes:\n  - name: benchmark-tools/sandbox.read\n    description: Read access to the sandbox dataset through the MCP tool surface.\n  - name: benchmark-tools/production.read\n    description: Read access to the production dataset through the MCP tool surface.\n- surface: Prices REST API\n  endpoint: https://api.benchmarkminerals.com/v2\n  type: apiKey-declared-scopes\n  evidence: per-operation security[].api_key[] arrays in https://www.benchmarkminerals.com/prices-api.yml\n  scopes:\n  - name: anodes:read\n    operations:\n    - anode-index\n    - anode-list-prices\n    - anode-summary\n    operation_count: 3\n  - name: black-mass:read\n    operations:\n    - black-mass-index\n    - black-mass-list-prices\n    - black-mass-summary\n    operation_count: 3\n  - name: cathodes:read\n    operations:\n    - cathodes-index\n    - cathodes-list-prices\n    - cathodes-summary\n    operation_count: 3\n  - name: cobalt:read\n    operations:\n\
  \    - cobalt-index\n    - cobalt-list-prices\n    - cobalt-summary\n    operation_count: 3\n  - name: electrolyte:read\n    operations:\n    - electrolyte-list-prices\n    - electrolyte-summary\n    operation_count: 2\n  - name: lithium-ion-battery-raw-material:read\n    operations:\n    - lithium-ion-battery-raw-material-index\n    operation_count: 1\n  - name: lithium-ion-battery:read\n    operations:\n    - lithium-ion-battery-index\n    - lithium-ion-battery-list-prices\n    - lithium-ion-battery-summary\n    operation_count: 3\n  - name: lithium:read\n    operations:\n    - lithium-index\n    - lithium-list-prices\n    - lithium-summary\n    operation_count: 3\n  - name: manganese:read\n    operations:\n    - manganese-list-prices\n    - manganese-summary\n    operation_count: 2\n  - name: natural-graphite:read\n    operations:\n    - natural-graphite-index\n    - natural-graphite-list-prices\n    - natural-graphite-summary\n    operation_count: 3\n  - name: nickel:read\n    operations:\n\
  \    - nickel-index\n    - nickel-list-prices\n    - nickel-summary\n    operation_count: 3\n  - name: prices:anodes\n    operations:\n    - anode-index\n    - anode-list-prices\n    - anode-summary\n    operation_count: 3\n  - name: prices:black-mass\n    operations:\n    - black-mass-index\n    - black-mass-list-prices\n    - black-mass-summary\n    operation_count: 3\n  - name: prices:cathodes\n    operations:\n    - cathodes-list-prices\n    - cathodes-summary\n    operation_count: 2\n  - name: prices:cobalt\n    operations:\n    - cobalt-index\n    - cobalt-list-prices\n    - cobalt-summary\n    operation_count: 3\n  - name: prices:electrolyte\n    operations:\n    - electrolyte-list-prices\n    - electrolyte-summary\n    operation_count: 2\n  - name: prices:lithium\n    operations:\n    - lithium-index\n    - lithium-list-prices\n    - lithium-summary\n    operation_count: 3\n  - name: prices:lithium-ion-batteries\n    operations:\n    - lithium-ion-battery-index\n    - lithium-ion-battery-list-prices\n\
  \    - lithium-ion-battery-summary\n    operation_count: 3\n  - name: prices:manganese\n    operations:\n    - manganese-list-prices\n    - manganese-summary\n    operation_count: 2\n  - name: prices:natural-graphite\n    operations:\n    - natural-graphite-index\n    - natural-graphite-list-prices\n    - natural-graphite-summary\n    operation_count: 3\n  - name: prices:nickel\n    operations:\n    - nickel-index\n    - nickel-list-prices\n    - nickel-summary\n    operation_count: 3\n  - name: prices:rare-earths\n    operations:\n    - rare-earths-index\n    - rare-earths-list-prices\n    - rare-earths-summary\n    operation_count: 3\n  - name: prices:synthetic-graphite\n    operations:\n    - synthetic-graphite-index\n    - synthetic-graphite-list-prices\n    - synthetic-graphite-summary\n    operation_count: 3\n  - name: rare-earths:read\n    operations:\n    - rare-earths-index\n    - rare-earths-list-prices\n    - rare-earths-summary\n    operation_count: 3\n  - name: spotlight:read\n\
  \    operations:\n    - spotlight-list-prices\n    operation_count: 1\n  - name: synthetic-graphite:read\n    operations:\n    - synthetic-graphite-index\n    - synthetic-graphite-list-prices\n    - synthetic-graphite-summary\n    operation_count: 3\nsummary:\n  oauth_scopes: 2\n  spec_declared_scopes: 26\n  pattern: two per market — <market>:read and prices:<market> — all read-only; no write scope exists anywhere\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/benchmark-minerals/refs/heads/main/scopes/benchmark-minerals-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Batteries
- Cobalt
- Critical Minerals
- Electric Vehicles
- Energy Transition
- Graphite
- Lithium
- Lithium-Ion
- Market Intelligence
- Mining
- Nickel
- Price Reporting
- Rare Earths
- Supply Chain
token_urls: []
---
