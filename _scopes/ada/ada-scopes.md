---
api_specs:
- filename: ada-conversations-api-openapi.yml
  format: yaml
  label: Ada Conversations API
  slug: ada-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-conversations-api-openapi.yml
- filename: ada-auditlog-api-openapi.yml
  format: yaml
  label: Ada Audit Log API
  slug: ada-auditlog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-auditlog-api-openapi.yml
- filename: ada-channels-api-openapi.yml
  format: yaml
  label: Ada Channels API
  slug: ada-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-channels-api-openapi.yml
- filename: ada-conversations-api-openapi.yml
  format: yaml
  label: Ada Conversations API
  slug: ada-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-conversations-api-openapi.yml
- filename: ada-custominstructions-api-openapi.yml
  format: yaml
  label: Ada Custom Instructions API
  slug: ada-custominstructions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-custominstructions-api-openapi.yml
- filename: ada-deletechatterdata-api-openapi.yml
  format: yaml
  label: Ada Delete Chatter Data API
  slug: ada-deletechatterdata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-deletechatterdata-api-openapi.yml
- filename: ada-endusers-api-openapi.yml
  format: yaml
  label: Ada End Users API
  slug: ada-endusers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-endusers-api-openapi.yml
- filename: ada-getdeletionjob-api-openapi.yml
  format: yaml
  label: Ada Get Deletion Job API
  slug: ada-getdeletionjob-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-getdeletionjob-api-openapi.yml
- filename: ada-knowledge-api-openapi.yml
  format: yaml
  label: Ada Knowledge API
  slug: ada-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-knowledge-api-openapi.yml
- filename: ada-knowledge-articles-api-openapi.yml
  format: yaml
  label: Ada knowledge > articles API
  slug: ada-knowledge-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-knowledge-articles-api-openapi.yml
- filename: ada-knowledge-sources-api-openapi.yml
  format: yaml
  label: Ada knowledge > sources API
  slug: ada-knowledge-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-knowledge-sources-api-openapi.yml
- filename: ada-knowledge-tags-api-openapi.yml
  format: yaml
  label: Ada knowledge > tags API
  slug: ada-knowledge-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-knowledge-tags-api-openapi.yml
- filename: ada-messages-api-openapi.yml
  format: yaml
  label: Ada Messages API
  slug: ada-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-messages-api-openapi.yml
- filename: ada-persona-api-openapi.yml
  format: yaml
  label: Ada Persona API
  slug: ada-persona-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-persona-api-openapi.yml
- filename: ada-platformintegrations-api-openapi.yml
  format: yaml
  label: Ada Platform Integrations API
  slug: ada-platformintegrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-platformintegrations-api-openapi.yml
- filename: ada-submitdeletionrequest-api-openapi.yml
  format: yaml
  label: Ada Submit Deletion Request API
  slug: ada-submitdeletionrequest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-submitdeletionrequest-api-openapi.yml
- filename: ada-variables-api-openapi.yml
  format: yaml
  label: Ada Variables API
  slug: ada-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-variables-api-openapi.yml
- filename: ada-webhookmanagement-api-openapi.yml
  format: yaml
  label: Ada Webhook Management API
  slug: ada-webhookmanagement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-webhookmanagement-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.ada.cx/reference/integrations/getting-started
flows:
- authorizationCode
- refreshToken
kind: oauth-scopes
layout: scope
method: searched
name: Ada Scopes
name_suffix: OAuth Scopes
note: None of Ada's four published OpenAPI documents declares an oauth2 securityScheme — every spec declares only http/bearer. The OAuth surface exists solely for the Integrations API (partner apps installed into a customer's AI Agent) and is documented in prose, not in the machine- readable contract. This artifact is therefore SEARCHED from the docs, not derived from a spec; derive-oauth-scopes.py correctly found zero.
overview: 'Ada publishes 8 OAuth 2.0 scopes via the authorizationCode and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Ada API on a user''s behalf.


  Tokens are issued from https://{bot-handle}.ada.support/api/platform_integrations/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Ada
