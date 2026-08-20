---
api_specs:
- filename: synup-api-openapi.yml
  format: yaml
  label: Synup API
  slug: synup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synup/refs/heads/main/openapi/synup-api-openapi.yml
authorization_urls: []
description: The only OAuth surface Synup publishes is the MCP server. Its authorization-server metadata declares two coarse scopes. The REST API v4 has no OAuth and therefore no scopes — it is API-key authenticated.
docs: https://developer.synup.com/synup-mcp-getting-connected-doc-2070739
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Synup Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Synup publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Synup API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Synup
provider_slug: synup
schemes: []
scope_count: 2
scope_names:
- mcp:read
- mcp:write
scopes:
- description: 'Read-only access to the Synup MCP tool surface: look up locations, reviews, rankings, listings, analytics. Equivalent to X-access-mode: read for key-authenticated sessions.'
  flows: []
  scope: mcp:read
- description: 'Create, update and delete through the Synup MCP tool surface. Equivalent to X-access-mode: write. Synup guidance is to start in read and switch to write deliberately.'
  flows: []
  scope: mcp:write
slug: synup-scopes
source_filename: synup-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "name: Synup OAuth scopes\ngenerated: '2026-08-13'\nmethod: probed\nsource: https://mcp-agent.synup.com/.well-known/oauth-authorization-server\ndocs: https://developer.synup.com/synup-mcp-getting-connected-doc-2070739\ndescription: The only OAuth surface Synup publishes is the MCP server. Its authorization-server metadata\n  declares two coarse scopes. The REST API v4 has no OAuth and therefore no scopes — it is API-key authenticated.\nissuer: https://mcp-agent.synup.com\napplies_to: https://mcp-agent.synup.com/mcp (and every tenant workspace domain + /mcp)\nscope_count: 2\nscopes:\n- scope: mcp:read\n  description: 'Read-only access to the Synup MCP tool surface: look up locations, reviews, rankings,\n    listings, analytics. Equivalent to X-access-mode: read for key-authenticated sessions.'\n- scope: mcp:write\n  description: 'Create, update and delete through the Synup MCP tool surface. Equivalent to X-access-mode:\n    write. Synup guidance is to start in read and switch\
  \ to write deliberately.'\ngranularity: coarse\nnotes:\n- Both scopes were read from the live RFC 8414 document and confirmed in the WWW-Authenticate challenge\n  on an anonymous tools/list call (scope=\"mcp:read mcp:write\").\n- There is no per-domain or per-resource scope; the X-tags-include/X-tags-exclude headers narrow which\n  tools are surfaced but are not an authorization boundary.\n- REST API v4 keys are unscoped — see authentication/synup-authentication.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synup/refs/heads/main/scopes/synup-scopes.yml
summary_line: 2 scopes
tags:
- Local Marketing
- Listings Management
- Reputation Management
- Local SEO
- Reviews
- Social-Media
- Analytics
- Business Listings
- Review Management
- Agency Software
token_urls: []
---
