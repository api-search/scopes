---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: 8B Education Investments Scopes
name_suffix: OAuth Scopes
note: ''
overview: '8B Education Investments uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: 8B Education Investments
provider_slug: 8b-education-investments
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: 8b-education-investments-scopes
source_filename: 8b-education-investments-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: https://www.8b.africa/.well-known/oauth-authorization-server\ndocs: null\ndocs_note: >-\n  8B publishes no scopes or permissions reference page. The scope set below is read\n  directly from the two machine-readable discovery documents the site serves, and nothing\n  is added to it. derive-oauth-scopes.py returned nothing for this provider because there\n  is no OpenAPI in the repository to derive from.\napi: 8b-education-investments-mcp\nflow: authorization_code\ngrant_types_supported:\n- authorization_code\n- refresh_token\nresponse_types_supported:\n- code\ncode_challenge_methods_supported:\n- S256\nauthorization_endpoint: https://www.8b.africa/oauth/authorize\ntoken_endpoint: https://www.8b.africa/oauth/token\nrevocation_endpoint: https://www.8b.africa/oauth/revoke\nscope_count: 1\nscopes:\n- name: mcp\n  description: >-\n    The single scope advertised by both the authorization-server metadata\n    (scopes_supported) and\
  \ the protected-resource metadata. It gates the Model Context\n    Protocol endpoint at https://www.8b.africa/wp-json/mcp/mcp-oauth-server as a whole.\n    No finer-grained scopes are published, so there is no read/write or per-resource\n    separation an agent could request; a token either reaches the entire MCP surface or\n    none of it.\n  evidence: https://www.8b.africa/.well-known/oauth-authorization-server\n  resource: https://www.8b.africa/wp-json/mcp/mcp-oauth-server\nnotes:\n- >-\n  scopes_supported appears identically in the RFC 8414 authorization-server document and\n  the RFC 9728 protected-resource document, which is the correct shape.\n- >-\n  Coarse granularity is the finding here: one scope over an unenumerated tool surface\n  means consent cannot be scoped to an operation. That is a property of the WordPress MCP\n  adapter default, not of a design decision 8B documented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/8b-education-investments/refs/heads/main/scopes/8b-education-investments-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Education
- Student Loans
- Financial Services
- Lending
- FinTech
- Africa
- Higher Education
- Study Abroad
- Community
token_urls: []
---
