---
api_specs:
- filename: mailersend-bulk-email-api-openapi.yml
  format: yaml
  label: MailerSend Bulk Email API
  slug: mailersend-bulk-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailersend/refs/heads/main/openapi/mailersend-bulk-email-api-openapi.yml
- filename: mailersend-domains-api-openapi.yml
  format: yaml
  label: MailerSend Domains API
  slug: mailersend-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailersend/refs/heads/main/openapi/mailersend-domains-api-openapi.yml
- filename: mailersend-email-api-openapi.yml
  format: yaml
  label: MailerSend Email API
  slug: mailersend-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailersend/refs/heads/main/openapi/mailersend-email-api-openapi.yml
- filename: mailersend-messages-api-openapi.yml
  format: yaml
  label: MailerSend Messages API
  slug: mailersend-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailersend/refs/heads/main/openapi/mailersend-messages-api-openapi.yml
- filename: mailersend-sender-identities-api-openapi.yml
  format: yaml
  label: MailerSend Sender Identities API
  slug: mailersend-sender-identities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailersend/refs/heads/main/openapi/mailersend-sender-identities-api-openapi.yml
- filename: mailersend-templates-api-openapi.yml
  format: yaml
  label: MailerSend Templates API
  slug: mailersend-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailersend/refs/heads/main/openapi/mailersend-templates-api-openapi.yml
- filename: mailersend-webhooks-api-openapi.yml
  format: yaml
  label: MailerSend Webhooks API
  slug: mailersend-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailersend/refs/heads/main/openapi/mailersend-webhooks-api-openapi.yml
authorization_urls: []
description: ''
docs: https://developers.mailersend.com/api/v1/account/tokens#possible-scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Mailersend Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'MailerSend publishes 30 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the MailerSend API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: MailerSend
provider_slug: mailersend
schemes:
- assignment: POST /v1/token with a scopes[] array
  enforcement_error: MS40301
  issued_per: sending domain
  name: APIToken
  source: https://developers.mailersend.com/api/v1/account/tokens
  type: apiKey-scoped
- authorizationUrl: https://mcp.mailersend.com/authorize
  code_challenge_methods:
  - S256
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://mcp.mailersend.com
  name: MCPOAuth
  note: The authorization-server metadata document omits scopes_supported; the granted scope set cannot be enumerated without completing an authorization flow. Recorded as unknown rather than guessed.
  registrationUrl: https://mcp.mailersend.com/register
  scopes_supported: null
  source: https://mcp.mailersend.com/.well-known/oauth-authorization-server
  tokenUrl: https://mcp.mailersend.com/token
  type: oauth2
scope_count: 30
scope_names:
- email_full
- domains_read
- domains_full
- activity_read
- activity_full
- analytics_read
- analytics_full
- tokens_full
- webhooks_full
- templates_full
- suppressions_read
- suppressions_full
- sms_read
- sms_full
- email_verification_read
- email_verification_full
- inbounds_full
- recipients_read
- recipients_full
- sender_identity_read
- sender_identity_full
- users_read
- users_full
- smtp_users_read
- smtp_users_full
- dmarc_monitoring_read
- dmarc_monitoring_full
- blocklist_monitoring_read
- blocklist_monitoring_full
- whatsapp_full
scopes:
- description: Full access to the email sending endpoints.
  flows: []
  scope: email_full
- description: Read sending domains.
  flows: []
  scope: domains_read
- description: Read and manage sending domains.
  flows: []
  scope: domains_full
- description: Read email activity.
  flows: []
  scope: activity_read
- description: Read and manage email activity.
  flows: []
  scope: activity_full
- description: Read email analytics.
  flows: []
  scope: analytics_read
- description: Read and manage email analytics.
  flows: []
  scope: analytics_full
- description: Read and manage API tokens.
  flows: []
  scope: tokens_full
- description: Read and manage webhooks.
  flows: []
  scope: webhooks_full
- description: Read and manage email templates.
  flows: []
  scope: templates_full
- description: Read suppression lists.
  flows: []
  scope: suppressions_read
- description: Read and manage suppression lists.
  flows: []
  scope: suppressions_full
- description: Read SMS resources.
  flows: []
  scope: sms_read
- description: Read and manage SMS resources.
  flows: []
  scope: sms_full
- description: Read email verification lists and results.
  flows: []
  scope: email_verification_read
- description: Read and manage email verification.
  flows: []
  scope: email_verification_full
- description: Read and manage inbound routes.
  flows: []
  scope: inbounds_full
- description: Read recipients.
  flows: []
  scope: recipients_read
- description: Read and manage recipients.
  flows: []
  scope: recipients_full
- description: Read sender identities.
  flows: []
  scope: sender_identity_read
- description: Read and manage sender identities.
  flows: []
  scope: sender_identity_full
- description: Read account users.
  flows: []
  scope: users_read
- description: Read and manage account users.
  flows: []
  scope: users_full
- description: Read SMTP users.
  flows: []
  scope: smtp_users_read
- description: Read and manage SMTP users.
  flows: []
  scope: smtp_users_full
- description: Read DMARC monitors and reports.
  flows: []
  scope: dmarc_monitoring_read
- description: Read and manage DMARC monitoring.
  flows: []
  scope: dmarc_monitoring_full
- description: Read blocklist monitors.
  flows: []
  scope: blocklist_monitoring_read
- description: Read and manage blocklist monitoring.
  flows: []
  scope: blocklist_monitoring_full
