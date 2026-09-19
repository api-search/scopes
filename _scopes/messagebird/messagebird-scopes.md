---
api_specs:
- filename: messagebird-bird-api-openapi.yml
  format: yaml
  label: Bird API
  slug: bird-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-bird-api-openapi.yml
- filename: messagebird-available-numbers-api-openapi.yml
  format: yaml
  label: messagebird Available Numbers API
  slug: messagebird-available-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-available-numbers-api-openapi.yml
- filename: messagebird-balance-api-openapi.yml
  format: yaml
  label: messagebird Balance API
  slug: messagebird-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-balance-api-openapi.yml
- filename: messagebird-call-flows-api-openapi.yml
  format: yaml
  label: messagebird Call Flows API
  slug: messagebird-call-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-call-flows-api-openapi.yml
- filename: messagebird-calls-api-openapi.yml
  format: yaml
  label: messagebird Calls API
  slug: messagebird-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-calls-api-openapi.yml
- filename: messagebird-contacts-api-openapi.yml
  format: yaml
  label: messagebird Contacts API
  slug: messagebird-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-contacts-api-openapi.yml
- filename: messagebird-conversations-api-openapi.yml
  format: yaml
  label: messagebird Conversations API
  slug: messagebird-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-conversations-api-openapi.yml
- filename: messagebird-groups-api-openapi.yml
  format: yaml
  label: messagebird Groups API
  slug: messagebird-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-groups-api-openapi.yml
- filename: messagebird-hlr-api-openapi.yml
  format: yaml
  label: messagebird HLR API
  slug: messagebird-hlr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-hlr-api-openapi.yml
- filename: messagebird-legs-api-openapi.yml
  format: yaml
  label: messagebird Legs API
  slug: messagebird-legs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-legs-api-openapi.yml
- filename: messagebird-lookup-api-openapi.yml
  format: yaml
  label: messagebird Lookup API
  slug: messagebird-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-lookup-api-openapi.yml
- filename: messagebird-messages-api-openapi.yml
  format: yaml
  label: messagebird Messages API
  slug: messagebird-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-messages-api-openapi.yml
- filename: messagebird-purchased-numbers-api-openapi.yml
  format: yaml
  label: messagebird Purchased Numbers API
  slug: messagebird-purchased-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-purchased-numbers-api-openapi.yml
- filename: messagebird-recordings-api-openapi.yml
  format: yaml
  label: messagebird Recordings API
  slug: messagebird-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-recordings-api-openapi.yml
- filename: messagebird-templates-api-openapi.yml
  format: yaml
  label: messagebird Templates API
  slug: messagebird-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-templates-api-openapi.yml
- filename: messagebird-transcriptions-api-openapi.yml
  format: yaml
  label: messagebird Transcriptions API
  slug: messagebird-transcriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-transcriptions-api-openapi.yml
- filename: messagebird-verify-api-openapi.yml
  format: yaml
  label: messagebird Verify API
  slug: messagebird-verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-verify-api-openapi.yml
- filename: messagebird-voice-messages-api-openapi.yml
  format: yaml
  label: messagebird Voice Messages API
  slug: messagebird-voice-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-voice-messages-api-openapi.yml
- filename: messagebird-webhooks-api-openapi.yml
  format: yaml
  label: messagebird Webhooks API
  slug: messagebird-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-webhooks-api-openapi.yml
authorization_urls:
- https://platform.bird.com/v1/oauth/authorize
description: ''
docs: https://bird.com/auth.md
flows:
- authorizationCode
- deviceCode
- refreshToken
kind: oauth-scopes
layout: scope
method: searched
name: Messagebird Scopes
name_suffix: OAuth Scopes
note: Bird's OpenAPI declares no oauth2 securityScheme (the spec documents bearer API keys), so derive-oauth-scopes.py found nothing. The scope surface is real and machine-readable — it is published in the RFC 8414 authorization server metadata at platform.bird.com and mirrored in the RFC 9728 protected-resource document. Every scope below is verbatim from that document. Scopes are resource:level pairs; :write implies the write level on the named resource and org:* scopes act at the organization rather than the workspace.
overview: 'Messagebird publishes 44 OAuth 2.0 scopes via the authorizationCode, deviceCode, and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Messagebird API on a user''s behalf.


  Tokens are issued from https://platform.bird.com/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Messagebird
