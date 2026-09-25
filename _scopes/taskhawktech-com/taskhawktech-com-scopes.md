---
api_specs:
- filename: taskhawktech-com-openapi.yml
  format: yaml
  label: Kevros Governance API
  slug: kevros-governance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taskhawktech-com/refs/heads/main/openapi/taskhawktech-com-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Taskhawktech Com Scopes
name_suffix: OAuth Scopes
note: The OpenAPI declares ONLY an apiKey scheme (X-API-Key), so derive-oauth-scopes.py found nothing to derive. These scopes come from the provider's published authorization-server metadata. No scopes reference page exists; descriptions below are limited to what the scope name plus the matching REST operation make evident, and are marked accordingly. The scopes are NOT referenced by any operation's security requirement in the contract.
overview: 'TaskHawk Systems uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: TaskHawk Systems
provider_slug: taskhawktech-com
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: taskhawktech-com-scopes
source_filename: taskhawktech-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://governance.taskhawktech.com/.well-known/oauth-authorization-server (RFC 8414 metadata, fetched 2026-09-19;\n  saved as well-known/taskhawktech-com-oauth-authorization-server.json)\ndocs: null\nnote: The OpenAPI declares ONLY an apiKey scheme (X-API-Key), so derive-oauth-scopes.py found nothing to derive.\n  These scopes come from the provider's published authorization-server metadata. No scopes reference page exists;\n  descriptions below are limited to what the scope name plus the matching REST operation make evident, and are marked\n  accordingly. The scopes are NOT referenced by any operation's security requirement in the contract.\nauthorization_server:\n  issuer: https://governance.taskhawktech.com\n  authorization_endpoint: https://governance.taskhawktech.com/oauth/authorize\n  token_endpoint: https://governance.taskhawktech.com/oauth/token\n  jwks_uri: https://governance.taskhawktech.com/.well-known/jwks.json\n\
  \  grant_types:\n  - authorization_code\n  - client_credentials\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  response_types:\n  - code\n  - token\n  token_endpoint_auth_methods:\n  - client_secret_post\n  signing_alg:\n  - ES256\nscopes:\n- name: governance:verify\n  description: Action verification — matches operation verify-action (POST /governance/verify).\n  operations:\n  - verify-action\n  confidence: medium (name match; not bound in the OpenAPI)\n- name: governance:attest\n  description: Provenance attestation — matches attest-action (POST /governance/attest).\n  operations:\n  - attest-action\n  confidence: medium\n- name: governance:bind\n  description: Intent binding — matches bind-intent (POST /governance/bind).\n  operations:\n  - bind-intent\n  confidence: medium\n- name: governance:entitlements\n  description: null\n  operations: []\n  confidence: low — no public operation; likely plan/entitlement lookup\n- name: governance:scim\n  description: null\n  operations:\
  \ []\n  confidence: low — implies a SCIM provisioning surface; no /scim path is published or probed\n- name: governance:logout\n  description: null\n  operations: []\n  confidence: low\n- name: governance:gtr\n  description: null\n  operations: []\n  confidence: low — acronym not expanded anywhere public\nscope_count: 7\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taskhawktech-com/refs/heads/main/scopes/taskhawktech-com-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- AI Governance
- Agent Security
- Runtime Enforcement
- Policy Enforcement
- Provenance
- Compliance
- Prompt Injection Detection
- Media Attestation
- Post-Quantum Cryptography
- Formal Verification
- x402
- L402
- Machine Payments
- MCP
- A2A
- Agent-Native
- Government
- Defense
token_urls: []
---
