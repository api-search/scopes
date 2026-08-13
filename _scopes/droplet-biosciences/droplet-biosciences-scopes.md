---
authorization_urls:
- https://dropletbiosci.com/events-manager/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Droplet Biosciences Scopes
name_suffix: OAuth Scopes
note: Read verbatim from the live authorization-server metadata document, not from documentation — the provider publishes no scope reference page. The scope surface is a single scope emitted by the Events Manager WordPress plugin, not a Droplet product permission model. derive-oauth-scopes.py was not the source here because there is no OpenAPI in this repo to derive from.
overview: 'Droplet Biosciences publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Droplet Biosciences API on a user''s behalf.


  Tokens are issued from https://dropletbiosci.com/wp-json/oauth/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Droplet Biosciences
provider_slug: droplet-biosciences
schemes:
- flows:
  - authorizationUrl: https://dropletbiosci.com/events-manager/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://dropletbiosci.com/wp-json/oauth/v1/token
  issuer: https://dropletbiosci.com/events-manager
  name: oauth2
  source: https://dropletbiosci.com/wp-json/oauth/v1/metadata
scope_count: 1
scope_names:
- events-manager:mcp
scopes:
- description: The only scope advertised in scopes_supported. Grants access to the Events Manager MCP server at /wp-json/mcp/events-manager. No description is published by the provider; this text is a statement of where the scope is used, not a quotation.
  flows:
  - authorizationCode
  scope: events-manager:mcp
slug: droplet-biosciences-scopes
source_filename: droplet-biosciences-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://dropletbiosci.com/wp-json/oauth/v1/metadata\ndocs: null\nnote: >-\n  Read verbatim from the live authorization-server metadata document, not from documentation —\n  the provider publishes no scope reference page. The scope surface is a single scope emitted by\n  the Events Manager WordPress plugin, not a Droplet product permission model. derive-oauth-scopes.py\n  was not the source here because there is no OpenAPI in this repo to derive from.\nschemes:\n- name: oauth2\n  source: https://dropletbiosci.com/wp-json/oauth/v1/metadata\n  issuer: https://dropletbiosci.com/events-manager\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://dropletbiosci.com/events-manager/oauth/authorize\n    tokenUrl: https://dropletbiosci.com/wp-json/oauth/v1/token\nscopes:\n- scope: events-manager:mcp\n  description: >-\n    The only scope advertised in scopes_supported. Grants access to the Events Manager MCP server\n  \
  \  at /wp-json/mcp/events-manager. No description is published by the provider; this text is a\n    statement of where the scope is used, not a quotation.\n  flows: [authorizationCode]\n  sources: [https://dropletbiosci.com/wp-json/oauth/v1/metadata]\nscope_count: 1\ngaps:\n- The other two MCP servers (mcp-adapter-default-server, amelia-mcp-server) have no advertised scope.\n- No scope-to-permission mapping, and no granularity beyond a single all-or-nothing scope.\nx-evidence:\n  fetched: '2026-08-12'\n  url: https://dropletbiosci.com/wp-json/oauth/v1/metadata\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/droplet-biosciences/refs/heads/main/scopes/droplet-biosciences-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Health
- Healthcare
- Diagnostics
- Oncology
- Genomics
- Liquid Biopsy
- Life Sciences
- Biotechnology
- Clinical Laboratory
token_urls:
- https://dropletbiosci.com/wp-json/oauth/v1/token
---