- description: Full access to WhatsApp messaging resources.
  flows: []
  scope: whatsapp_full
slug: mailersend-scopes
source_filename: mailersend-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developers.mailersend.com/api/v1/account/tokens\ndocs: https://developers.mailersend.com/api/v1/account/tokens#possible-scopes\nnotes: >-\n  MailerSend has two separate authorization surfaces and they do not share a scope vocabulary.\n  (1) The REST API uses long-lived API tokens issued per sending domain, each carrying an explicit list\n  from the fixed scope vocabulary below — that list is set at POST /v1/token time and is the permission\n  boundary for every request made with the token. A request outside the token's scopes returns MS40301.\n  (2) The MCP server at mcp.mailersend.com is a real OAuth 2.1 authorization server (RFC 8414 metadata,\n  dynamic client registration, PKCE S256) but publishes no `scopes_supported` in its metadata, so its\n  scope vocabulary is not discoverable anonymously.\n  derive-oauth-scopes.py found no oauth2 securityScheme in the captured OpenAPI, which is correct — the\n  REST API is\
  \ bearer-token, not OAuth. This artifact is searched, not derived.\nschemes:\n  - name: APIToken\n    type: apiKey-scoped\n    source: https://developers.mailersend.com/api/v1/account/tokens\n    issued_per: sending domain\n    assignment: 'POST /v1/token with a scopes[] array'\n    enforcement_error: MS40301\n  - name: MCPOAuth\n    type: oauth2\n    source: https://mcp.mailersend.com/.well-known/oauth-authorization-server\n    issuer: https://mcp.mailersend.com\n    authorizationUrl: https://mcp.mailersend.com/authorize\n    tokenUrl: https://mcp.mailersend.com/token\n    registrationUrl: https://mcp.mailersend.com/register\n    grant_types: [authorization_code, refresh_token]\n    code_challenge_methods: [S256]\n    scopes_supported: null\n    note: >-\n      The authorization-server metadata document omits scopes_supported; the granted scope set cannot be\n      enumerated without completing an authorization flow. Recorded as unknown rather than guessed.\nscope_count: 30\nscopes:\n\
  \  - {scope: email_full, surface: api-token, description: Full access to the email sending endpoints.}\n  - {scope: domains_read, surface: api-token, description: Read sending domains.}\n  - {scope: domains_full, surface: api-token, description: Read and manage sending domains.}\n  - {scope: activity_read, surface: api-token, description: Read email activity.}\n  - {scope: activity_full, surface: api-token, description: Read and manage email activity.}\n  - {scope: analytics_read, surface: api-token, description: Read email analytics.}\n  - {scope: analytics_full, surface: api-token, description: Read and manage email analytics.}\n  - {scope: tokens_full, surface: api-token, description: Read and manage API tokens.}\n  - {scope: webhooks_full, surface: api-token, description: Read and manage webhooks.}\n  - {scope: templates_full, surface: api-token, description: Read and manage email templates.}\n  - {scope: suppressions_read, surface: api-token, description: Read suppression lists.}\n\
  \  - {scope: suppressions_full, surface: api-token, description: Read and manage suppression lists.}\n  - {scope: sms_read, surface: api-token, description: Read SMS resources.}\n  - {scope: sms_full, surface: api-token, description: Read and manage SMS resources.}\n  - {scope: email_verification_read, surface: api-token, description: Read email verification lists and results.}\n  - {scope: email_verification_full, surface: api-token, description: Read and manage email verification.}\n  - {scope: inbounds_full, surface: api-token, description: Read and manage inbound routes.}\n  - {scope: recipients_read, surface: api-token, description: Read recipients.}\n  - {scope: recipients_full, surface: api-token, description: Read and manage recipients.}\n  - {scope: sender_identity_read, surface: api-token, description: Read sender identities.}\n  - {scope: sender_identity_full, surface: api-token, description: Read and manage sender identities.}\n  - {scope: users_read, surface: api-token, description:\
  \ Read account users.}\n  - {scope: users_full, surface: api-token, description: Read and manage account users.}\n  - {scope: smtp_users_read, surface: api-token, description: Read SMTP users.}\n  - {scope: smtp_users_full, surface: api-token, description: Read and manage SMTP users.}\n  - {scope: dmarc_monitoring_read, surface: api-token, description: Read DMARC monitors and reports.}\n  - {scope: dmarc_monitoring_full, surface: api-token, description: Read and manage DMARC monitoring.}\n  - {scope: blocklist_monitoring_read, surface: api-token, description: Read blocklist monitors.}\n  - {scope: blocklist_monitoring_full, surface: api-token, description: Read and manage blocklist monitoring.}\n  - {scope: whatsapp_full, surface: api-token, description: Full access to WhatsApp messaging resources.}\npattern:\n  shape: '<resource>_read | <resource>_full'\n  note: >-\n    A clean two-level read/full split per resource domain. Note the asymmetry: email, tokens, webhooks,\n    templates,\
  \ inbounds and whatsapp expose only `_full` — there is no read-only scope for sending, for\n    template access, or for token introspection, so a least-privilege agent cannot be given read-only\n    visibility into those domains.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mailersend/refs/heads/main/scopes/mailersend-scopes.yml
summary_line: 30 scopes
tags:
- Email
- Transactional Email
- SMTP
- Marketing
- Communications
- SMS
- Messaging
- Templates
- Webhooks
- Email Verification
- Deliverability
- Analytics
- MCP
token_urls: []
---
