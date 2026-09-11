---
api_specs:
- filename: aerofarms-news-openapi.yml
  format: yaml
  label: AeroFarms News API
  slug: aerofarms-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerofarms/refs/heads/main/openapi/aerofarms-news-openapi.yml
- filename: aerofarms-pages-openapi.yml
  format: yaml
  label: AeroFarms Pages API
  slug: aerofarms-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerofarms/refs/heads/main/openapi/aerofarms-pages-openapi.yml
- filename: aerofarms-products-openapi.yml
  format: yaml
  label: AeroFarms Products API
  slug: aerofarms-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerofarms/refs/heads/main/openapi/aerofarms-products-openapi.yml
- filename: aerofarms-store-openapi.yml
  format: yaml
  label: AeroFarms Store API
  slug: aerofarms-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerofarms/refs/heads/main/openapi/aerofarms-store-openapi.yml
- filename: aerofarms-faq-openapi.yml
  format: yaml
  label: AeroFarms FAQ API
  slug: aerofarms-faq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerofarms/refs/heads/main/openapi/aerofarms-faq-openapi.yml
- filename: aerofarms-taxonomy-openapi.yml
  format: yaml
  label: AeroFarms Taxonomy API
  slug: aerofarms-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerofarms/refs/heads/main/openapi/aerofarms-taxonomy-openapi.yml
- filename: aerofarms-media-openapi.yml
  format: yaml
  label: AeroFarms Media API
  slug: aerofarms-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerofarms/refs/heads/main/openapi/aerofarms-media-openapi.yml
- filename: aerofarms-search-openapi.yml
  format: yaml
  label: AeroFarms Search API
  slug: aerofarms-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerofarms/refs/heads/main/openapi/aerofarms-search-openapi.yml
- filename: aerofarms-discovery-openapi.yml
  format: yaml
  label: AeroFarms Discovery API
  slug: aerofarms-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerofarms/refs/heads/main/openapi/aerofarms-discovery-openapi.yml
authorization_urls: []
description: AeroFarms publishes no scope reference page — it publishes no developer documentation at all. The single scope below is not derived from an OpenAPI oauth2 flow (none exists); it is read verbatim from the scopes_supported array of the authorization-server metadata document the site itself serves, and from the matching scopes_supported in its protected-resource metadata.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Aerofarms Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'AeroFarms uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AeroFarms
provider_slug: aerofarms
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: aerofarms-scopes
source_filename: aerofarms-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: probed\nsource: https://www.aerofarms.com/.well-known/oauth-authorization-server (RFC 8414, fetched 2026-09-10)\ndocs: null\ndescription: >-\n  AeroFarms publishes no scope reference page — it publishes no developer documentation at all. The\n  single scope below is not derived from an OpenAPI oauth2 flow (none exists); it is read verbatim\n  from the scopes_supported array of the authorization-server metadata document the site itself\n  serves, and from the matching scopes_supported in its protected-resource metadata.\nauthorization_server: https://www.aerofarms.com\nprotected_resource: https://www.aerofarms.com/wp-json/mcp/mcp-oauth-server\nscope_count: 1\nscopes:\n- name: mcp\n  description: >-\n    Access to the Model Context Protocol server at /wp-json/mcp/mcp-oauth-server. The provider gives\n    no finer definition, and there is no second scope: authorization to this resource is all-or-nothing\n    at the protocol level. What a token\
  \ actually permits inside the server is decided by the WordPress\n    capabilities of the identity behind it, which is not expressed in the scope vocabulary.\n  source: scopes_supported\n  evidence: https://www.aerofarms.com/.well-known/oauth-authorization-server\ngranularity:\n  verdict: coarse\n  note: >-\n    One scope for one resource. An agent cannot request read-only access, and a consent screen cannot\n    tell a user which tools the grant covers. This is the WordPress MCP Adapter default rather than a\n    choice AeroFarms documented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aerofarms/refs/heads/main/scopes/aerofarms-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Agriculture
- Vertical Farming
- Indoor Farming
- AgTech
- Food and Beverage
- Consumer Packaged Goods
- Microgreens
- Sustainability
- Content
- Commerce
- MCP
token_urls: []
---
