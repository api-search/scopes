---
authorization_urls:
- https://influencermarketing.ai/wp-admin/admin.php?page=novamira-oauth-authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Stagwell Scopes
name_suffix: OAuth Scopes
note: No OpenAPI is published anywhere in this profile, so derive-oauth-scopes.py has no spec to read. The scope surface recorded here comes straight from the anonymous RFC 8414 authorization-server metadata and the RFC 9728 protected-resource metadata served by influencermarketing.ai (IMAI, a Stagwell company). Exactly one scope is advertised. The IMAI Discovery and Raw product APIs use an API key, not OAuth, and therefore have no scope surface at all.
overview: 'Stagwell uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://influencermarketing.ai/wp-json/novamira/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Stagwell
provider_slug: stagwell
schemes:
- flows:
  - authorizationUrl: https://influencermarketing.ai/wp-admin/admin.php?page=novamira-oauth-authorize
    code_challenge_methods_supported:
    - S256
    flow: authorizationCode
    tokenUrl: https://influencermarketing.ai/wp-json/novamira/v1/oauth/token
  issuer: https://influencermarketing.ai
  name: novamira-oauth
  source: https://influencermarketing.ai/.well-known/oauth-authorization-server
scope_count: 0
scope_names: []
scopes: []
slug: stagwell-scopes
source_filename: stagwell-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://influencermarketing.ai/.well-known/oauth-authorization-server\nnote: >-\n  No OpenAPI is published anywhere in this profile, so derive-oauth-scopes.py has\n  no spec to read. The scope surface recorded here comes straight from the\n  anonymous RFC 8414 authorization-server metadata and the RFC 9728\n  protected-resource metadata served by influencermarketing.ai (IMAI, a Stagwell\n  company). Exactly one scope is advertised. The IMAI Discovery and Raw product\n  APIs use an API key, not OAuth, and therefore have no scope surface at all.\nschemes:\n  - name: novamira-oauth\n    issuer: https://influencermarketing.ai\n    source: https://influencermarketing.ai/.well-known/oauth-authorization-server\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://influencermarketing.ai/wp-admin/admin.php?page=novamira-oauth-authorize\n        tokenUrl: https://influencermarketing.ai/wp-json/novamira/v1/oauth/token\n\
  \        code_challenge_methods_supported: [S256]\nscopes:\n  - name: mcp\n    description: >-\n      Access the Model Context Protocol server at\n      https://influencermarketing.ai/wp-json/mcp/novamira-oauth. The provider\n      publishes no per-tool or finer-grained scope decomposition; \"mcp\" is the\n      only value in scopes_supported on both the authorization-server and the\n      protected-resource metadata.\n    source: /.well-known/oauth-authorization-server\n    applies_to: https://influencermarketing.ai/wp-json/mcp/novamira-oauth\nscope_count: 1\nx-evidence:\n  fetched: '2026-08-12'\n  probes:\n    - url: https://influencermarketing.ai/.well-known/oauth-authorization-server\n      status: 200\n    - url: https://influencermarketing.ai/.well-known/oauth-protected-resource\n      status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stagwell/refs/heads/main/scopes/stagwell-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Marketing
- Advertising
- Media
- MarTech
- Influencer Marketing
- Market Research
- Creator Economy
- Public Relations
- Consumer Insights
- Holding Company
token_urls:
- https://influencermarketing.ai/wp-json/novamira/v1/oauth/token
---
