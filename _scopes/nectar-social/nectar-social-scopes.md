---
authorization_urls:
- https://beta-api.nectarsocial.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Nectar Social Scopes
name_suffix: OAuth Scopes
note: Derived from the provider's own RFC 8414 OAuth 2.0 Authorization Server Metadata document, fetched anonymously. Nectar Social publishes no public OpenAPI and no public scopes reference page, so scopes_supported in the discovery document is the authoritative published scope vocabulary. Descriptions below are the plain reading of each scope string against the product surface Nectar Social markets; no scope, permission, or grouping has been invented.
overview: 'Nectar Social publishes 18 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Nectar Social API on a user''s behalf.


  Tokens are issued from https://beta-api.nectarsocial.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Nectar Social
provider_slug: nectar-social
schemes:
- dynamic_client_registration: https://beta-api.nectarsocial.com/oauth/register
  flows:
  - authorizationUrl: https://beta-api.nectarsocial.com/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://beta-api.nectarsocial.com/oauth/token
    tokenUrl: https://beta-api.nectarsocial.com/oauth/token
  name: OAuth2
  pkce:
    required_methods:
    - S256
  resource_indicators_supported: true
  revocation_endpoint: https://beta-api.nectarsocial.com/oauth/revoke
  source: https://beta-api.nectarsocial.com/.well-known/oauth-authorization-server
  type: oauth2
scope_count: 18
scope_names:
- analytics:read
- content:read
- community:read
- campaigns:read
- competitors:read
- social_listening:read
- inbox:read
- inbox_rule:trigger
- mention_content
- workspace:read
- emails:read
- emails:write
- phone_numbers:read
- phone_numbers:write
- custom_field_values:read
- custom_field_values:write
- webhooks:write
- webhooks:delete
scopes:
- description: Read performance analytics, KPI dashboards and post-level insights.
  flows:
  - authorizationCode
  scope: analytics:read
- description: Read social content/posts managed in the workspace.
  flows:
  - authorizationCode
  scope: content:read
- description: Read community management data.
  flows:
  - authorizationCode
  scope: community:read
- description: Read campaign records.
  flows:
  - authorizationCode
  scope: campaigns:read
- description: Read competitor tracking data.
  flows:
  - authorizationCode
  scope: competitors:read
- description: Read social listening / cross-channel monitoring data.
  flows:
  - authorizationCode
  scope: social_listening:read
- description: Read the social inbox (DMs, comments, mentions).
  flows:
  - authorizationCode
  scope: inbox:read
- description: Trigger an inbox automation rule.
  flows:
  - authorizationCode
  scope: inbox_rule:trigger
- description: Access mention content. Note the scope string carries no read/write suffix, unlike the other 17.
  flows:
  - authorizationCode
  scope: mention_content
- description: Read workspace metadata.
  flows:
  - authorizationCode
  scope: workspace:read
- description: Read contact email addresses.
  flows:
  - authorizationCode
  scope: emails:read
- description: Write contact email addresses.
  flows:
  - authorizationCode
  scope: emails:write
- description: Read contact phone numbers.
  flows:
  - authorizationCode
  scope: phone_numbers:read
- description: Write contact phone numbers.
  flows:
  - authorizationCode
  scope: phone_numbers:write
- description: Read custom field values on records.
  flows:
  - authorizationCode
  scope: custom_field_values:read
- description: Write custom field values on records.
  flows:
  - authorizationCode
  scope: custom_field_values:write
- description: Create or update webhook subscriptions.
  flows:
  - authorizationCode
  scope: webhooks:write
- description: Delete webhook subscriptions.
  flows:
  - authorizationCode
  scope: webhooks:delete
