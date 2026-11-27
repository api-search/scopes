---
api_specs:
- filename: corebee-ai-auth-api-openapi.yml
  format: yaml
  label: Corebee Auth API
  slug: corebee-ai-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corebee-ai/openapi/corebee-ai-auth-api-openapi.yml
- filename: corebee-ai-contacts-api-openapi.yml
  format: yaml
  label: Corebee Contacts API
  slug: corebee-ai-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corebee-ai/openapi/corebee-ai-contacts-api-openapi.yml
- filename: corebee-ai-conversations-api-openapi.yml
  format: yaml
  label: Corebee Conversations API
  slug: corebee-ai-conversations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corebee-ai/openapi/corebee-ai-conversations-api-openapi.yml
- filename: corebee-ai-labels-api-openapi.yml
  format: yaml
  label: Corebee Labels API
  slug: corebee-ai-labels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corebee-ai/openapi/corebee-ai-labels-api-openapi.yml
- filename: corebee-ai-voice-api-openapi.yml
  format: yaml
  label: Corebee Voice API
  slug: corebee-ai-voice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corebee-ai/openapi/corebee-ai-voice-api-openapi.yml
- filename: corebee-ai-webhooks-api-openapi.yml
  format: yaml
  label: Corebee Webhooks API
  slug: corebee-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corebee-ai/openapi/corebee-ai-webhooks-api-openapi.yml
authorization_urls: []
description: ''
docs: https://corebee.ai/api/v1/openapi.json
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Corebee Scopes
name_suffix: OAuth Scopes
note: OAuth 2.1 (authorization_code + refresh_token, PKCE S256, Dynamic Client Registration at https://corebee.ai/api/v1/mcp/oauth/register). The spec models auth as http bearer, so no oauth2 securityScheme exists to derive from; scopes are read from the authorization-server metadata. voice:bridge is named in the spec but not in scopes_supported (it is an API-key permission chosen when the key is minted).
overview: 'Corebee publishes 12 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Corebee API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Corebee
provider_slug: corebee-ai
schemes: []
scope_count: 12
scope_names:
- conversations:read
- conversations:write
- contacts:read
- contacts:write
- contacts:delete
- knowledge:read
- knowledge:write
- knowledge:delete
- metrics:read
- settings:read
- settings:write
- voice:bridge
scopes:
- description: ''
  flows: []
  scope: conversations:read
- description: ''
  flows: []
  scope: conversations:write
- description: ''
  flows: []
  scope: contacts:read
- description: ''
  flows: []
  scope: contacts:write
- description: ''
  flows: []
  scope: contacts:delete
- description: ''
  flows: []
  scope: knowledge:read
- description: ''
  flows: []
  scope: knowledge:write
- description: ''
  flows: []
  scope: knowledge:delete
- description: ''
  flows: []
  scope: metrics:read
- description: ''
  flows: []
  scope: settings:read
- description: ''
  flows: []
  scope: settings:write
- description: Required by every voice/bridge operation; an all-access * key is not enough for some voice operations.
  flows: []
  scope: voice:bridge
slug: corebee-ai-scopes
source_filename: corebee-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://corebee.ai/.well-known/oauth-authorization-server\ndocs: https://corebee.ai/api/v1/openapi.json\nname: Corebee OAuth scopes\nnote: OAuth 2.1 (authorization_code + refresh_token, PKCE S256, Dynamic Client Registration at https://corebee.ai/api/v1/mcp/oauth/register).\n  The spec models auth as http bearer, so no oauth2 securityScheme exists to derive from; scopes are read\n  from the authorization-server metadata. voice:bridge is named in the spec but not in scopes_supported\n  (it is an API-key permission chosen when the key is minted).\nscopes:\n- name: conversations:read\n  source: oauth-authorization-server scopes_supported\n- name: conversations:write\n  source: oauth-authorization-server scopes_supported\n- name: contacts:read\n  source: oauth-authorization-server scopes_supported\n- name: contacts:write\n  source: oauth-authorization-server scopes_supported\n- name: contacts:delete\n  source: oauth-authorization-server\
  \ scopes_supported\n- name: knowledge:read\n  source: oauth-authorization-server scopes_supported\n- name: knowledge:write\n  source: oauth-authorization-server scopes_supported\n- name: knowledge:delete\n  source: oauth-authorization-server scopes_supported\n- name: metrics:read\n  source: oauth-authorization-server scopes_supported\n- name: settings:read\n  source: oauth-authorization-server scopes_supported\n- name: settings:write\n  source: oauth-authorization-server scopes_supported\n- name: voice:bridge\n  description: Required by every voice/bridge operation; an all-access * key is not enough for some voice\n    operations.\n  source: openapi bearerAuth description\n"
source_yaml_url: https://artifacts.apis.io/corebee-ai/scopes/corebee-ai-scopes.yml
summary_line: 12 scopes
tags:
- Company
- Customer Service
- Artificial Intelligence
- Chatbots
- Help Desk
- Omnichannel Messaging
- Voice Agents
- MCP
token_bound: false
token_urls: []
---
