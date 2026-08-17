---
api_specs:
- filename: sendpulse-bulk-email-openapi.yml
  format: yaml
  label: SendPulse Bulk Email API
  slug: sendpulse-bulk-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-bulk-email-openapi.yml
- filename: sendpulse-smtp-openapi.yml
  format: yaml
  label: SendPulse SMTP API
  slug: sendpulse-smtp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-smtp-openapi.yml
- filename: sendpulse-sms-openapi.yml
  format: yaml
  label: SendPulse SMS API
  slug: sendpulse-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-sms-openapi.yml
- filename: sendpulse-crm-openapi.yml
  format: yaml
  label: SendPulse CRM Public API
  slug: sendpulse-crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-crm-openapi.yml
- filename: sendpulse-a360-openapi.yml
  format: yaml
  label: SendPulse Automation 360 API
  slug: sendpulse-a360-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-a360-openapi.yml
- filename: sendpulse-chatbots-openapi.yml
  format: yaml
  label: SendPulse Chatbots Service API
  slug: sendpulse-chatbots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-chatbots-openapi.yml
- filename: sendpulse-whatsapp-openapi.yml
  format: yaml
  label: SendPulse WhatsApp Chatbot API
  slug: sendpulse-whatsapp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-whatsapp-openapi.yml
- filename: sendpulse-telegram-openapi.yml
  format: yaml
  label: SendPulse Telegram Chatbot API
  slug: sendpulse-telegram-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-telegram-openapi.yml
- filename: sendpulse-facebook-openapi.yml
  format: yaml
  label: SendPulse Facebook Messenger Chatbot API
  slug: sendpulse-facebook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-facebook-openapi.yml
- filename: sendpulse-instagram-openapi.yml
  format: yaml
  label: SendPulse Instagram Chatbot API
  slug: sendpulse-instagram-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-instagram-openapi.yml
- filename: sendpulse-viber-chatbot-openapi.yml
  format: yaml
  label: SendPulse Viber Chatbot API
  slug: sendpulse-viber-chatbot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-viber-chatbot-openapi.yml
- filename: sendpulse-tiktok-openapi.yml
  format: yaml
  label: SendPulse TikTok Chatbot API
  slug: sendpulse-tiktok-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-tiktok-openapi.yml
- filename: sendpulse-live-chat-openapi.yml
  format: yaml
  label: SendPulse LiveChat API
  slug: sendpulse-live-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-live-chat-openapi.yml
- filename: sendpulse-web-push-openapi.yml
  format: yaml
  label: SendPulse Web Push API
  slug: sendpulse-web-push-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-web-push-openapi.yml
- filename: sendpulse-viber-openapi.yml
  format: yaml
  label: SendPulse Viber API
  slug: sendpulse-viber-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-viber-openapi.yml
- filename: sendpulse-verifier-openapi.yml
  format: yaml
  label: SendPulse Verifier API
  slug: sendpulse-verifier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-verifier-openapi.yml
- filename: sendpulse-edu-openapi.yml
  format: yaml
  label: SendPulse Education API
  slug: sendpulse-edu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-edu-openapi.yml
- filename: sendpulse-popups-openapi.yml
  format: yaml
  label: SendPulse Pop-up API
  slug: sendpulse-popups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-popups-openapi.yml
- filename: sendpulse-file-manager-openapi.yml
  format: yaml
  label: SendPulse File Manager API
  slug: sendpulse-file-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-file-manager-openapi.yml
authorization_urls: []
description: ''
docs: https://sendpulse.com/integrations/api
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Sendpulse Scopes
name_suffix: OAuth Scopes
note: SendPulse operates TWO distinct OAuth surfaces and only one of them has scopes at all. 1. The REST API (api.sendpulse.com) uses client_credentials and declares an EMPTY scopes object in all 19 published specs. There is no scope, permission or consent reference page — an API key or client-credentials token carries the full permissions of the account that issued it. Least-privilege is not expressible. 2. The remote MCP server (mcp.sendpulse.com) publishes RFC 8414 metadata advertising exactly one scope, "rest", which is coarse — a single scope granting the whole REST surface.
overview: 'SendPulse publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the SendPulse API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SendPulse
provider_slug: sendpulse
schemes: []
scope_count: 1
scope_names:
- rest
scopes:
- description: Access to the SendPulse REST API on behalf of the authorising account.
  flows: []
  scope: rest
slug: sendpulse-scopes
source_filename: sendpulse-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://mcp.sendpulse.com/.well-known/oauth-authorization-server (HTTP 200) + openapi/*.yml\ndocs: https://sendpulse.com/integrations/api\nnote: 'SendPulse operates TWO distinct OAuth surfaces and only one of them has scopes at all.\n\n  1. The REST API (api.sendpulse.com) uses client_credentials and declares an EMPTY scopes object in all 19 published\n  specs. There is no scope, permission or consent reference page — an API key or client-credentials token carries\n  the full permissions of the account that issued it. Least-privilege is not expressible.\n\n  2. The remote MCP server (mcp.sendpulse.com) publishes RFC 8414 metadata advertising exactly one scope, \"rest\",\n  which is coarse — a single scope granting the whole REST surface.'\nauthorization_servers:\n- name: SendPulse REST API\n  issuer: https://api.sendpulse.com\n  flow: clientCredentials\n  token_endpoint: https://api.sendpulse.com/oauth/access_token\n  scopes_declared:\
  \ 0\n  scopes: []\n  evidence: components.securitySchemes.oauth2.flows.clientCredentials.scopes == {} in all 19 specs under openapi/\n- name: SendPulse MCP Server\n  issuer: https://mcp.sendpulse.com\n  metadata: https://mcp.sendpulse.com/.well-known/oauth-authorization-server\n  http_status: 200\n  flows:\n  - authorization_code\n  - refresh_token\n  pkce:\n  - S256\n  - plain\n  dynamic_client_registration: https://mcp.sendpulse.com/oauth/register\n  scopes_declared: 1\n  scopes:\n  - scope: rest\n    description: Access to the SendPulse REST API on behalf of the authorising account. The only scope advertised;\n      it is not decomposed by service or by read/write.\n    source: scopes_supported in the RFC 8414 metadata\nscopes:\n- scope: rest\n  issuer: https://mcp.sendpulse.com\n  description: Access to the SendPulse REST API on behalf of the authorising account.\nscope_count: 1\ngaps:\n- No per-service or read/write scope decomposition anywhere.\n- The REST API has no scope model\
  \ at all — a leaked API key is a full-account credential.\n- No consent/permissions reference page is published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/scopes/sendpulse-scopes.yml
summary_line: 1 scope
tags:
- Marketing
- Marketing Automation
- Email
- Transactional Email
- SMS
- Web Push
- Chatbots
- CRM
- Multichannel
- Messaging
- Online Courses
- Pop-ups
- Email Verification
- MCP
- Agent Ready
token_urls: []
---
