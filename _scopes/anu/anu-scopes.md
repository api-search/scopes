---
api_specs:
- filename: anu-quantum-numbers-openapi.yml
  format: yaml
  label: ANU Quantum Numbers (AQN) API
  slug: quantum-numbers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anu/refs/heads/main/openapi/anu-quantum-numbers-openapi.yml
- filename: anu-qrng-legacy-openapi.yml
  format: yaml
  label: QRNG@ANU Legacy JSON API
  slug: qrng-legacy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anu/refs/heads/main/openapi/anu-qrng-legacy-openapi.yml
- filename: anu-open-research-oai-pmh-openapi.yml
  format: yaml
  label: ANU Open Research OAI-PMH
  slug: openresearch-oai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anu/refs/heads/main/openapi/anu-open-research-oai-pmh-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Anu Scopes
name_suffix: OAuth Scopes
note: 'ANU exposes NO scoped authorization on any institution-operated API surface. This file records that absence with the probes that established it, rather than being omitted — an absent scopes file reads as "not looked at", and this was looked at. The AQN API is a single-key, single-operation service: one static x-api-key grants the one GET it offers, with no scope parameter, no consent screen and no partial grant. The legacy QRNG endpoint and the OAI-PMH endpoint are unauthenticated. The only OAuth2 token endpoint anywhere on an ANU host is the LTI 1.3 platform token endpoint inside Moodle (https://wattlecourses.anu.edu.au/mod/lti/token.php), which issues tokens against IMS Global LTI Advantage service scopes to registered LTI tools — not to outside developers, and not through any public client-registration path.'
overview: 'Australian National University uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Australian National University
provider_slug: anu
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: anu-scopes
source_filename: anu-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: https://api.quantumnumbers.anu.edu.au\nx-operator: institution\nnote: >-\n  ANU exposes NO scoped authorization on any institution-operated API surface. This file\n  records that absence with the probes that established it, rather than being omitted — an\n  absent scopes file reads as \"not looked at\", and this was looked at.\n\n\n  The AQN API is a single-key, single-operation service: one static x-api-key grants the one\n  GET it offers, with no scope parameter, no consent screen and no partial grant. The legacy\n  QRNG endpoint and the OAI-PMH endpoint are unauthenticated. The only OAuth2 token endpoint\n  anywhere on an ANU host is the LTI 1.3 platform token endpoint inside Moodle\n  (https://wattlecourses.anu.edu.au/mod/lti/token.php), which issues tokens against\n  IMS Global LTI Advantage service scopes to registered LTI tools — not to outside developers,\n  and not through any public client-registration path.\nschemes:\
  \ []\nscopes: []\nnegative_probes:\n- url: https://api.quantumnumbers.anu.edu.au/\n  status: 403\n  finding: '{\"message\":\"Forbidden\"} — gateway key check only; no OAuth challenge, no WWW-Authenticate scope hint.'\n- url: https://www.anu.edu.au/.well-known/openid-configuration\n  status: 404\n  finding: No OIDC discovery document on the institutional domain.\n- url: https://wattlecourses.anu.edu.au/.well-known/openid-configuration\n  status: 404\n  finding: No OIDC discovery document on the LMS host either; the LTI endpoints are not advertised via .well-known.\n- url: https://developer.anu.edu.au/\n  status: 000\n  finding: Host does not resolve. No developer portal exists at the conventional address.\n- url: https://api.anu.edu.au/\n  status: 000\n  finding: Host does not resolve. There is no central institutional API gateway.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anu/refs/heads/main/scopes/anu-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- Research
- Australia
- Group of Eight
- Research Repository
- Identity Federation
- Open Access
- Quantum
- Random Numbers
- OAI-PMH
token_urls: []
---
