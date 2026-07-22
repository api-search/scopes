---
authorization_urls:
- https://mcp.mutinyhq.com/oauth/authorize
description: ''
docs: https://help.mutinyhq.com/articles/5003451538-connecting-mutiny-to-claude
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Mutiny Hq Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Mutiny HQ publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Mutiny HQ API on a user''s behalf.


  Tokens are issued from https://mcp.mutinyhq.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Mutiny HQ
provider_slug: mutiny-hq
schemes:
- flows:
  - authorizationUrl: https://mcp.mutinyhq.com/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://mcp.mutinyhq.com/oauth/token
  name: OAuth2
  source: well-known/mutiny-hq-oauth-authorization-server.json
scope_count: 5
scope_names:
- read_asset_groups
- create_asset_groups
- publish_asset_groups
- read_library_content
- manage_library_content
scopes:
- description: View assets, templates, and blueprints.
  flows:
  - authorizationCode
  scope: read_asset_groups
- description: Build assets and use the creative agent.
  flows:
  - authorizationCode
  scope: create_asset_groups
- description: Deploy/publish assets to production.
  flows:
  - authorizationCode
  scope: publish_asset_groups
- description: Browse content library items.
  flows:
  - authorizationCode
  scope: read_library_content
- description: Upload, modify, and remove content library items.
  flows:
  - authorizationCode
  scope: manage_library_content
slug: mutiny-hq-scopes
source_filename: mutiny-hq-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://mcp.mutinyhq.com/.well-known/oauth-authorization-server\ndocs: https://help.mutinyhq.com/articles/5003451538-connecting-mutiny-to-claude\nschemes:\n- name: OAuth2\n  source: well-known/mutiny-hq-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.mutinyhq.com/oauth/authorize\n    tokenUrl: https://mcp.mutinyhq.com/oauth/token\n    pkce: S256\nscopes:\n- scope: read_asset_groups\n  description: View assets, templates, and blueprints.\n  flows: [authorizationCode]\n  sources: [well-known/mutiny-hq-oauth-authorization-server.json]\n- scope: create_asset_groups\n  description: Build assets and use the creative agent.\n  flows: [authorizationCode]\n  sources: [well-known/mutiny-hq-oauth-authorization-server.json]\n- scope: publish_asset_groups\n  description: Deploy/publish assets to production.\n  flows: [authorizationCode]\n  sources: [well-known/mutiny-hq-oauth-authorization-server.json]\n\
  - scope: read_library_content\n  description: Browse content library items.\n  flows: [authorizationCode]\n  sources: [well-known/mutiny-hq-oauth-authorization-server.json]\n- scope: manage_library_content\n  description: Upload, modify, and remove content library items.\n  flows: [authorizationCode]\n  sources: [well-known/mutiny-hq-oauth-authorization-server.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mutiny-hq/refs/heads/main/scopes/mutiny-hq-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Company
- GTM
- Sales Enablement
- Marketing
- Website Personalization
- AI
- Agents
- MCP
- ABM
- Content Generation
token_urls:
- https://mcp.mutinyhq.com/oauth/token
---
