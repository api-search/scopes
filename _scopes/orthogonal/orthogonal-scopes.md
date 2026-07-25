---
api_specs:
- filename: orthogonal-account-api-openapi.yml
  format: yaml
  label: Orthogonal Account API
  slug: orthogonal-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orthogonal/refs/heads/main/openapi/orthogonal-account-api-openapi.yml
- filename: orthogonal-discovery-api-openapi.yml
  format: yaml
  label: Orthogonal Discovery API
  slug: orthogonal-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orthogonal/refs/heads/main/openapi/orthogonal-discovery-api-openapi.yml
- filename: orthogonal-run-api-openapi.yml
  format: yaml
  label: Orthogonal Run API
  slug: orthogonal-run-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orthogonal/refs/heads/main/openapi/orthogonal-run-api-openapi.yml
authorization_urls: []
description: OAuth 2.0 scopes advertised by Orthogonal's authorization server metadata (issuer clerk.orthogonal.com). These govern the hosted MCP OAuth flow; the REST API itself uses opaque API keys with no scope model. Scopes below are the Clerk scoped-access set exposed for api.orthogonal.com.
docs: https://clerk.com/docs/oauth/scoped-access
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Orthogonal Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Orthogonal uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Orthogonal
provider_slug: orthogonal
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: orthogonal-scopes
source_filename: orthogonal-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://api.orthogonal.com/.well-known/oauth-authorization-server\ndocs: https://clerk.com/docs/oauth/scoped-access\ndescription: >-\n  OAuth 2.0 scopes advertised by Orthogonal's authorization server metadata\n  (issuer clerk.orthogonal.com). These govern the hosted MCP OAuth flow; the\n  REST API itself uses opaque API keys with no scope model. Scopes below are the\n  Clerk scoped-access set exposed for api.orthogonal.com.\noauth2:\n  authorization_endpoint: https://clerk.orthogonal.com/oauth/authorize\n  token_endpoint: https://clerk.orthogonal.com/oauth/token\nscopes:\n- name: openid\n  description: OpenID Connect sign-in; issues an ID token.\n- name: profile\n  description: Access the user's basic profile information.\n- name: email\n  description: Access the user's email address.\n- name: public_metadata\n  description: Read the user's public metadata.\n- name: private_metadata\n  description: Read the user's private\
  \ metadata.\n- name: offline_access\n  description: Issue a refresh token for offline/long-lived access.\n- name: 'user:org:read'\n  description: Read the user's organization membership.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orthogonal/refs/heads/main/scopes/orthogonal-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- AI Agents
- API Discovery
- API Marketplace
- Agent Payments
- MCP
- Data Enrichment
- Crypto
- Stablecoins
token_urls: []
---
