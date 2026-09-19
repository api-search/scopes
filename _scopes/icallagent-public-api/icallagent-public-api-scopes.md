---
api_specs:
- filename: icallagent-public-api-agents-api-openapi.yml
  format: yaml
  label: iCallAgent Public API Agents API
  slug: icallagent-public-api-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icallagent-public-api/refs/heads/main/openapi/icallagent-public-api-agents-api-openapi.yml
- filename: icallagent-public-api-campaigns-api-openapi.yml
  format: yaml
  label: iCallAgent Public API Campaigns API
  slug: icallagent-public-api-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icallagent-public-api/refs/heads/main/openapi/icallagent-public-api-campaigns-api-openapi.yml
- filename: icallagent-public-api-contacts-api-openapi.yml
  format: yaml
  label: iCallAgent Public API Contacts API
  slug: icallagent-public-api-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icallagent-public-api/refs/heads/main/openapi/icallagent-public-api-contacts-api-openapi.yml
- filename: icallagent-public-api-phone-numbers-api-openapi.yml
  format: yaml
  label: iCallAgent Public API Phone Numbers API
  slug: icallagent-public-api-phone-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icallagent-public-api/refs/heads/main/openapi/icallagent-public-api-phone-numbers-api-openapi.yml
- filename: icallagent-public-api-webhooks-api-openapi.yml
  format: yaml
  label: iCallAgent Public API Webhooks API
  slug: icallagent-public-api-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icallagent-public-api/refs/heads/main/openapi/icallagent-public-api-webhooks-api-openapi.yml
authorization_urls:
- /oauth/authorize/
description: ''
docs: https://docs.icallagent.com/api-reference/authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Icallagent Public Api Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'iCallAgent Public API publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the iCallAgent Public API API on a user''s behalf.


  Tokens are issued from /oauth/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: iCallAgent Public API
provider_slug: icallagent-public-api
schemes:
- description: OAuth2 access token from the consent flow third-party apps go through (see /oauth/authorize/). Interchangeable with a personal API key on every operation below — both are sent as a Bearer token in the same header.
  flows:
  - authorizationUrl: /oauth/authorize/
    flow: authorizationCode
    tokenUrl: /oauth/token/
  name: oauth2
  source: openapi/icallagent-public-api-openapi.json
scope_count: 3
scope_names:
- campaigns:read
- campaigns:write
- contacts:write
scopes:
- description: List your call campaigns
  flows:
  - authorizationCode
  scope: campaigns:read
- description: Create new call campaigns
  flows:
  - authorizationCode
  scope: campaigns:write
- description: Create contacts and queue calls into your campaigns
  flows:
  - authorizationCode
  scope: contacts:write
slug: icallagent-public-api-scopes
source_filename: icallagent-public-api-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-15'\nmethod: searched\nsource: openapi/icallagent-public-api-openapi.json\ndocs: https://docs.icallagent.com/api-reference/authentication\nschemes:\n- name: oauth2\n  source: openapi/icallagent-public-api-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /oauth/authorize/\n    tokenUrl: /oauth/token/\n  description: OAuth2 access token from the consent flow third-party apps go through (see /oauth/authorize/).\n    Interchangeable with a personal API key on every operation below — both are sent as a Bearer\n    token in the same header.\nscopes:\n- scope: campaigns:read\n  description: List your call campaigns\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/icallagent-public-api-openapi.json\n- scope: campaigns:write\n  description: Create new call campaigns\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/icallagent-public-api-openapi.json\n- scope: contacts:write\n  description: Create contacts and queue calls\
  \ into your campaigns\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/icallagent-public-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/icallagent-public-api/refs/heads/main/scopes/icallagent-public-api-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Voice AI
- voice ai assistant
- Conversational AI
- Voice Agents
- telephony / CPaaS
- contact center / CCaaS
- Outbound Calling
- speech (ASR/TTS)
- agent tools / MCP
token_urls:
- /oauth/token/
---
