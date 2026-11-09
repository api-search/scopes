---
api_specs:
- filename: dadan-io-openapi-generated.yml
  format: yaml
  label: Dadan Recording Request API
  slug: recording-request-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dadan-io/openapi/_ae-authored/dadan-io-openapi-generated.yml
authorization_urls: []
description: OAuth scopes of the Dadan MCP server, as advertised in its protected-resource and authorization-server metadata (HTTP 200). The REST Recording Request API uses an API key, not OAuth.
docs: https://kb.dadan.io/docs/use-dadan-with-your-ai-assistant-mcp
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Dadan Io Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Dadan publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Dadan API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Dadan
provider_slug: dadan-io
schemes:
- docs: https://kb.dadan.io/docs/use-dadan-with-your-ai-assistant-mcp
  grant_types:
  - authorization_code
  - refresh_token
  name: Dadan MCP OAuth
  notes: Token URL not recorded here; read the authorization-server metadata.
  tokenUrl: null
  type: oauth2
scope_count: 2
scope_names:
- dadan:full
- dadan:read
scopes:
- description: 'Default when connecting: docs say connecting "gives your assistant broad access to your Dadan account. It can read and change your library, using your account''s permissions."'
  flows: []
  scope: dadan:full
- description: 'Read-only access; docs: "To let it only search and read, tick **Read-only** on the Dadan sign-in page when you connect." (mapping of the checkbox to this scope name is inferred from the scope names, not stated).'
  flows: []
  scope: dadan:read
slug: dadan-io-scopes
source_filename: dadan-io-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource:\n- https://mcp.dadan.io/.well-known/oauth-protected-resource\n- https://kb.dadan.io/docs/use-dadan-with-your-ai-assistant-mcp\ndocs: https://kb.dadan.io/docs/use-dadan-with-your-ai-assistant-mcp\ndescription: OAuth scopes of the Dadan MCP server, as advertised in its protected-resource and authorization-server\n  metadata (HTTP 200). The REST Recording Request API uses an API key, not OAuth.\nschemes:\n- name: Dadan MCP OAuth\n  type: oauth2\n  grant_types:\n  - authorization_code\n  - refresh_token\n  tokenUrl: null\n  docs: https://kb.dadan.io/docs/use-dadan-with-your-ai-assistant-mcp\n  notes: Token URL not recorded here; read the authorization-server metadata.\nscopes:\n- scope: dadan:full\n  description: 'Default when connecting: docs say connecting \"gives your assistant broad access to your Dadan account.\n    It can read and change your library, using your account''s permissions.\"'\n  schemes:\n  - Dadan MCP OAuth\n\
  - scope: dadan:read\n  description: 'Read-only access; docs: \"To let it only search and read, tick **Read-only** on the Dadan sign-in\n    page when you connect.\" (mapping of the checkbox to this scope name is inferred from the scope names, not stated).'\n  schemes:\n  - Dadan MCP OAuth\n"
source_yaml_url: https://artifacts.apis.io/dadan-io/scopes/dadan-io-scopes.yml
summary_line: 2 scopes
tags:
- Company
- Video
- Screen Recording
- Video Hosting
- Video Analytics
- MCP
- AI Agents
token_bound: false
token_urls: []
---
