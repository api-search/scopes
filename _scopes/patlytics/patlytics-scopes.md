---
authorization_urls:
- https://mcp.patlytics.ai/authorize
description: ''
docs: https://mcp.patlytics.ai/docs
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Patlytics Scopes
name_suffix: OAuth Scopes
note: Scopes are taken verbatim from the live RFC 8414 authorization-server metadata and the RFC 9728 protected-resource metadata on the MCP host. Patlytics publishes no OpenAPI and no separate scopes/permissions reference page, so descriptions below are the pipeline's plain reading of the scope names against the published read-only tool surface, not provider copy.
overview: 'Patlytics publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Patlytics API on a user''s behalf.


  Tokens are issued from https://mcp.patlytics.ai/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Patlytics
provider_slug: patlytics
schemes:
- flows:
  - authorizationUrl: https://mcp.patlytics.ai/authorize
    flow: authorizationCode
    tokenUrl: https://mcp.patlytics.ai/token
  issuer: https://mcp.patlytics.ai/
  name: PatlyticsOAuth
  source: well-known/patlytics-oauth-authorization-server.json
scope_count: 2
scope_names:
- patent:search
- patent:read
scopes:
- description: Run semantic searches — concept-level similarity search over patent claims and search of non-patent literature (papers, journals, books via OpenAlex).
  flows:
  - authorizationCode
  scope: patent:search
- description: Read patent records — bibliographic data and claims by publication number — and list the organization's private Patlytics portfolios and vault patents.
  flows:
  - authorizationCode
  scope: patent:read
slug: patlytics-scopes
source_filename: patlytics-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://mcp.patlytics.ai/.well-known/oauth-authorization-server\ndocs: https://mcp.patlytics.ai/docs\nnote: >-\n  Scopes are taken verbatim from the live RFC 8414 authorization-server metadata and the\n  RFC 9728 protected-resource metadata on the MCP host. Patlytics publishes no OpenAPI and no\n  separate scopes/permissions reference page, so descriptions below are the pipeline's plain\n  reading of the scope names against the published read-only tool surface, not provider copy.\nschemes:\n- name: PatlyticsOAuth\n  source: well-known/patlytics-oauth-authorization-server.json\n  issuer: https://mcp.patlytics.ai/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.patlytics.ai/authorize\n    tokenUrl: https://mcp.patlytics.ai/token\nresources:\n- resource: https://mcp.patlytics.ai/mcp\n  authorization_servers: [https://mcp.patlytics.ai/]\n  scopes_supported: [patent:search, patent:read]\n  bearer_methods_supported:\
  \ [header]\n  source: well-known/patlytics-oauth-protected-resource.json\nscopes:\n- scope: patent:search\n  description: >-\n    Run semantic searches — concept-level similarity search over patent claims and search of\n    non-patent literature (papers, journals, books via OpenAlex).\n  flows: [authorizationCode]\n  sources:\n  - well-known/patlytics-oauth-authorization-server.json\n  - well-known/patlytics-oauth-protected-resource.json\n- scope: patent:read\n  description: >-\n    Read patent records — bibliographic data and claims by publication number — and list the\n    organization's private Patlytics portfolios and vault patents.\n  flows: [authorizationCode]\n  sources:\n  - well-known/patlytics-oauth-authorization-server.json\n  - well-known/patlytics-oauth-protected-resource.json\nsummary:\n  scope_count: 2\n  write_scopes: 0\n  read_only: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/patlytics/refs/heads/main/scopes/patlytics-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Intellectual Property
- Patents
- Legal Tech
- Artificial Intelligence
- Patent Search
- Prior Art
- MCP
- Agents
- Research
token_urls:
- https://mcp.patlytics.ai/token
---
