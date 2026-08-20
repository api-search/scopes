---
authorization_urls: []
description: ''
docs: https://docs.getbluma.com/authentication
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Bluma Scopes
name_suffix: OAuth Scopes
note: Bluma publishes two disjoint scope vocabularies. The REST API keys carry eight product scopes, granted as a default set on every new key. The MCP server's OAuth tokens carry Clerk identity scopes instead, and nothing published maps one onto the other. Neither vocabulary is derivable from a spec — the advertised OpenAPI at https://api.getbluma.com/api/v1/openapi.json returns 401 — so both lists are read verbatim from Bluma's own documentation and from live anonymous OAuth metadata.
overview: 'Bluma uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bluma
provider_slug: bluma
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: bluma-scopes
source_filename: bluma-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://docs.getbluma.com/authentication\ndocs: https://docs.getbluma.com/authentication\nnote: >-\n  Bluma publishes two disjoint scope vocabularies. The REST API keys carry eight\n  product scopes, granted as a default set on every new key. The MCP server's OAuth\n  tokens carry Clerk identity scopes instead, and nothing published maps one onto the\n  other. Neither vocabulary is derivable from a spec — the advertised OpenAPI at\n  https://api.getbluma.com/api/v1/openapi.json returns 401 — so both lists are read\n  verbatim from Bluma's own documentation and from live anonymous OAuth metadata.\napi_key_scopes:\n  model: API key scopes (not OAuth)\n  granted: default set on every key created through the dashboard or API\n  custom_scopes: Enterprise plans only, by request to support@getbluma.com\n  scopes:\n  - name: videos:create\n    description: Generate new videos\n  - name: videos:read\n    description: View video status\
  \ and details\n  - name: videos:download\n    description: Download generated videos\n  - name: templates:list\n    description: Browse available templates\n  - name: templates:read\n    description: View template details\n  - name: credits:read\n    description: Check credit balance and history\n  - name: webhooks:manage\n    description: Create and manage webhooks\n  - name: usage:read\n    description: View usage analytics\n  enforcement:\n    status: 403\n    type: permission_denied\n    response_metadata:\n    - required_scope\n    - available_scopes\noauth_scopes:\n  model: OAuth 2.1 / OpenID Connect (Clerk)\n  applies_to: https://api.getbluma.com/api/mcp\n  advertised_by_resource:\n    source: https://api.getbluma.com/.well-known/oauth-protected-resource\n    scopes:\n    - name: email\n      description: Access the authenticated user's email address\n    - name: profile\n      description: Access the authenticated user's basic profile\n    - name: offline_access\n      description:\
  \ Issue a refresh token for long-lived agent sessions\n  supported_by_authorization_server:\n    source: https://clerk.getbluma.com/.well-known/oauth-authorization-server\n    scopes:\n    - name: openid\n      description: OpenID Connect authentication\n    - name: profile\n      description: Basic profile claims\n    - name: email\n      description: Email claim\n    - name: public_metadata\n      description: Clerk public user metadata\n    - name: private_metadata\n      description: Clerk private user metadata\n    - name: offline_access\n      description: Refresh token issuance\n  service_documentation: https://clerk.com/docs/oauth/scoped-access\nsummary:\n  api_key_scope_count: 8\n  oauth_scope_count: 3\n  oauth_scope_count_supported_by_as: 6\n  scopes_mapped_across_models: false\ngaps:\n- The OAuth vocabulary is identity-only. No published scope expresses authority over\n  Bluma resources (videos, templates, credits) for an MCP-authenticated agent, so the\n  blast radius of an\
  \ MCP token is not stated.\n- API key scopes are granted as a fixed default set; the docs describe no self-service\n  way to issue a reduced-scope key outside Enterprise, so least-privilege is not\n  available to Free/Starter/Pro customers.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bluma/refs/heads/main/scopes/bluma-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Artificial Intelligence
- Video
- Video Generation
- Advertising
- Marketing
- Content Creation
- Short-Form Video
- Social-Media
- Generative AI
- Creative Tools
- Text-to-Speech
- Media
- Automation
- Webhook
token_urls: []
---
