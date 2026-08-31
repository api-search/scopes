---
api_specs:
- filename: lemlist-campaigns-api-openapi.yml
  format: yaml
  label: lemlist Campaigns API
  slug: lemlist-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-campaigns-api-openapi.yml
- filename: lemlist-sequences-api-openapi.yml
  format: yaml
  label: lemlist Sequences API
  slug: lemlist-sequences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-sequences-api-openapi.yml
- filename: lemlist-leads-api-openapi.yml
  format: yaml
  label: lemlist Leads API
  slug: lemlist-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-leads-api-openapi.yml
- filename: lemlist-people-database-api-openapi.yml
  format: yaml
  label: lemlist People Database API
  slug: lemlist-people-database-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-people-database-api-openapi.yml
- filename: lemlist-enrich-api-openapi.yml
  format: yaml
  label: lemlist Enrich API
  slug: lemlist-enrich-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-enrich-api-openapi.yml
- filename: lemlist-inbox-api-openapi.yml
  format: yaml
  label: lemlist Inbox API
  slug: lemlist-inbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-inbox-api-openapi.yml
- filename: lemlist-contacts-api-openapi.yml
  format: yaml
  label: lemlist Contacts API
  slug: lemlist-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-contacts-api-openapi.yml
- filename: lemlist-companies-api-openapi.yml
  format: yaml
  label: lemlist Companies API
  slug: lemlist-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-companies-api-openapi.yml
- filename: lemlist-signal-agents-api-openapi.yml
  format: yaml
  label: lemlist Signal Agents API
  slug: lemlist-signal-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-signal-agents-api-openapi.yml
- filename: lemlist-webhooks-api-openapi.yml
  format: yaml
  label: lemlist Webhooks API
  slug: lemlist-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-webhooks-api-openapi.yml
- filename: lemlist-unsubscribes-api-openapi.yml
  format: yaml
  label: lemlist Unsubscribes API
  slug: lemlist-unsubscribes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-unsubscribes-api-openapi.yml
- filename: lemlist-schedules-api-openapi.yml
  format: yaml
  label: lemlist Schedules API
  slug: lemlist-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-schedules-api-openapi.yml
- filename: lemlist-tasks-api-openapi.yml
  format: yaml
  label: lemlist Tasks API
  slug: lemlist-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-tasks-api-openapi.yml
- filename: lemlist-activities-api-openapi.yml
  format: yaml
  label: lemlist Activities API
  slug: lemlist-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-activities-api-openapi.yml
- filename: lemlist-team-api-openapi.yml
  format: yaml
  label: lemlist Team API
  slug: lemlist-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-team-api-openapi.yml
- filename: lemlist-users-api-openapi.yml
  format: yaml
  label: lemlist Users API
  slug: lemlist-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-users-api-openapi.yml
- filename: lemlist-email-accounts-api-openapi.yml
  format: yaml
  label: lemlist Email Accounts API
  slug: lemlist-email-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-email-accounts-api-openapi.yml
- filename: lemlist-lemwarm-api-openapi.yml
  format: yaml
  label: lemlist lemwarm API
  slug: lemlist-lemwarm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-lemwarm-api-openapi.yml
- filename: lemlist-deliverability-alerts-api-openapi.yml
  format: yaml
  label: lemlist Deliverability Alerts API
  slug: lemlist-deliverability-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-deliverability-alerts-api-openapi.yml
- filename: lemlist-fields-api-openapi.yml
  format: yaml
  label: lemlist Fields API
  slug: lemlist-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-fields-api-openapi.yml
- filename: lemlist-stats-api-openapi.yml
  format: yaml
  label: lemlist Stats API
  slug: lemlist-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-stats-api-openapi.yml
authorization_urls:
- https://app.lemlist.com/oauth/authorize
description: ''
docs: https://developer.lemlist.com/mcp/setup
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Lemlist Scopes
name_suffix: OAuth Scopes
note: The lemlist OpenAPI declares only basicAuth, so no scopes are derivable from the spec. These scopes come from the RFC 8414 authorization-server metadata lemlist serves anonymously, which is what the MCP server and the CLI authorize against. lemlist publishes no prose scopes reference page; descriptions below are the resource + access-level the scope name states, not provider copy.
overview: 'lemlist publishes 14 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the lemlist API on a user''s behalf.


  Tokens are issued from https://app.lemlist.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: lemlist
provider_slug: lemlist
schemes:
- flows:
  - authorizationUrl: https://app.lemlist.com/oauth/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    tokenUrl: https://app.lemlist.com/oauth/token
  name: oauth2
  source: https://app.lemlist.com/.well-known/oauth-authorization-server
scope_count: 14
scope_names:
- campaigns:read
- campaigns:write
- leads:read
- leads:write
- sequences:read
- sequences:write
- team:read
- webhooks:read
- webhooks:write
- unsubscribes:read
- unsubscribes:write
- full_access
- openid
- email
scopes:
- description: Read campaigns, their sequences metadata and stats
  flows:
  - authorizationCode
  scope: campaigns:read
- description: Create, update, start, pause and duplicate campaigns
  flows:
  - authorizationCode
  scope: campaigns:write
- description: Read leads in campaigns and look leads up by id or email
  flows:
  - authorizationCode
  scope: leads:read