provider_slug: ada
schemes:
- flows:
  - authorizationUrl: null
    authorization_note: The authorization step is initiated from the Ada dashboard, which redirects the AI Agent Manager to the partner's own oauth_callback_url. Ada does not publish a fixed /authorize URL.
    flow: authorizationCode
    refreshUrl: https://{bot-handle}.ada.support/api/platform_integrations/oauth/token
    tokenUrl: https://{bot-handle}.ada.support/api/platform_integrations/oauth/token
  - flow: refreshToken
    tokenUrl: https://{bot-handle}.ada.support/api/platform_integrations/oauth/token
  in_openapi: false
  installation_lookup: https://{bot-handle}.ada.support/api/platform_integrations/oauth/self
  name: PlatformIntegrationsOAuth
  refresh_rotation: true
  refresh_rotation_note: '"The Ada authorization server issues a new refresh token each time one is used as a security best practice." Callers must overwrite the stored refresh token on every exchange.'
  registration:
    auth: Ada API key (Bearer) from the development AI Agent
    endpoint: POST https://{bot-handle}.ada.support/api/v2/platform-integrations
    fields:
    - oauth_callback_url
    - scopes
    returns:
    - id
    - client_secret
  source: https://docs.ada.cx/reference/integrations/getting-started
  token_lifetimes:
    access_token: 1 hour
    authorization_code: 5 minutes
    refresh_token: 30 days
  type: oauth2
scope_count: 8
scope_names:
- articles:read
- articles:write
- article_tags:read
- article_tags:write
- knowledge_sources:read
- knowledge_sources:write
- platform_integration_installations:read
- platform_integration_installations:write
scopes:
- description: Read knowledge articles.
  flows:
  - authorizationCode
  scope: articles:read
- description: Create, update and delete knowledge articles.
  flows:
  - authorizationCode
  scope: articles:write
- description: Read knowledge article tags.
  flows:
  - authorizationCode
  scope: article_tags:read
- description: Create, update and delete knowledge article tags.
  flows:
  - authorizationCode
  scope: article_tags:write
- description: Read knowledge sources.
  flows:
  - authorizationCode
  scope: knowledge_sources:read
- description: Create, update and delete knowledge sources.
  flows:
  - authorizationCode
  scope: knowledge_sources:write
- description: Read the integration's own installation records.
  flows:
  - authorizationCode
  scope: platform_integration_installations:read
- description: Update the integration's own installation status (e.g. mark it `complete`).
  flows:
  - authorizationCode
  scope: platform_integration_installations:write