provider_slug: messagebird
schemes:
- flows:
  - authorizationUrl: https://platform.bird.com/v1/oauth/authorize
    flow: authorizationCode
    pkce: S256 (required for public clients; plain not supported)
    tokenUrl: https://platform.bird.com/v1/oauth/token
  - deviceAuthorizationUrl: https://platform.bird.com/v1/oauth/device
    flow: deviceCode
    tokenUrl: https://platform.bird.com/v1/oauth/token
  - flow: refreshToken
    note: Refresh tokens rotate on every use; reuse of a rotated token revokes the grant family.
  name: BirdOAuth2
  not_supported:
  - client_credentials
  - assertion grants
  registration: RFC 7591 dynamic client registration, open to agents with no pre-issued client
  registrationUrl: https://platform.bird.com/v1/oauth/register
  revocationUrl: https://platform.bird.com/v1/oauth/revoke
  source: https://platform.bird.com/.well-known/oauth-authorization-server
scope_count: 44
scope_names:
- amb:write
- amb_management:write
- analytics:write
- api_keys:write
- assets:write
- audit:write
- competitive:write
- compliance:write
- domains:write
- email_management:write
- email_marketing:write
- emails:write
- esim:write
- esim_credentials:write
- inbox_insights:write
- ip_pools:write
- lookup:write
- mailbox:write
- mailbox_management:write
- members:write
- numbers:write
- preferences:write
- realtime:write
- request_logs:write
- service_accounts:write
- sms:write
- sms_management:write
- trust:write
- verify:write
- verify_management:write
- voice:write
- voice_management:write
- webhooks:write
- whatsapp:write
- whatsapp_management:write
- workspace:write
- org:access_restrictions:write
- org:audit:write
- org:billing:write
- org:ip_pools:write
- org:members:write
- org:settings:write
- org:trust:write
- org:workspaces:write
scopes:
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: amb:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: amb_management:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: analytics:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: api_keys:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: assets:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: audit:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: competitive:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: compliance:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: domains:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: email_management:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: email_marketing:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: emails:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: esim:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: esim_credentials:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: inbox_insights:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: ip_pools:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: lookup:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: mailbox:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: mailbox_management:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: members:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: numbers:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: preferences:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: realtime:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: request_logs:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: service_accounts:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: sms:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: sms_management:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: trust:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: verify:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: verify_management:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: voice:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: voice_management:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: webhooks:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: whatsapp:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: whatsapp_management:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: workspace:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: org:access_restrictions:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: org:audit:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: org:billing:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: org:ip_pools:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: org:members:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: org:settings:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: org:trust:write
- description: ''
  flows:
  - authorizationCode
  - deviceCode
  scope: org:workspaces:write
