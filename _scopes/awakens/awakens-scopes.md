---
authorization_urls:
- https://genomelink.io/oauth/authorize
description: ''
docs: https://genomelink.io/developers/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Awakens Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'AWAKENS uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://genomelink.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AWAKENS
provider_slug: awakens
schemes:
- flows:
  - authorizationUrl: https://genomelink.io/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://genomelink.io/oauth/token
  name: oauth2
  source: https://github.com/genomelink/genomelink-python/blob/master/genomelink/oauth.py
scope_count: 0
scope_names: []
scopes: []
slug: awakens-scopes
source_filename: awakens-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: https://github.com/genomelink/genomelink-python\ndocs: https://genomelink.io/developers/\nschemes:\n- name: oauth2\n  source: https://github.com/genomelink/genomelink-python/blob/master/genomelink/oauth.py\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://genomelink.io/oauth/authorize\n    tokenUrl: https://genomelink.io/oauth/token\nscopes: []\nnotes: >-\n  The OAuth authorization-code flow accepts a `scope` parameter (passed through\n  the SDK authorize_url / authorizeUrl helpers), and access is granted per\n  genetic-trait report requested by the consenting user (reports are addressed\n  by trait name, e.g. eye-color, and population). AWAKENS does not publish an\n  enumerated scope reference on the developers page, so no specific scope\n  strings are asserted here to avoid fabrication. scopes[] is intentionally\n  empty pending a published permissions reference.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/awakens/refs/heads/main/scopes/awakens-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Genomics
- DNA
- Bioinformatics
- Health
- Consumer Genetics
- Ancestry
- OAuth
- Personal Genomics
token_urls:
- https://genomelink.io/oauth/token
---