slug: ada-scopes
source_filename: ada-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://docs.ada.cx/reference/integrations/getting-started\ndocs: https://docs.ada.cx/reference/integrations/getting-started\noverview: https://docs.ada.cx/reference/integrations/overview\nnote: >-\n  None of Ada's four published OpenAPI documents declares an oauth2 securityScheme — every spec\n  declares only http/bearer. The OAuth surface exists solely for the Integrations API (partner\n  apps installed into a customer's AI Agent) and is documented in prose, not in the machine-\n  readable contract. This artifact is therefore SEARCHED from the docs, not derived from a spec;\n  derive-oauth-scopes.py correctly found zero.\nschemes:\n- name: PlatformIntegrationsOAuth\n  type: oauth2\n  source: https://docs.ada.cx/reference/integrations/getting-started\n  in_openapi: false\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: null\n    authorization_note: >-\n      The authorization step is initiated from the Ada dashboard,\
  \ which redirects the AI Agent\n      Manager to the partner's own oauth_callback_url. Ada does not publish a fixed /authorize URL.\n    tokenUrl: https://{bot-handle}.ada.support/api/platform_integrations/oauth/token\n    refreshUrl: https://{bot-handle}.ada.support/api/platform_integrations/oauth/token\n  - flow: refreshToken\n    tokenUrl: https://{bot-handle}.ada.support/api/platform_integrations/oauth/token\n  token_lifetimes:\n    authorization_code: 5 minutes\n    access_token: 1 hour\n    refresh_token: 30 days\n  refresh_rotation: true\n  refresh_rotation_note: >-\n    \"The Ada authorization server issues a new refresh token each time one is used as a security\n    best practice.\" Callers must overwrite the stored refresh token on every exchange.\n  installation_lookup: https://{bot-handle}.ada.support/api/platform_integrations/oauth/self\n  registration:\n    endpoint: POST https://{bot-handle}.ada.support/api/v2/platform-integrations\n    auth: Ada API key (Bearer) from the\
  \ development AI Agent\n    returns:\n    - id\n    - client_secret\n    fields:\n    - oauth_callback_url\n    - scopes\nscopes:\n- scope: articles:read\n  description: Read knowledge articles.\n  flows:\n  - authorizationCode\n  sources:\n  - https://docs.ada.cx/reference/integrations/getting-started\n- scope: articles:write\n  description: Create, update and delete knowledge articles.\n  flows:\n  - authorizationCode\n  sources:\n  - https://docs.ada.cx/reference/integrations/getting-started\n- scope: article_tags:read\n  description: Read knowledge article tags.\n  flows:\n  - authorizationCode\n  sources:\n  - https://docs.ada.cx/reference/integrations/getting-started\n- scope: article_tags:write\n  description: Create, update and delete knowledge article tags.\n  flows:\n  - authorizationCode\n  sources:\n  - https://docs.ada.cx/reference/integrations/getting-started\n- scope: knowledge_sources:read\n  description: Read knowledge sources.\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - https://docs.ada.cx/reference/integrations/getting-started\n- scope: knowledge_sources:write\n  description: Create, update and delete knowledge sources.\n  flows:\n  - authorizationCode\n  sources:\n  - https://docs.ada.cx/reference/integrations/getting-started\n- scope: platform_integration_installations:read\n  description: Read the integration's own installation records.\n  always_granted: true\n  note: Granted implicitly even when omitted from the `scopes` field at registration.\n  flows:\n  - authorizationCode\n  sources:\n  - https://docs.ada.cx/reference/integrations/getting-started\n- scope: platform_integration_installations:write\n  description: Update the integration's own installation status (e.g. mark it `complete`).\n  always_granted: true\n  note: Granted implicitly even when omitted from the `scopes` field at registration.\n  flows:\n  - authorizationCode\n  sources:\n  - https://docs.ada.cx/reference/integrations/getting-started\nscope_count: 8\ncoverage:\n  note:\
  \ >-\n    Ada states \"More scopes will become available as more APIs become available.\" Today the OAuth\n    scope vocabulary covers Knowledge and the integration's own installation record ONLY — end\n    users, conversations, channels, webhooks, persona, variables, custom instructions and the\n    audit log are reachable with an API key but have no OAuth scope, so a partner integration\n    cannot be granted access to them.\nmcp_authorization:\n  note: >-\n    The Ada MCP server also supports OAuth (https://<instance>/api/mcp/oauth) but does NOT use\n    these scopes. MCP access is governed by the connected user's Ada dashboard role\n    (Owner/Admin = writes, Agent/Read Only = reads). See mcp/ada-mcp.yml.\n  source: https://docs.ada.cx/mcp/introduction/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/scopes/ada-scopes.yml
summary_line: 8 scopes · authorizationCode/refreshToken
tags:
- Artificial Intelligence
- Customer Service
- Chatbots
- Automation
- Conversational AI
- Help Desk
- CRM
- Integration
- Knowledge-Management
- Data Export
token_urls:
- https://{bot-handle}.ada.support/api/platform_integrations/oauth/token
---
