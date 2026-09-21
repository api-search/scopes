---
authorization_urls: []
description: ''
docs: https://augworlds.ai/mcp
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Augworlds Ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Travel World uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Travel World
provider_slug: augworlds-ai
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: augworlds-ai-scopes
source_filename: augworlds-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: https://travel.augworlds.ai/.well-known/oauth-authorization-server\ndocs: https://augworlds.ai/mcp\ncorroborating_source: https://travel.augworlds.ai/.well-known/oauth-protected-resource/mcp\nsummary: >-\n  Travel World publishes no OpenAPI, so derive-oauth-scopes.py has nothing to read; this artifact was\n  PROBED from the RFC 8414 authorization-server metadata and the RFC 9728 protected-resource metadata\n  the provider serves on travel.augworlds.ai. Both documents list the same six scopes. The scopes are\n  MCP-resource scopes (mcp:* prefix) for the single protected resource https://travel.augworlds.ai/mcp;\n  no OIDC scopes (openid/profile/email) are advertised and no scopes are attached to the A2A bearer scheme.\nmodel: >-\n  Resource-family scopes with a read/write verb suffix. The provider publishes names only — no\n  per-scope descriptions exist on any public page, so the descriptions below are limited to what the\n \
  \ name itself states and are marked as such.\nauthorization_server:\n  issuer: https://travel.augworlds.ai\n  metadata_url: https://travel.augworlds.ai/.well-known/oauth-authorization-server\n  http_status: 200\n  authorization_endpoint: https://travel.augworlds.ai/api/oauth/authorize\n  token_endpoint: https://travel.augworlds.ai/api/oauth/token\n  registration_endpoint: https://travel.augworlds.ai/api/oauth/register\n  revocation_endpoint: https://travel.augworlds.ai/api/oauth/revoke\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  response_types_supported:\n  - code\n  code_challenge_methods_supported:\n  - S256\n  token_endpoint_auth_methods_supported:\n  - none\n  resource_indicators_supported: true\n  authorization_response_iss_parameter_supported: true\nprotected_resource:\n  resource: https://travel.augworlds.ai/mcp\n  metadata_url: https://travel.augworlds.ai/.well-known/oauth-protected-resource/mcp\n  http_status: 200\n  bearer_methods_supported:\n  - header\n\
  \  resource_documentation: https://augworlds.ai/mcp\nscope_count: 6\nscopes:\n- name: mcp:tools:list\n  family: tools\n  access: list\n  description: Enumerate the MCP server's tools (the MCP tools/list method). Name-derived; the provider publishes no description.\n- name: mcp:tk:read\n  family: tk\n  access: read\n  description: Read access to the \"tk\" resource family. The provider does not expand the abbreviation anywhere public; it is not guessed here.\n- name: mcp:brandlanes:read\n  family: brandlanes\n  access: read\n  description: Read access to the \"brandlanes\" resource family. Name-derived; likely the direct-from-travel-partner offers the site markets as \"buy direct — no middleman\", but the provider does not say so.\n- name: mcp:search:read\n  family: search\n  access: read\n  description: Read access to search — the flight and hotel search the public docs describe. Name-derived.\n- name: mcp:profile:apply\n  family: profile\n  access: apply\n  description: Apply the member's\
  \ saved profile (loyalty programs and travel preferences, per the public docs) to results. Name-derived; a write-shaped verb.\n- name: mcp:observations:write\n  family: observations\n  access: write\n  description: Write access to the \"observations\" resource family. Name-derived; the provider publishes no description.\nnotes:\n- The A2A agent card's bearer scheme carries an empty scope list; the OAuth scopes above apply to the MCP resource only.\n- token_endpoint_auth_methods_supported is [none], so every registered client is a public client relying on PKCE.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/augworlds-ai/refs/heads/main/scopes/augworlds-ai-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Travel
- Flights
- Hotels
- Travel Agent
- MCP
- A2A
- AI Agents
- Authentication
- Marketplace
token_urls: []
---
