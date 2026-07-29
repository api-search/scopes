---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: derived
name: Hydro One Scopes
name_suffix: OAuth Scopes
note: Hydro One publishes no scope reference. This artifact records the NAESB ESPI function-block scope syntax observed on a live Green Button Connect My Data authorization request against Hydro One's authorization surface (recorded in review.yml during the 2026-07-27 review of a publicly indexed instance of https://www.hydroone.com/green-button-cmd-home). The individual function-block identifiers are defined by the NAESB REQ.21 ESPI standard, not by Hydro One, and Hydro One publishes no mapping of block id to meaning — so no per-block descriptions are asserted here. Values are recorded verbatim, unexpanded.
overview: 'Hydro One uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hydro One
provider_slug: hydro-one
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: hydro-one-scopes
source_filename: hydro-one-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: derived\nsource: review.yml\nnote: >-\n  Hydro One publishes no scope reference. This artifact records the NAESB ESPI\n  function-block scope syntax observed on a live Green Button Connect My Data\n  authorization request against Hydro One's authorization surface (recorded in\n  review.yml during the 2026-07-27 review of a publicly indexed instance of\n  https://www.hydroone.com/green-button-cmd-home). The individual function-block\n  identifiers are defined by the NAESB REQ.21 ESPI standard, not by Hydro One,\n  and Hydro One publishes no mapping of block id to meaning — so no per-block\n  descriptions are asserted here. Values are recorded verbatim, unexpanded.\nscheme: green-button-cmd-oauth2\nscope_model: naesb-espi-function-blocks\nsyntax: 'FB=<function block ids separated by underscores>;historyLength=<seconds>'\nstandard:\n  name: NAESB REQ.21 Energy Services Provider Interface (ESPI)\n  version_required_in_ontario: '3.3'\n  reference:\
  \ https://www.greenbuttonalliance.org/\n  developer_guide: https://greenbuttonalliance.github.io/OpenESPI-GreenButton-API-Documentation/\nobserved_scope:\n  raw: 'FB=1_3_4_5_13_15_16_31_37_39_51_53_54_55_56_57_58_59_60_64_65;historyLength=32148000'\n  function_blocks:\n  - '1'\n  - '3'\n  - '4'\n  - '5'\n  - '13'\n  - '15'\n  - '16'\n  - '31'\n  - '37'\n  - '39'\n  - '51'\n  - '53'\n  - '54'\n  - '55'\n  - '56'\n  - '57'\n  - '58'\n  - '59'\n  - '60'\n  - '64'\n  - '65'\n  history_length_seconds: 32148000\n  observed_on: '2026-07-27'\n  observed_at: https://www.hydroone.com/green-button-cmd-home\n  confidence: medium\n  confidence_note: >-\n    Single observation of one onboarded third party's authorization request. It\n    evidences the scope syntax Hydro One accepts; it is not a published list of\n    the scopes Hydro One grants, and other vendors may be issued different\n    function-block sets.\nscopes: []\nscopes_note: >-\n  No enumerated, documented scope list exists on any Hydro\
  \ One surface. The\n  function-block set a vendor receives is negotiated during onboarding.\nrelated:\n- authentication/hydro-one-authentication.yml\n- conformance/hydro-one-conformance.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hydro-one/refs/heads/main/scopes/hydro-one-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Energy
- Canada
- Utilities
- Electricity
- Grid
- Smart Metering
- Green Button
- Energy Data
- Transmission
- Distribution
token_urls: []
---
