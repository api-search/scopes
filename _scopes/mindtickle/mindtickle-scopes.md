---
authorization_urls:
- https://app.mindtickle.com/api/users/v1/oauth/authorize
description: 'Mindtickle publishes its OAuth 2.0 scope vocabulary anonymously in two places: scopes_supported in the RFC 8414 authorization-server metadata and scopes_supported in the RFC 9728 protected-resource metadata. Both lists are identical - seven scopes covering AI roleplays, call recordings, Copilot chat, digital sales rooms and search. Descriptions below are DERIVED from the scope name plus the matching product surface in Mindtickle''s own product pages; the provider publishes no prose scope reference, so the strings themselves are the only authoritative part.'
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: probed
name: Mindtickle Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Mindtickle publishes 7 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Mindtickle API on a user''s behalf.


  Tokens are issued from https://app.mindtickle.com/api/users/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Mindtickle
provider_slug: mindtickle
schemes:
- flows:
  - authorizationUrl: https://app.mindtickle.com/api/users/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://app.mindtickle.com/api/users/v1/oauth/token
  - flow: clientCredentials
    tokenUrl: https://app.mindtickle.com/api/users/v1/oauth/token
  issuer: https://app.mindtickle.com
  name: mindtickleOAuth2
  source: well-known/mindtickle-oauth-authorization-server.json
scope_count: 7
scope_names:
- read:ai_roleplays
- write:ai_roleplays
- read:calls
- read:copilot_chat
- read:rooms
- write:rooms
- read:search
scopes:
- description: Read access to AI role play simulations and their results. Derived label - Mindtickle publishes no scope reference page.
  flows:
  - authorizationCode
  - clientCredentials
  scope: read:ai_roleplays
- description: Create or modify AI role play simulations. Derived label.
  flows:
  - authorizationCode
  - clientCredentials
  scope: write:ai_roleplays
- description: Read access to call recordings, transcripts and conversation-intelligence data - the same domain the Call AI public GraphQL API exposes. Derived label.
  flows:
  - authorizationCode
  - clientCredentials
  scope: read:calls
- description: Read access to Mindtickle Copilot chat. Derived label.
  flows:
  - authorizationCode
  - clientCredentials
  scope: read:copilot_chat
- description: Read access to digital sales rooms and their buyer-engagement data. Derived label.
  flows:
  - authorizationCode
  - clientCredentials
  scope: read:rooms
- description: Create or modify digital sales rooms. Derived label.
  flows:
  - authorizationCode
  - clientCredentials
  scope: write:rooms
- description: Read access to platform-wide search across content and readiness objects. Derived label.
  flows:
  - authorizationCode
  - clientCredentials
  scope: read:search
slug: mindtickle-scopes
source_filename: mindtickle-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://app.mindtickle.com/.well-known/oauth-protected-resource\nname: Mindtickle OAuth 2.0 scopes\ndescription: >-\n  Mindtickle publishes its OAuth 2.0 scope vocabulary anonymously in two places:\n  scopes_supported in the RFC 8414 authorization-server metadata and\n  scopes_supported in the RFC 9728 protected-resource metadata. Both lists are\n  identical - seven scopes covering AI roleplays, call recordings, Copilot chat,\n  digital sales rooms and search. Descriptions below are DERIVED from the scope\n  name plus the matching product surface in Mindtickle's own product pages; the\n  provider publishes no prose scope reference, so the strings themselves are the\n  only authoritative part.\ndocs: null\n\nschemes:\n- name: mindtickleOAuth2\n  source: well-known/mindtickle-oauth-authorization-server.json\n  issuer: https://app.mindtickle.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.mindtickle.com/api/users/v1/oauth/authorize\n\
  \    tokenUrl: https://app.mindtickle.com/api/users/v1/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://app.mindtickle.com/api/users/v1/oauth/token\n\nscopes:\n- scope: read:ai_roleplays\n  access: read\n  resource: AI Sales Role Play\n  description: >-\n    Read access to AI role play simulations and their results. Derived label -\n    Mindtickle publishes no scope reference page.\n  flows: [authorizationCode, clientCredentials]\n  sources: [well-known/mindtickle-oauth-authorization-server.json, well-known/mindtickle-oauth-protected-resource.json]\n- scope: write:ai_roleplays\n  access: write\n  resource: AI Sales Role Play\n  description: >-\n    Create or modify AI role play simulations. Derived label.\n  flows: [authorizationCode, clientCredentials]\n  sources: [well-known/mindtickle-oauth-authorization-server.json, well-known/mindtickle-oauth-protected-resource.json]\n- scope: read:calls\n  access: read\n  resource: Call AI / Conversation Intelligence\n  description:\
  \ >-\n    Read access to call recordings, transcripts and conversation-intelligence\n    data - the same domain the Call AI public GraphQL API exposes. Derived label.\n  flows: [authorizationCode, clientCredentials]\n  sources: [well-known/mindtickle-oauth-authorization-server.json, well-known/mindtickle-oauth-protected-resource.json]\n- scope: read:copilot_chat\n  access: read\n  resource: Copilot\n  description: >-\n    Read access to Mindtickle Copilot chat. Derived label.\n  flows: [authorizationCode, clientCredentials]\n  sources: [well-known/mindtickle-oauth-authorization-server.json, well-known/mindtickle-oauth-protected-resource.json]\n- scope: read:rooms\n  access: read\n  resource: Digital Sales Room\n  description: >-\n    Read access to digital sales rooms and their buyer-engagement data. Derived label.\n  flows: [authorizationCode, clientCredentials]\n  sources: [well-known/mindtickle-oauth-authorization-server.json, well-known/mindtickle-oauth-protected-resource.json]\n-\
  \ scope: write:rooms\n  access: write\n  resource: Digital Sales Room\n  description: >-\n    Create or modify digital sales rooms. Derived label.\n  flows: [authorizationCode, clientCredentials]\n  sources: [well-known/mindtickle-oauth-authorization-server.json, well-known/mindtickle-oauth-protected-resource.json]\n- scope: read:search\n  access: read\n  resource: Platform search\n  description: >-\n    Read access to platform-wide search across content and readiness objects.\n    Derived label.\n  flows: [authorizationCode, clientCredentials]\n  sources: [well-known/mindtickle-oauth-authorization-server.json, well-known/mindtickle-oauth-protected-resource.json]\n\nsummary:\n  scope_count: 7\n  read_scopes: 5\n  write_scopes: 2\n  granularity: resource-and-verb\n  notes:\n  - >-\n    The scope vocabulary is shaped like an agent/assistant surface (roleplays,\n    Copilot chat, calls, rooms, search) rather than like the admin REST API\n    (users, groups, modules, reporting). No MCP endpoint\
  \ was found on any host -\n    every /mcp, /api/mcp, /sse and /copilot/mcp path returns the same generic\n    \"learner not authenticated\" 401 that a nonsense path returns, so no MCP\n    server is claimed.\n  - >-\n    Mindtickle publishes no human-readable scope reference. The strings are\n    authoritative; the descriptions here are derived and should be replaced if\n    the provider publishes a permissions page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mindtickle/refs/heads/main/scopes/mindtickle-scopes.yml
summary_line: 7 scopes · authorizationCode/clientCredentials
tags:
- Sales Enablement
- Revenue Productivity
- Sales Readiness
- Coaching
- Conversation Intelligence
- Learning Management
- Content Management
- Call AI
- Revenue Intelligence
token_urls:
- https://app.mindtickle.com/api/users/v1/oauth/token
---
