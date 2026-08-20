---
api_specs:
- filename: storylane-connect
  format: yaml
  label: Storylane External API
  slug: storylane-external-api
  spec_type: Postman
  url: https://www.postman.com/team-storylane/storylane-public/collection/2zkg7jc/storylane-connect
authorization_urls: []
description: 'OAuth 2.0 scopes Storylane publishes in its RFC 8414 Authorization Server Metadata at identity.storylane.io. These are the scopes an MCP client requests when a user authorizes Claude, ChatGPT or another MCP-capable client against the Storylane MCP server. Scope descriptions below are derived from the scope names and the documented MCP tool categories — Storylane does not publish a per-scope permissions reference page, so no description here is quoted from the provider.

  '
docs: https://docs.storylane.io/integrations/integrations-and-data-flow/mcp
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Storylane Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Storylane uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Storylane
provider_slug: storylane
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: storylane-scopes
source_filename: storylane-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://identity.storylane.io/.well-known/oauth-authorization-server\ndocs: https://docs.storylane.io/integrations/integrations-and-data-flow/mcp\ndescription: >\n  OAuth 2.0 scopes Storylane publishes in its RFC 8414 Authorization Server\n  Metadata at identity.storylane.io. These are the scopes an MCP client requests\n  when a user authorizes Claude, ChatGPT or another MCP-capable client against\n  the Storylane MCP server. Scope descriptions below are derived from the\n  scope names and the documented MCP tool categories — Storylane does not\n  publish a per-scope permissions reference page, so no description here is\n  quoted from the provider.\nissuer: https://identity.storylane.io\nauthorization_endpoint: https://identity.storylane.io/oauth/authorize\ntoken_endpoint: https://identity.storylane.io/oauth/token\nregistration_endpoint: https://identity.storylane.io/oauth/register\ngrant_types_supported:\n  - authorization_code\n\
  \  - client_credentials\n  - refresh_token\ncode_challenge_methods_supported:\n  - S256\ntoken_endpoint_auth_methods_supported:\n  - none\n  - client_secret_post\nscope_count: 4\nscopes:\n  - name: mcp\n    description: >\n      Access to the Storylane MCP server transport itself. Published in the\n      authorization server metadata; required to reach\n      https://identity.storylane.io/mcp.\n    source: authorization-server-metadata\n  - name: demos_read\n    description: >\n      Read access to the demo library. Aligns with the documented read tools\n      list_workspaces, list_demos, get_demo, get_demo_status, list_hubs,\n      get_hub, list_links and list_voices.\n    source: authorization-server-metadata\n    tools_inferred:\n      - list_workspaces\n      - list_demos\n      - get_demo\n      - get_demo_status\n      - list_hubs\n      - get_hub\n      - list_links\n      - list_voices\n  - name: demos_write\n    description: >\n      Write access to demos and share links. Aligns\
  \ with the documented write\n      tools convert_images_to_demo, convert_video_to_demo, add_step,\n      personalise_demo, update_demo_settings, publish_demo, create_link and\n      update_link. Storylane's ChatGPT setup notes that write actions require\n      Developer Mode, which is in beta for Business and Enterprise plans.\n    source: authorization-server-metadata\n    tools_inferred:\n      - convert_images_to_demo\n      - convert_video_to_demo\n      - add_step\n      - personalise_demo\n      - update_demo_settings\n      - publish_demo\n      - create_link\n      - update_link\n  - name: analytics_read\n    description: >\n      Read access to demo engagement analytics, captured leads and engaged\n      accounts. Aligns with get_demo_analytics, get_leads and get_accounts.\n    source: authorization-server-metadata\n    tools_inferred:\n      - get_demo_analytics\n      - get_leads\n      - get_accounts\nnotes:\n  - >\n    Scope-to-tool mapping is INFERRED from scope names against\
  \ the provider's\n    published tool catalog. Storylane publishes no scopes reference page, so the\n    mapping is a reasonable reading, not a provider statement.\n  - >\n    All scopes are additionally workspace-scoped at runtime: the docs state every\n    tool is limited to the authenticated user's active workspace and their own\n    permissions within it.\n  - >\n    The External REST API does NOT use these scopes. It authenticates with a\n    support-issued Bearer access_token plus a workspace_id and has no scope model.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/storylane/refs/heads/main/scopes/storylane-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Interactive Demos
- Product Walkthroughs
- Sales Enablement
- Marketing
- Demo Analytics
- Demo Automation
- Buyer Hub
- Sales
- MCP
- Agent Tools
- Webhook
- Embeds
- oEmbed
- Demo Automation Platform
token_urls: []
---
