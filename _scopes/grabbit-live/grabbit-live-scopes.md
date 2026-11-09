---
api_specs:
- filename: grabbit-live-account-api-openapi.yml
  format: yaml
  label: grabbit-live Account API
  slug: grabbit-live-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grabbit-live/openapi/grabbit-live-account-api-openapi.yml
- filename: grabbit-live-grabs-api-openapi.yml
  format: yaml
  label: grabbit-live Grabs API
  slug: grabbit-live-grabs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grabbit-live/openapi/grabbit-live-grabs-api-openapi.yml
authorization_urls:
- https://www.grabbit.live/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Grabbit Live Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'grabbit-live publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the grabbit-live API on a user''s behalf.


  Tokens are issued from https://www.grabbit.live/api/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: grabbit-live
provider_slug: grabbit-live
schemes:
- description: OAuth 2.1 authorization code + PKCE with dynamic client registration (RFC 7591). Used by MCP clients such as claude.ai.
  flows:
  - authorizationUrl: https://www.grabbit.live/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://www.grabbit.live/api/v1/oauth/token
  name: oauth2
  source: openapi/grabbit-live-openapi.json
- description: OAuth 2.1 authorization code + PKCE with dynamic client registration (RFC 7591). Used by MCP clients such as claude.ai.
  flows:
  - authorizationUrl: https://www.grabbit.live/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://www.grabbit.live/api/v1/oauth/token
  name: oauth2
  source: openapi/www.grabbit.live_openapi.json
scope_count: 1
scope_names:
- grabs
scopes:
- description: Create, list, and read screenshots and read the team's credit balance.
  flows:
  - authorizationCode
  scope: grabs
slug: grabbit-live-scopes
source_filename: grabbit-live-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/grabbit-live-openapi.json, openapi/www.grabbit.live_openapi.json\nschemes:\n- name: oauth2\n  source: openapi/grabbit-live-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.grabbit.live/oauth/authorize\n    tokenUrl: https://www.grabbit.live/api/v1/oauth/token\n  description: OAuth 2.1 authorization code + PKCE with dynamic client registration (RFC 7591).\n    Used by MCP clients such as claude.ai.\n- name: oauth2\n  source: openapi/www.grabbit.live_openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.grabbit.live/oauth/authorize\n    tokenUrl: https://www.grabbit.live/api/v1/oauth/token\n  description: OAuth 2.1 authorization code + PKCE with dynamic client registration (RFC 7591).\n    Used by MCP clients such as claude.ai.\nscopes:\n- scope: grabs\n  description: Create, list, and read screenshots and read the team's credit balance.\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - openapi/grabbit-live-openapi.json\n  - openapi/www.grabbit.live_openapi.json\n"
source_yaml_url: https://artifacts.apis.io/grabbit-live/scopes/grabbit-live-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Screenshots
- AI Agents
- Automation
- Visual
token_bound: false
token_urls:
- https://www.grabbit.live/api/v1/oauth/token
---