slug: messagebird-scopes
source_filename: messagebird-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: https://platform.bird.com/.well-known/oauth-authorization-server\ndocs: https://bird.com/auth.md\nnote: >-\n  Bird's OpenAPI declares no oauth2 securityScheme (the spec documents bearer API keys), so\n  derive-oauth-scopes.py found nothing. The scope surface is real and machine-readable — it\n  is published in the RFC 8414 authorization server metadata at platform.bird.com and\n  mirrored in the RFC 9728 protected-resource document. Every scope below is verbatim from\n  that document. Scopes are resource:level pairs; :write implies the write level on the\n  named resource and org:* scopes act at the organization rather than the workspace.\nissuer: https://platform.bird.com\nschemes:\n- name: BirdOAuth2\n  source: https://platform.bird.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://platform.bird.com/v1/oauth/authorize\n    tokenUrl: https://platform.bird.com/v1/oauth/token\n\
  \    pkce: S256 (required for public clients; plain not supported)\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://platform.bird.com/v1/oauth/device\n    tokenUrl: https://platform.bird.com/v1/oauth/token\n  - flow: refreshToken\n    note: Refresh tokens rotate on every use; reuse of a rotated token revokes the grant family.\n  revocationUrl: https://platform.bird.com/v1/oauth/revoke\n  registrationUrl: https://platform.bird.com/v1/oauth/register\n  registration: RFC 7591 dynamic client registration, open to agents with no pre-issued client\n  not_supported: [client_credentials, assertion grants]\nscope_count: 44\nscopes:\n- scope: amb:write\n  resource: amb\n  level: write\n  tier: workspace\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n- scope: amb_management:write\n  resource: amb_management\n  level: write\n  tier: workspace\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n\
  - scope: analytics:write\n  resource: analytics\n  level: write\n  tier: workspace\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n- scope: api_keys:write\n  resource: api_keys\n  level: write\n  tier: workspace\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n- scope: assets:write\n  resource: assets\n  level: write\n  tier: workspace\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n- scope: audit:write\n  resource: audit\n  level: write\n  tier: workspace\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n- scope: competitive:write\n  resource: competitive\n  level: write\n  tier: workspace\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n\
  - scope: compliance:write\n  resource: compliance\n  level: write\n  tier: workspace\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n- scope: domains:write\n  resource: domains\n  level: write\n  tier: workspace\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n- scope: email_management:write\n  resource: email_management\n  level: write\n  tier: workspace\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n- scope: email_marketing:write\n  resource: email_marketing\n  level: write\n  tier: workspace\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n- scope: emails:write\n  resource: emails\n  level: write\n  tier: workspace\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n\
  - scope: esim:write\n  resource: esim\n  level: write\n  tier: workspace\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n- scope: esim_credentials:write\n  resource: esim_credentials\n  level: write\n  tier: workspace\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n- scope: inbox_insights:write\n  resource: inbox_insights\n  level: write\n  tier: workspace\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n- scope: ip_pools:write\n  resource: ip_pools\n  level: write\n  tier: workspace\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n- scope: lookup:write\n  resource: lookup\n  level: write\n  tier: workspace\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n\
  - scope: mailbox:write\n  resource: mailbox\n  level: write\n  tier: workspace\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n- scope: mailbox_management:write\n  resource: mailbox_management\n  level: write\n  tier: workspace\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n- scope: members:write\n  resource: members\n  level: write\n  tier: workspace\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n- scope: numbers:write\n  resource: numbers\n  level: write\n  tier: workspace\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n- scope: preferences:write\n  resource: preferences\n  level: write\n  tier: workspace\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n\
  - scope: realtime:write\n  resource: realtime\n  level: write\n  tier: workspace\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n- scope: request_logs:write\n  resource: request_logs\n  level: write\n  tier: workspace\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n- scope: service_accounts:write\n  resource: service_accounts\n  level: write\n  tier: workspace\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n- scope: sms:write\n  resource: sms\n  level: write\n  tier: workspace\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n- scope: sms_management:write\n  resource: sms_management\n  level: write\n  tier: workspace\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n\
  - scope: trust:write\n  resource: trust\n  level: write\n  tier: workspace\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n- scope: verify:write\n  resource: verify\n  level: write\n  tier: workspace\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n- scope: verify_management:write\n  resource: verify_management\n  level: write\n  tier: workspace\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n- scope: voice:write\n  resource: voice\n  level: write\n  tier: workspace\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n- scope: voice_management:write\n  resource: voice_management\n  level: write\n  tier: workspace\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n\
  - scope: webhooks:write\n  resource: webhooks\n  level: write\n  tier: workspace\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n- scope: whatsapp:write\n  resource: whatsapp\n  level: write\n  tier: workspace\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n- scope: whatsapp_management:write\n  resource: whatsapp_management\n  level: write\n  tier: workspace\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n- scope: workspace:write\n  resource: workspace\n  level: write\n  tier: workspace\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n- scope: org:access_restrictions:write\n  resource: org:access_restrictions\n  level: write\n  tier: organization\n  flows: [authorizationCode, deviceCode]\n  sources:\
  \ [https://platform.bird.com/.well-known/oauth-authorization-server]\n- scope: org:audit:write\n  resource: org:audit\n  level: write\n  tier: organization\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n- scope: org:billing:write\n  resource: org:billing\n  level: write\n  tier: organization\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n- scope: org:ip_pools:write\n  resource: org:ip_pools\n  level: write\n  tier: organization\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n- scope: org:members:write\n  resource: org:members\n  level: write\n  tier: organization\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n- scope: org:settings:write\n  resource: org:settings\n  level: write\n  tier: organization\n\
  \  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n- scope: org:trust:write\n  resource: org:trust\n  level: write\n  tier: organization\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n- scope: org:workspaces:write\n  resource: org:workspaces\n  level: write\n  tier: organization\n  flows: [authorizationCode, deviceCode]\n  sources: [https://platform.bird.com/.well-known/oauth-authorization-server]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/scopes/messagebird-scopes.yml
summary_line: 44 scopes · authorizationCode/deviceCode/refreshToken
tags:
- Communications
- Messaging
- SMS
- Email
- WhatsApp
- Voice
- Verification
- CPaaS
- Webhook
- Agents
token_urls:
- https://platform.bird.com/v1/oauth/token
---