- description: Create, update, pause, resume, unsubscribe and delete leads, and set lead custom variables
  flows:
  - authorizationCode
  scope: leads:write
- description: Read campaign sequences and their steps
  flows:
  - authorizationCode
  scope: sequences:read
- description: Add, update and delete sequence steps and A/B test variants
  flows:
  - authorizationCode
  scope: sequences:write
- description: Read team information, senders and remaining credits
  flows:
  - authorizationCode
  scope: team:read
- description: List webhook subscriptions
  flows:
  - authorizationCode
  scope: webhooks:read
- description: Create and delete webhook subscriptions
  flows:
  - authorizationCode
  scope: webhooks:write
- description: Read unsubscribed contacts and variables
  flows:
  - authorizationCode
  scope: unsubscribes:read
- description: Unsubscribe and re-subscribe contacts and variables
  flows:
  - authorizationCode
  scope: unsubscribes:write
- description: Full access to the lemlist account. This is the only scope the MCP protected-resource metadata advertises as supported, so an MCP client authorizing against https://app.lemlist.com/mcp requests full_access rather than the granular set.
  flows:
  - authorizationCode
  scope: full_access
- description: OIDC — issue an id_token for the authenticated user
  flows:
  - authorizationCode
  scope: openid
- description: OIDC — include the user's email claim
  flows:
  - authorizationCode
  scope: email
slug: lemlist-scopes
source_filename: lemlist-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://app.lemlist.com/.well-known/oauth-authorization-server\nalso_served_at:\n- https://app.lemlist.com/.well-known/openid-configuration\n- https://api.lemlist.com/.well-known/oauth-authorization-server\n- https://api.lemlist.com/.well-known/openid-configuration\nnote: >-\n  The lemlist OpenAPI declares only basicAuth, so no scopes are derivable from the\n  spec. These scopes come from the RFC 8414 authorization-server metadata lemlist\n  serves anonymously, which is what the MCP server and the CLI authorize against.\n  lemlist publishes no prose scopes reference page; descriptions below are the\n  resource + access-level the scope name states, not provider copy.\ndocs: https://developer.lemlist.com/mcp/setup\nschemes:\n- name: oauth2\n  source: https://app.lemlist.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.lemlist.com/oauth/authorize\n    tokenUrl:\
  \ https://app.lemlist.com/oauth/token\n    code_challenge_methods:\n    - S256\nscope_count: 14\nscopes:\n- scope: campaigns:read\n  description: Read campaigns, their sequences metadata and stats\n  flows:\n  - authorizationCode\n- scope: campaigns:write\n  description: Create, update, start, pause and duplicate campaigns\n  flows:\n  - authorizationCode\n- scope: leads:read\n  description: Read leads in campaigns and look leads up by id or email\n  flows:\n  - authorizationCode\n- scope: leads:write\n  description: Create, update, pause, resume, unsubscribe and delete leads, and set\n    lead custom variables\n  flows:\n  - authorizationCode\n- scope: sequences:read\n  description: Read campaign sequences and their steps\n  flows:\n  - authorizationCode\n- scope: sequences:write\n  description: Add, update and delete sequence steps and A/B test variants\n  flows:\n  - authorizationCode\n- scope: team:read\n  description: Read team information, senders and remaining credits\n  flows:\n\
  \  - authorizationCode\n- scope: webhooks:read\n  description: List webhook subscriptions\n  flows:\n  - authorizationCode\n- scope: webhooks:write\n  description: Create and delete webhook subscriptions\n  flows:\n  - authorizationCode\n- scope: unsubscribes:read\n  description: Read unsubscribed contacts and variables\n  flows:\n  - authorizationCode\n- scope: unsubscribes:write\n  description: Unsubscribe and re-subscribe contacts and variables\n  flows:\n  - authorizationCode\n- scope: full_access\n  description: Full access to the lemlist account. This is the only scope the MCP\n    protected-resource metadata advertises as supported, so an MCP client authorizing\n    against https://app.lemlist.com/mcp requests full_access rather than the granular\n    set.\n  flows:\n  - authorizationCode\n- scope: openid\n  description: OIDC — issue an id_token for the authenticated user\n  flows:\n  - authorizationCode\n- scope: email\n  description: OIDC — include the user's email claim\n  flows:\n\
  \  - authorizationCode\nprotected_resources:\n- resource: https://app.lemlist.com/mcp\n  authorization_servers:\n  - https://app.lemlist.com\n  bearer_methods_supported:\n  - header\n  scopes_supported:\n  - full_access\n  source: https://app.lemlist.com/.well-known/oauth-protected-resource\ngap:\n  detail: >-\n    lemlist publishes 11 granular resource scopes plus full_access, but the MCP\n    protected-resource metadata lists only full_access as supported. An agent\n    connecting over MCP therefore cannot request least privilege today; the granular\n    scopes are only reachable through a direct OAuth client.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/scopes/lemlist-scopes.yml
summary_line: 14 scopes · authorizationCode
tags:
- Email Outreach
- Sales Engagement
- Cold Email
- Sales Automation
- LinkedIn Outreach
- Lead Generation
- Data Enrichment
- Deliverability
- CRM
- Multichannel Messaging
- Webhook
- MCP
token_urls:
- https://app.lemlist.com/oauth/token
---
