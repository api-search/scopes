---
authorization_urls: []
description: ''
docs: https://docs.webz.io/docs/webz/news-search-api-mcp
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Webz Scopes
name_suffix: OAuth Scopes
note: Webz.io's REST APIs use a single opaque API token with no scopes; entitlement is a per-product permission on the account, not an OAuth scope. The only OAuth surface is the authorization server in front of the News Search MCP endpoint, and it advertises exactly one scope. Recorded from the live RFC 8414 metadata document, not inferred.
overview: 'Webz.io uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Webz.io
provider_slug: webz
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: webz-scopes
source_filename: webz-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: https://news-search-mcp.webz.io/.well-known/oauth-authorization-server\ndocs: https://docs.webz.io/docs/webz/news-search-api-mcp\nnote: >-\n  Webz.io's REST APIs use a single opaque API token with no scopes; entitlement is a per-product\n  permission on the account, not an OAuth scope. The only OAuth surface is the authorization server\n  in front of the News Search MCP endpoint, and it advertises exactly one scope. Recorded from the\n  live RFC 8414 metadata document, not inferred.\nauthorization_server: https://news-search-mcp.webz.io/\nresource: https://news-search-mcp.webz.io/mcp\nscope_count: 1\nscopes:\n- name: mcp\n  description: >-\n    The only scope the News Search MCP authorization server advertises in scopes_supported. It grants\n    access to the single protected resource https://news-search-mcp.webz.io/mcp; the server publishes\n    no finer-grained or per-tool scopes.\n  source: scopes_supported in the RFC 8414\
  \ metadata\nflows:\n  authorization_code:\n    supported: true\n    pkce: S256\n  refresh_token:\n    supported: true\n  client_credentials:\n    supported: false\ntoken_endpoint_auth_methods_supported:\n- client_secret_post\n- client_secret_basic\ndynamic_client_registration: https://news-search-mcp.webz.io/register\nnon_oauth_entitlements:\n  note: >-\n    These are account permissions, not scopes. They are listed here because they are what actually\n    gates access on the REST surface, and an agent planning a call needs to know them.\n  permissions:\n  - api_news\n  products_requiring_separate_entitlement:\n  - News / Blogs / Forums\n  - Reviews\n  - Cyber\n  - Data Breaches\n  - Archive\n  - Firehose\n  - view-password (Data Breaches — returns unmasked passwords)\n  - per-domain authorization (Data Breaches)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/webz/refs/heads/main/scopes/webz-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- news-data
- web-data
- web-scraping
- dark-web
- deep-web
- cybersecurity
- threat-intelligence
- data-breach
- pii-monitoring
- osint
- reviews-data
- ai-training-data
- media-monitoring
token_urls: []
---
