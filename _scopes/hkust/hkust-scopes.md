---
api_specs:
- filename: hkust-path-advisor-openapi.yml
  format: yaml
  label: HKUST Path Advisor API
  slug: path-advisor
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hkust/refs/heads/main/openapi/hkust-path-advisor-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Hkust Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Hong Kong University of Science and Technology uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hong Kong University of Science and Technology
provider_slug: hkust
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: hkust-scopes
source_filename: hkust-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "name: Hong Kong University of Science and Technology — authorization scopes\nprovider: Hong Kong University of Science and Technology\nproviderId: hkust\ngenerated: '2026-08-30'\nmethod: probed\nsource: >-\n  Live probes on 2026-08-30 across every HKUST API surface found. This file records an\n  ABSENCE that was checked for, not a scope catalog that exists.\nsummary: >-\n  HKUST publishes no scope vocabulary on any surface. There is no OAuth 2.0 or OpenID\n  Connect authorization server on any HKUST host probed, and therefore no scope strings to\n  catalog. Authorization on the surfaces that have any is coarse-grained and binary.\nsurfaces:\n  - surface: HKUST Path Advisor API\n    x-operator: institution\n    scopes: []\n    model: >-\n      None. Public routes are unauthenticated and unscoped; /connectors is a single\n      all-or-nothing gate returning 401 with no scheme advertised.\n  - surface: HKUST API Gateway (Azure API Management)\n    x-operator: tenant\n    scopes:\
  \ []\n    model: >-\n      Azure API Management Products, not scopes. Authorization granularity is the Product a\n      subscription key is approved against — HKUST names \"IoT Sensor Data\" and \"Sensor\n      Inventory\" — and the Product catalog is not enumerable without signing in, so the\n      full list cannot be verified from outside. A Product is closer to a plan than a scope\n      and carries no scope string a client can request.\n  - surface: HKUST Shibboleth Identity Provider\n    x-operator: institution\n    scopes: []\n    model: >-\n      SAML attribute release, not OAuth scopes. The federation-level equivalent is the\n      REFEDS Research & Scholarship entity category, which HKUST's IdP carries — that\n      governs which attribute bundle is released to a service provider. Per-service\n      attribute release policy is not published.\n    entityCategories:\n      - http://refeds.org/category/research-and-scholarship\n      - https://refeds.org/sirtfi\nmaintainers:\n  -\
  \ FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hkust/refs/heads/main/scopes/hkust-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- Research
- Hong Kong
- China
- Research Data
- Open Data
- Identity Federation
- Course Catalog
- Library
- Smart Campus
- API Gateway
- Wayfinding
token_urls: []
---