slug: nectar-social-scopes
source_filename: nectar-social-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://beta-api.nectarsocial.com/.well-known/oauth-authorization-server\nraw: well-known/nectar-social-oauth-authorization-server.json\nnote: >-\n  Derived from the provider's own RFC 8414 OAuth 2.0 Authorization Server Metadata document,\n  fetched anonymously. Nectar Social publishes no public OpenAPI and no public scopes reference\n  page, so scopes_supported in the discovery document is the authoritative published scope\n  vocabulary. Descriptions below are the plain reading of each scope string against the product\n  surface Nectar Social markets; no scope, permission, or grouping has been invented.\nschemes:\n- name: OAuth2\n  type: oauth2\n  source: https://beta-api.nectarsocial.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://beta-api.nectarsocial.com/oauth/authorize\n    tokenUrl: https://beta-api.nectarsocial.com/oauth/token\n    refreshUrl: https://beta-api.nectarsocial.com/oauth/token\n\
  \  pkce:\n    required_methods:\n    - S256\n  dynamic_client_registration: https://beta-api.nectarsocial.com/oauth/register\n  revocation_endpoint: https://beta-api.nectarsocial.com/oauth/revoke\n  resource_indicators_supported: true\nscope_count: 18\nscopes:\n- scope: analytics:read\n  description: Read performance analytics, KPI dashboards and post-level insights.\n  flows: [authorizationCode]\n  mcp_required: true\n- scope: content:read\n  description: Read social content/posts managed in the workspace.\n  flows: [authorizationCode]\n  mcp_required: true\n- scope: community:read\n  description: Read community management data.\n  flows: [authorizationCode]\n- scope: campaigns:read\n  description: Read campaign records.\n  flows: [authorizationCode]\n- scope: competitors:read\n  description: Read competitor tracking data.\n  flows: [authorizationCode]\n- scope: social_listening:read\n  description: Read social listening / cross-channel monitoring data.\n  flows: [authorizationCode]\n\
  - scope: inbox:read\n  description: Read the social inbox (DMs, comments, mentions).\n  flows: [authorizationCode]\n- scope: inbox_rule:trigger\n  description: Trigger an inbox automation rule.\n  flows: [authorizationCode]\n- scope: mention_content\n  description: Access mention content. Note the scope string carries no read/write suffix, unlike the other 17.\n  flows: [authorizationCode]\n- scope: workspace:read\n  description: Read workspace metadata.\n  flows: [authorizationCode]\n- scope: emails:read\n  description: Read contact email addresses.\n  flows: [authorizationCode]\n  pii: true\n- scope: emails:write\n  description: Write contact email addresses.\n  flows: [authorizationCode]\n  pii: true\n- scope: phone_numbers:read\n  description: Read contact phone numbers.\n  flows: [authorizationCode]\n  pii: true\n- scope: phone_numbers:write\n  description: Write contact phone numbers.\n  flows: [authorizationCode]\n  pii: true\n- scope: custom_field_values:read\n  description: Read\
  \ custom field values on records.\n  flows: [authorizationCode]\n- scope: custom_field_values:write\n  description: Write custom field values on records.\n  flows: [authorizationCode]\n- scope: webhooks:write\n  description: Create or update webhook subscriptions.\n  flows: [authorizationCode]\n- scope: webhooks:delete\n  description: Delete webhook subscriptions.\n  flows: [authorizationCode]\nobservations:\n  granularity: resource:action\n  read_write_split: 13 read/trigger-style scopes, 4 explicit write/delete scopes, 1 unsuffixed (mention_content)\n  pii_scopes: [emails:read, emails:write, phone_numbers:read, phone_numbers:write]\n  webhook_management: >-\n    webhooks:write and webhooks:delete are published, which means the API exposes webhook\n    subscription management. The event catalog itself is not public — see\n    asyncapi/nectar-social-webhooks.yml.\n  docs: null\n  docs_note: >-\n    No public scopes/permissions reference page was found. docs.nectarsocial.com 307-redirects\n\
  \    to https://app.nectarsocial.com/docs, a JS-rendered application shell that requires a login.\nx-evidence:\n  fetched: '2026-08-13'\n  url: https://beta-api.nectarsocial.com/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nectar-social/refs/heads/main/scopes/nectar-social-scopes.yml
summary_line: 18 scopes · authorizationCode
tags:
- Company
- AI
- Social Media
- Community Management
- Social Listening
- Influencer Marketing
- Customer Engagement
- Social Commerce
- MCP
- Agents
- OAuth
token_urls:
- https://beta-api.nectarsocial.com/oauth/token
---
