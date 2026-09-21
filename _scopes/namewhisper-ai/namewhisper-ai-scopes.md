---
authorization_urls:
- https://namewhisper.ai/oauth/authorize
description: Scopes published in the provider's RFC 8414 authorization-server metadata and repeated in the RFC 9728 protected-resource metadata for https://namewhisper.ai/mcp. There is no OpenAPI to derive from (derive-oauth-scopes.py found no oauth2 scheme), so this file is read from the metadata documents. The scopes are declared but no document explains which tools each scope covers; the natural reading - from the server card's free/transaction split - is that mcp.read maps to the 19 FREE read tools and mcp.transact to the 25 TRANSACTION tools, but that mapping is an inference and is labelled as such below.
docs: https://namewhisper.ai/auth.md
flows:
- erc8128_signed_request
kind: oauth-scopes
layout: scope
method: searched
name: Namewhisper Ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'NameWhisper publishes 2 OAuth 2.0 scopes via the erc8128_signed_request flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the NameWhisper API on a user''s behalf.


  Tokens are issued from https://namewhisper.ai/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: NameWhisper
provider_slug: namewhisper-ai
schemes:
- flows:
  - authorizationUrl: https://namewhisper.ai/oauth/authorize
    flow: erc8128_signed_request
    note: Non-standard grant type; no bearer tokens are issued, identity rides on each signed request.
    tokenUrl: https://namewhisper.ai/oauth/token
  issuer: https://namewhisper.ai
  name: namewhisper-authorization-server
  source: well-known/namewhisper-ai-oauth-authorization-server.json
scope_count: 2
scope_names:
- mcp.read
- mcp.transact
scopes:
- description: Declared in scopes_supported; no published definition.
  flows:
  - erc8128_signed_request
  scope: mcp.read
- description: Declared in scopes_supported; no published definition.
  flows:
  - erc8128_signed_request
  scope: mcp.transact
slug: namewhisper-ai-scopes
source_filename: namewhisper-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://namewhisper.ai/.well-known/oauth-authorization-server\ndocs: https://namewhisper.ai/auth.md\ndescription: >-\n  Scopes published in the provider's RFC 8414 authorization-server metadata and repeated in the RFC 9728\n  protected-resource metadata for https://namewhisper.ai/mcp. There is no OpenAPI to derive from\n  (derive-oauth-scopes.py found no oauth2 scheme), so this file is read from the metadata documents. The scopes\n  are declared but no document explains which tools each scope covers; the natural reading - from the server\n  card's free/transaction split - is that mcp.read maps to the 19 FREE read tools and mcp.transact to the 25\n  TRANSACTION tools, but that mapping is an inference and is labelled as such below.\nschemes:\n- name: namewhisper-authorization-server\n  source: well-known/namewhisper-ai-oauth-authorization-server.json\n  issuer: https://namewhisper.ai\n  flows:\n  - flow: erc8128_signed_request\n\
  \    authorizationUrl: https://namewhisper.ai/oauth/authorize\n    tokenUrl: https://namewhisper.ai/oauth/token\n    note: Non-standard grant type; no bearer tokens are issued, identity rides on each signed request.\nscopes:\n- scope: mcp.read\n  description: Declared in scopes_supported; no published definition.\n  inferred_coverage: the 19 FREE / read-only tools (inference from the server card, not a provider statement)\n  flows: [erc8128_signed_request]\n  sources: [well-known/namewhisper-ai-oauth-authorization-server.json, well-known/namewhisper-ai-oauth-protected-resource.json]\n- scope: mcp.transact\n  description: Declared in scopes_supported; no published definition.\n  inferred_coverage: the 25 TRANSACTION tools that build unsigned calldata (inference, not a provider statement)\n  flows: [erc8128_signed_request]\n  sources: [well-known/namewhisper-ai-oauth-authorization-server.json, well-known/namewhisper-ai-oauth-protected-resource.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/namewhisper-ai/refs/heads/main/scopes/namewhisper-ai-scopes.yml
summary_line: 2 scopes · erc8128_signed_request
tags:
- ENS
- Ethereum
- Web3
- Domain Names
- AI Agents
- MCP
- A2A
- Valuation
- NFT Marketplace
- Agent Identity
- Blockchain
token_urls:
- https://namewhisper.ai/oauth/token
---
