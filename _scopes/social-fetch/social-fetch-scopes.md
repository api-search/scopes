---
api_specs:
- filename: openapi.json
  format: json
  label: Social Fetch REST API
  slug: social-fetch-rest-api
  spec_type: OpenAPI
  url: https://www.socialfetch.dev/openapi.json
authorization_urls: []
description: ''
docs: https://www.socialfetch.dev/docs/integrations/mcp.mdx
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Social Fetch Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Social Fetch uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Social Fetch
provider_slug: social-fetch
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: social-fetch-scopes
source_filename: social-fetch-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-11'\nmethod: searched\nsource: >-\n  OAuth 2.0 / OpenID Connect discovery documents served at\n  api.socialfetch.dev/.well-known/openid-configuration and\n  app.socialfetch.dev, plus docs/integrations/mcp.mdx. Read 2026-09-11.\ndocs: https://www.socialfetch.dev/docs/integrations/mcp.mdx\nauthorization_server: https://app.socialfetch.dev\ngrant_types:\n  - authorization_code\n  - client_credentials\n  - refresh_token\npkce: S256\nscopes:\n  - name: openid\n    description: OpenID Connect authentication (issue an ID token).\n  - name: profile\n    description: Access basic profile claims (name, picture, given/family name).\n  - name: email\n    description: Access email and email_verified claims.\n  - name: offline_access\n    description: Issue a refresh token for long-lived access.\n  - name: socialfetch:read\n    description: >-\n      Read access to Social Fetch data operations — the scope MCP/OAuth clients\n      request to call /v1 read routes on the\
  \ user's behalf.\nnotes: >-\n  The REST OpenAPI itself declares only an apiKey scheme (x-api-key, sfk_...); the\n  OAuth scopes above govern the hosted MCP endpoint and are advertised via the\n  served authorization-server metadata. scopes_supported is identical on the api\n  and app hosts.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/social-fetch/refs/heads/main/scopes/social-fetch-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- social media
- web scraping
- data extraction
- social listening
- monitoring
- structured data
- JSON API
- REST
- MCP
- agent-native
- TypeScript SDK
- transcripts
- ads intelligence
token_urls: []
---
